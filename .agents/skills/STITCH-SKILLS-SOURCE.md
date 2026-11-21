# Stitch skills cho nhóm Healthcare Portal

Nguồn: https://github.com/google-labs-code/stitch-skills. Các thư mục được bổ sung là bản sao của skill đã cài từ nguồn này, không phải skill nhóm tự viết.

| Skill | File | Vai trò |
|---|---|---|
| `design-md` | [SKILL.md](./design-md/SKILL.md) | Phân tích tài nguyên project thành DESIGN.md |
| `enhance-prompt` | [SKILL.md](./enhance-prompt/SKILL.md) | Chuẩn bị prompt thiết kế rõ ràng |
| `stitch::manage-design-system` | [SKILL.md](./manage-design-system/SKILL.md) | Nhận diện, quản lý và áp dụng Design System qua MCP |
| `stitch::generate-design` | [SKILL.md](./generate-design/SKILL.md) | Tạo/chỉnh màn hình qua MCP |
| `stitch::upload-to-stitch` | [SKILL.md](./upload-to-stitch/SKILL.md) | Tài nguyên hỗ trợ upload được skill quản lý Design System tham chiếu |

Giữ nguyên scripts/references/examples trong từng thư mục; chưa chạy scripts upload hoặc cài dependencies trong lần đưa tài liệu lên GitHub. Không đưa cấu hình đăng nhập hay khóa API vào repository.

Nguồn upstream của năm thư mục nằm tại `plugins/stitch-utilities/skills/` hoặc `plugins/stitch-design/skills/` trong repository trên. Nhánh nguồn là `main`; lần cài chưa ghi nhận commit upstream cụ thể. Bản trong repository này được truy vết theo commit của chính repository.

Giấy phép nguồn: Apache License 2.0; xem [STITCH-SKILLS-LICENSE](./STITCH-SKILLS-LICENSE). Giữ các ghi chú bản quyền có trong tài nguyên nguồn. Việc thêm skills không cài plugin hoặc kết nối MCP cho tài khoản các thành viên.

Trình tự gợi ý cho project đã có màn hình: `design-md` → nhóm rà soát → `stitch::manage-design-system` khi có MCP và phương án được duyệt → `enhance-prompt` / `stitch::generate-design` cho từng thay đổi → kiểm tra prototype và ghi nhận kết quả. Nếu chưa có MCP, có thể chuẩn bị prompt rồi thao tác thủ công trong Stitch; không tuyên bố đã chạy thay đổi từ xa.
