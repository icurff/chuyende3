# Phương án quản lý Design System — chưa áp dụng thay đổi

Ngày rà soát: 21/11/2026. Project ID: `17731225245642953956`.

## Căn cứ

Đã đọc skill `stitch::manage-design-system`, [DESIGN.md](./DESIGN.md) và tài nguyên xuất ở `assets/`. Chưa có Stitch MCP trong phiên, vì vậy chưa gọi được `list_design_systems` hoặc `get_project` để xác nhận asset ID, screen instance ID và liên kết áp dụng hiện hành.

Không nhầm một file Markdown Design System xuất ra với bằng chứng đầy đủ về danh tính tài sản Design System trên dịch vụ.

## Kết quả đối chiếu snapshot

- Có tài liệu nguồn mang tên **An Tâm Healthcare Portal**.
- Đoạn cấu hình thiết kế trong cả sáu HTML giống nhau.
- Màu chính `#00544F`, nền `#F7FAF8`, ba nhóm màu lịch hẹn và các font Plus Jakarta Sans / Be Vietnam Pro / Source Code Pro khớp hồ sơ tổng hợp.
- Bo góc đang áp dụng gồm 8px cho nút/input, 12px cho thẻ, 16px cho tóm tắt; badge dạng viên thuốc.
- Chưa có căn cứ cần tạo mới hoặc áp dụng lại hàng loạt chỉ để đổi tên/file tài liệu.

## Phương án đề xuất

1. Giữ nguyên palette/font/spacing/bo góc đang khớp.
2. Khi có MCP, đọc danh sách Design System và project metadata; nhận diện đúng tài sản đã có và các màn hình liên quan. Chưa tìm được không đồng nghĩa tài sản không tồn tại.
3. Nếu tài sản đã khớp, giữ nguyên, không tạo/upload thêm.
4. Nếu có chênh lệch, trình bày delta và phạm vi ảnh hưởng; chỉ cập nhật tài sản hiện hữu khi công cụ hỗ trợ và hành động được duyệt.
5. Nếu chưa xác định được tài sản hoặc không có cách cập nhật phù hợp, dừng thao tác từ xa để làm rõ; không tự tạo một bản khác thay thế.

`DESIGN.md` hiện tại có cả bằng chứng, nhận xét và đề xuất chưa duyệt. Không upload toàn bộ như thể mọi nội dung đều là quy tắc đã thống nhất. Nếu cần áp dụng, chuẩn bị bản quy tắc được duyệt riêng.

## Màn hình có thể bị ảnh hưởng

S01–S06 trong [mục lục thiết kế](./README.md) là phạm vi dự kiến nếu thay token chung: chọn lịch, chờ xác nhận, đề nghị đổi, chi tiết yêu cầu nhân viên, danh sách và kết quả xác nhận. Chưa xác nhận đây là danh sách đầy đủ của project hoặc đích áp dụng theo screen ID.

Sửa validation/loading chỉ nên nhắm component/màn hình liên quan, không coi là thay đổi toàn bộ theme. Các đề xuất responsive, contrast và keyboard cần kiểm tra riêng; chưa có kết quả chứng minh đã đạt.

## Trạng thái bàn giao

Chưa tạo, upload, cập nhật hoặc áp dụng Design System lên project. Lần đóng gói GitHub chỉ bổ sung tài liệu và snapshot nguồn để nhóm review.
