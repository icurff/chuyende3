# Healthcare Portal — Design System & Prototype

Cập nhật hồ sơ: 21/11/2026. Project: [Cổng Đặt Lịch Khám Agile](https://stitch.google.com/projects/17731225245642953956).

## Tài liệu để review

| Tài liệu | Vai trò |
|---|---|
| [DESIGN.md](./DESIGN.md) | Tổng hợp màu, typography, bố cục, spacing, component và trạng thái. Phần “ĐỀ XUẤT” chưa được áp dụng |
| [DESIGN-SYSTEM-REVIEW.md](./DESIGN-SYSTEM-REVIEW.md) | Kết quả đối chiếu và phương án tránh tạo Design System trùng lặp |
| [Design System nguồn](./assets/an-tâm-healthcare-portal-design-system.md) | Tài liệu nguyên bản xuất từ Stitch, giữ để đối chiếu |
| [Phân công nhóm](../team/Phan-cong-nhom-Design-System-Prototype-Stitch.docx) | Phân công TV01–TV09, cách phối hợp và đầu ra; nhóm điền tên/hạn thực tế |

## Sáu màn hình trong snapshot

| Mã | Màn hình / HTML nguồn |
|---|---|
| S01 | [Người đặt — Chọn bác sĩ và thời gian](./assets/người-đặt-khám-chọn-bác-sĩ-và-thời-gian/code.html) |
| S02 | [Người đặt — Kết quả gửi yêu cầu, chờ xác nhận](./assets/người-đặt-khám-kết-quả-gửi-yêu-cầu-chờ-xác-nhận/code.html) |
| S03 | [Người đặt — Đề nghị thời gian khác](./assets/người-đặt-khám-đề-nghị-thời-gian-khác/code.html) |
| S04 | [Nhân viên — Chi tiết yêu cầu](./assets/nhân-viên-tiếp-nhận-chi-tiết-yêu-cầu-yc-1046/code.html) |
| S05 | [Nhân viên — Danh sách yêu cầu](./assets/nhân-viên-tiếp-nhận-danh-sách-yêu-cầu/code.html) |
| S06 | [Nhân viên — Kết quả xác nhận](./assets/nhân-viên-tiếp-nhận-kết-quả-xác-nhận-lịch/code.html) |

Các file HTML là tài nguyên để đọc mã và đối chiếu, không được GitHub tự hiển thị như website. Bản export tham chiếu một số đường dẫn prototype logic khác tên thư mục thực tế; chưa sửa vì cần giữ nguyên snapshot nguồn. Không coi mở HTML local là đã kiểm thử toàn bộ luồng Stitch. Các font và Tailwind trong nguồn còn phụ thuộc tài nguyên mạng.

## Góp ý ưu tiên

- Người xem có phân biệt được gửi yêu cầu và lịch đã được xác nhận không?
- Thông tin người đặt/người liên hệ và người được khám đã rõ chưa?
- Nhân viên biết cần xử lý yêu cầu nào và kết quả thay đổi là gì không?
- Nút, form, card, ô giờ và badge có dùng cùng quy tắc không?
- Có lỗi nào quan sát được về bố cục, chữ dài, màn hình nhỏ, bàn phím hoặc thông báo lỗi? Ghi điều kiện thử thay vì chỉ kết luận “chưa responsive”.

Dùng mẫu issue [Góp ý thiết kế](../../.github/ISSUE_TEMPLATE/design-review.md), hoặc tạo issue theo cấu trúc trong README gốc. Chưa có kết quả kiểm tra người dùng nào được tạo trong lần đóng gói này.

## Skills

Các skill liên quan được lưu trong `.agents/skills`; xem [nguồn và cách dùng](../../.agents/skills/STITCH-SKILLS-SOURCE.md). Có skill không đồng nghĩa đã kết nối Stitch MCP. Chỉ những thao tác ghi rõ đã thực hiện mới được coi là đã chạy.
