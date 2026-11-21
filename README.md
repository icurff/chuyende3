# Healthcare Portal — Chuyên đề 3

Tài liệu môn Quản lý dự án với Agile/Scrum của nhóm 9 thành viên. Repository tập hợp hồ sơ nghiên cứu, bản thiết kế và các skill để mọi người đọc, trao đổi và kiểm tra quyết định của nhóm.

## Đọc từ đâu?

| Nội dung | Đường dẫn |
|---|---|
| Research & Discovery và bộ đầu ra hiện hành | [Mục lục nghiên cứu](./docs/research-discovery/README.md) |
| Design System & Prototype | [Mục lục thiết kế và cách góp ý](./docs/design-prototype/README.md) |
| Quy tắc thiết kế tổng hợp từ Stitch | [DESIGN.md](./docs/design-prototype/DESIGN.md) |
| Phương án giữ/cập nhật Design System | [Design System Review](./docs/design-prototype/DESIGN-SYSTEM-REVIEW.md) |
| Phân công nhóm trên Stitch | [File Word](./docs/team/Phan-cong-nhom-Design-System-Prototype-Stitch.docx) |
| Nguồn và cách dùng các Stitch skills được bổ sung | [Stitch Skills](./.agents/skills/STITCH-SKILLS-SOURCE.md) |

Project Stitch: https://stitch.google.com/projects/17731225245642953956.

## Trạng thái

- Bộ Research & Discovery đã có trên repository được giữ nguyên; đọc README của phần đó để xác định tài liệu đầu vào và đầu ra hiện hành.
- Phần thiết kế được bổ sung từ bản xuất Stitch ngày 21/11/2026: một tài liệu Design System gốc và sáu màn hình HTML. Đây là snapshot để review, không tự đồng bộ với project sau này.
- Các thông tin cá nhân/lịch khám trong thiết kế là dữ liệu mẫu cho mô phỏng. Không coi chúng là phỏng vấn hoặc dữ liệu người dùng thật.
- Chưa xác nhận `assetId` và liên kết Design System qua Stitch MCP; chưa upload hoặc áp dụng lại Design System lên project.
- Màn hình xuất là tài nguyên thiết kế; liên kết nội bộ của bản xuất chưa được sửa/kiểm thử để chạy như một website. Không có ứng dụng backend được triển khai qua lần bổ sung này.

## Góp ý cho nhóm

Mở tab **Issues → New issue** và chọn mẫu **Góp ý thiết kế** nếu mẫu xuất hiện. Hoặc tạo issue có tiêu đề chỉ rõ màn hình/vấn đề và ghi:

1. Màn hình hoặc đường dẫn tài liệu đang xem.
2. Điều chưa rõ/sai và bước tái hiện nếu có.
3. Ảnh đánh dấu hoặc đoạn nội dung liên quan, dùng dữ liệu mẫu.
4. Kết quả mong đợi và đề xuất sửa, kèm lý do.

Ưu tiên nhận xét về trạng thái lịch hẹn, phân biệt người đặt/người khám, luồng xử lý nhân viên, tính nhất quán component và bố cục. Tách lỗi quan sát được khỏi đề xuất cá nhân; chưa thử thì ghi rõ chưa thử.

Người phụ trách tổng hợp và thống nhất thay đổi trước khi tích hợp vào project chính. Không cần mỗi thành viên tự tạo một Design System mới.
