ỨNG DỤNG TÍNH LƯƠNG GIA SƯ – BẢN 2
================================

TÍNH NĂNG CHÍNH
- Tạo nhiều lớp/môn; nhập tên học sinh, học phí theo buổi và các thứ học.
- Tự tạo lịch học từng tháng, đánh dấu nghỉ/vắng để không tính tiền.
- Xem lương toàn bộ lớp theo tháng, lương dự kiến và lương đã đến ngày.
- Nhấn vào MỘT LỚP để xem thu nhập riêng của lớp và từng ngày học/nghỉ.
- Chuyển qua các tháng trước hoặc tháng sau ngay trong trang chi tiết lớp.
- Đánh dấu nghỉ ngay trong trang chi tiết lớp; tiền lương và tin nhắn tự cập nhật.
- Tự viết tin nhắn báo phụ huynh: các ngày học, ngày nghỉ và học phí.
- Chỉnh sửa tin nhắn, sao chép để dán vào Zalo/Messenger/SMS hoặc mở Chia sẻ trên iPhone.
- Hỗ trợ sửa giá/lịch theo mốc ngày mà vẫn giữ các tháng cũ.
- Sao lưu và khôi phục dữ liệu ra/vào tệp JSON.

LƯU Ý QUAN TRỌNG VỀ TIỀN LƯƠNG VÀ TIN NHẮN
- Các buổi đã qua mà không được đánh dấu nghỉ sẽ được coi là đã dạy.
- Lương dự kiến có thể tính cả các buổi tương lai; tin nhắn phụ huynh tháng hiện tại
  chỉ tính các buổi có ngày không muộn hơn hôm nay.
- Ngày nghỉ đã đánh dấu sẽ không tính học phí.
- Tin nhắn chưa tự gửi đi; bạn phải chọn đúng người nhận trong ứng dụng nhắn tin.
- Cần kiểm tra nội dung và số tiền trước khi gửi cho phụ huynh.

CHẠY TRÊN WINDOWS
1. Giải nén ZIP.
2. Trong Visual Studio Code, chọn File > Open Folder rồi mở thư mục tinh-luong-gia-su.
3. Mở Terminal tại thư mục chứa index.html và chạy:
       py -m http.server 5500
   Hoặc:
       python -m http.server 5500
4. Mở trình duyệt tại http://localhost:5500
5. Dừng server bằng Ctrl+C.

ĐƯA LÊN IPHONE BẰNG GITHUB PAGES (MIỄN PHÍ)
1. Mở repository GitHub Pages hiện tại của bạn.
2. TRƯỚC KHI CẬP NHẬT: mở app cũ và nhấn Sao lưu để lưu một bản JSON.
3. Tải/commit các file của bản mới vào cùng vị trí ở repository cũ.
4. Khi trang đã cập nhật, mở lại bằng Safari; làm mới trang và mở lại app nếu cần.
5. Nếu chưa có GitHub Pages: tạo repository public, tải các file lên,
   chọn Settings > Pages > Deploy from a branch > main > / (root).
6. Mở link trang bằng Safari trên iPhone > Chia sẻ > Thêm vào Màn hình chính.

CHÚ Ý DỮ LIỆU
- Bản mới giữ cùng khóa localStorage với bản cũ để đọc dữ liệu đã nhập, với điều
  kiện vẫn dùng cùng URL/nguồn gốc và cùng phạm vi dữ liệu trình duyệt.
- Nếu đổi tên trang, đổi domain, đổi iPhone hoặc cài ở nơi khác, dữ liệu không
  tự chuyển theo. Hãy dùng Sao lưu ở bản cũ và Khôi phục ở bản mới.
- GitHub Pages với repository public công khai mã nguồn; dữ liệu lớp và lương
  nhập trên iPhone được lưu cục bộ, không tự tải lên GitHub.
- Xóa dữ liệu Safari hoặc app có thể làm mất thông tin. Hãy sao lưu định kỳ.
- Đây là PWA, không phải file .ipa hay app được phát hành trên App Store.
