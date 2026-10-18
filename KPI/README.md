# KPI Portal Demo

Ứng dụng web minh họa quy trình quản lý chỉ tiêu và đánh giá KPI cho doanh nghiệp nhà nước, đơn vị hành chính/sự nghiệp và cán bộ, công chức, viên chức.

## Chạy website

- **XAMPP:** khởi động Apache, sau đó mở `http://localhost/KPI/`.
- **Không dùng XAMPP:** mở `index.html` bằng trình duyệt hiện đại.

Website không cần cài thêm package hoặc cấu hình máy chủ.

## Chức năng

- Dashboard và báo cáo được tổng hợp từ dữ liệu đang lưu.
- Thêm, sửa, xóa đơn vị, cán bộ và chỉ tiêu KPI.
- Tạo phiếu đánh giá theo kỳ, nhập giá trị thực tế và điểm (0–100) cho từng KPI, thêm giải trình, chuyển trạng thái.
- Tự tính điểm tổng hợp theo công thức `tổng(điểm KPI × trọng số) / tổng(trọng số)` trên các KPI được chấm. Trạng thái “Đã hoàn thành” và “Chờ phê duyệt” yêu cầu nhập điểm đầy đủ cho bộ KPI áp dụng.
- Tìm kiếm/lọc, xuất danh sách CSV, tải và khôi phục bản sao lưu JSON.
- Lưu dữ liệu trong `localStorage` của trình duyệt hiện tại; tải lại trang không làm mất thay đổi.

## Dữ liệu và giới hạn

Đây là bản demo chạy cục bộ, không có API, cơ sở dữ liệu dùng chung, đăng nhập, phân quyền thật hoặc đồng bộ giữa các máy. Tên tổ chức và điểm đánh giá mẫu không phải số liệu chính thức. Không nhập dữ liệu cá nhân nhạy cảm hoặc sử dụng kết quả demo để ra quyết định nhân sự/doanh nghiệp.

Khi xóa dữ liệu trình duyệt, dữ liệu đã lưu sẽ mất. Hãy tạo bản sao lưu JSON trong **Cài đặt → Sao lưu dữ liệu** trước khi chuyển trình duyệt hoặc máy tính.

Để đưa vào sử dụng chính thức cần bổ sung máy chủ và cơ sở dữ liệu, xác thực/phân quyền, nhật ký kiểm toán phía máy chủ, HTTPS, chính sách lưu trữ và rà soát pháp lý các tiêu chí đánh giá theo từng đối tượng.
