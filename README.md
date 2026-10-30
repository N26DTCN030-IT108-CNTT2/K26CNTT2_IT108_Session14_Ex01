# K26CNTT2_IT108_Session14_Ex01
Bài tập 1


## Phần 1 (Phân tích): 3 hậu quả của "Thảm họa dữ liệu truyền thống"Trường hợp của Nam gặp phải các rủi ro điển hình khi chỉ dựa hoàn toàn vào lưu trữ cục bộ (Local Storage) và phương pháp thủ công qua Zalo:
### Mất dữ liệu vĩnh viễn không thể khôi phục (Data Loss & Overwrite): Khi Nam lỡ tay xóa đoạn code quan trọng và bấm Ctrl+S trên ổ đĩa cục bộ, hệ điều hành sẽ ghi đè trực tiếp lên tệp hiện có. Không có bản sao lưu tự động hay lịch sử thay đổi (Version History) trên ổ cứng cục bộ, dẫn đến việc đoạn code quý giá biến mất hoàn toàn.

### Hỗn loạn kiểm soát phiên bản (Version Control Chaos): Việc đặt tên tệp thủ công kiểu v1.py, v2_final.py rất dễ gây nhầm lẫn. Khi làm việc nhóm, việc gửi file qua Zalo khiến các thành viên khác không biết đâu mới thực sự là phiên bản mới nhất, dẫn đến xung đột mã nguồn (Merge Conflict) và mất thời gian ráp nối thủ công.

### Phụ thuộc hoàn toàn vào thiết bị cá nhân (Single Point of Failure): Lập luận "file chỉ có trên máy em" cho thấy rủi ro chí mạng: khi máy tính của Nam gặp sự cố phần cứng (hỏng ổ cứng, sập nguồn, mất máy), toàn bộ tiến độ của dự án Startup "Smart Food" bị đình trệ vì không có bản dự phòng trên không gian đám mây (Cloud Workspace).

Phần 2 (Sửa lỗi): Đề xuất quy trình Hybrid Workflow (1-Click Version History)Để giúp Nam khắc phục triệt để tình trạng trên mà vẫn đảm bảo tốc độ làm việc mượt mà, quy trình kết hợp giữa Local và Cloud được đề xuất như sau:
Bước 1: Thiết lập môi trường làm việc kết hợp (Hybrid Workspace)Lưu trữ cục bộ để code: Nam vẫn viết code trên máy cá nhân bằng các công cụ quen thuộc (như VS Code) để đảm bảo hiệu năng cao, không sợ giật lag do kết nối mạng.Đồng bộ thời gian thực lên Cloud (Google Drive / GitHub): Sử dụng các dịch vụ lưu trữ đám mây có tính năng tự động đồng bộ (như Google Drive for Desktop) hoặc công cụ quản lý mã nguồn chuyên nghiệp (Git & GitHub) để mọi thay đổi được lưu trữ an toàn trên mây ngay khi lưu file.
Bước 2: Kích hoạt và tận dụng "Version History"Trên Google Drive / Docs: Nếu lưu file dạng văn bản/script lên Drive, khi cần quay lại trạng thái cũ, Nam chỉ cần nhấn chuột phải vào file $\rightarrow$ Manage versions (Quản lý phiên bản) hoặc Version history, sau đó chọn mốc thời gian trước khi lỗi xảy ra và khôi phục chỉ trong 1-click.Trên Git / GitHub: Sử dụng lệnh git commit định kỳ theo từng tính năng hoàn thiện. Nếu xảy ra sự cố xóa nhầm code, Nam chỉ cần dùng lệnh git checkout hoặc xem lại lịch sử commit trên GitHub để lấy lại chính xác đoạn code đã mất mà không sợ ghi đè nhầm.
Bước 3: Chuẩn hóa quy trình giao tiếp nhómThay vì gửi file .py qua Zalo gây trôi tin nhắn và đè file lung tung, nhóm "Smart Food" sẽ sử dụng chung một repository trên GitHub hoặc thư mục chia sẻ trên Cloud với phân quyền rõ ràng (Editor/Viewer), giúp loại bỏ hoàn toàn việc thất lạc mã nguồn.
