# Design System: An Tâm Healthcare Portal

**Project ID:** `17731225245642953956`  
**Tên trên canvas:** Cổng Đặt Lịch Khám Agile  
**Ngày phân tích:** 21/11/2026 — Asia/Saigon  
**Trạng thái:** Tổng hợp từ tài nguyên hiện có; chưa áp dụng thay đổi lên project.

## Phạm vi và cách phân biệt thông tin

Áp dụng hướng phân tích của skill `design-md`: nhận diện ngôn ngữ thị giác, màu theo vai trò, typography, hình khối, thành phần và bố cục. Phiên làm việc chưa có Stitch MCP, nên không thực hiện được tuyến lấy metadata qua MCP như skill mô tả. Thay vào đó, đã mở đúng project bằng Opera GX và dùng Export → chọn các màn hình → `.zip` để đọc tài nguyên xuất trực tiếp từ project. Không gửi prompt tạo/sửa hoặc áp dụng Design System lên Stitch.

Nguồn gồm một tài liệu Design System và sáu màn hình HTML. Các giá trị chính xác dưới đây lấy từ tài liệu/HTML, không lấy mẫu màu hoặc ước lượng pixel từ ảnh canvas. Không khẳng định đây là toàn bộ màn hình của project ngoài tập đã xuất.

Quy ước:

- **ĐÃ CÓ — khai báo:** được ghi trong Design System hoặc cấu hình HTML, chưa đồng nghĩa đã dùng ở mọi màn hình.
- **ĐÃ CÓ — áp dụng:** tìm thấy thành phần/lớp hoặc nội dung tương ứng trong HTML xuất; chưa phải kết quả thử tương tác trên trình duyệt.
- **ĐỀ XUẤT:** bổ sung của agent, chưa duyệt và chưa thay đổi project. Không tự coi là quy tắc hiện có.

## 1. Visual Theme & Atmosphere

### ĐÃ CÓ

Tài liệu xuất mô tả hướng **Corporate / Modern Minimalism**: nền sáng, xanh ngọc đậm cho hành động chính, phân cấp nội dung bằng khoảng cách, tiêu đề và lớp bề mặt thay vì hiệu ứng trang trí.

HTML dùng nền xanh xám rất nhạt `#F7FAF8`, thẻ trắng `#FFFFFF`, chữ đậm `#181C1C`, viền xám xanh và góc bo vừa phải. Không tìm thấy lớp `shadow-*` hoặc khai báo `box-shadow` trong sáu HTML được đọc. Giao diện vì vậy thể hiện chiều sâu chủ yếu bằng bề mặt và viền; tên component `card-elevated` không chứng minh có bóng đổ.

Mục tiêu được khai báo trong nguồn là giúp người đặt khám và nhân viên quét thông tin, nhận biết trạng thái. Đây là ý đồ thiết kế, chưa phải hiệu quả đã được kiểm tra với người dùng.

Header chung có nhận diện phòng khám, nhãn “Dữ liệu mẫu” và điều hướng chuyển vai trò. Footer ghi rõ demo Agile/Scrum. Các tên, lịch và thông tin người khám trong bản xuất là dữ liệu mẫu, không được xem như dữ liệu nghiên cứu thực tế.

## 2. Color Palette & Roles

### 2.1. ĐÃ CÓ — màu nền và tương tác của giao diện sáng

Các token dưới đây được khai báo trong tài liệu gốc và cấu hình của cả sáu HTML. Vai trò được đối chiếu với lớp sử dụng trong màn hình.

| Token | Giá trị | Mô tả và vai trò hiện có |
|---|---|---|
| `light-primary` | `#00544F` | Xanh ngọc đậm; nút chính, liên kết/điểm nhấn, viền lựa chọn |
| `light-on-primary` | `#FFFFFF` | Chữ/icon trên nền primary |
| `light-primary-container` | `#0D6E68` | Xanh ngọc sáng hơn; được dùng cho hover nút chính |
| `light-on-primary-container` | `#9CEDE5` | Xanh ngọc nhạt; cặp chữ khai báo cho primary-container |
| `light-secondary` | `#476461` | Xanh xám; màu hỗ trợ được khai báo |
| `light-secondary-container` | `#C9E9E5` | Nền xanh rất nhạt; avatar/nhóm lựa chọn, có nơi dùng thêm độ trong suốt |
| `light-on-secondary-container` | `#183533` | Chữ xanh đậm trên nền secondary-container |
| `light-tertiary` | `#753A21` | Nâu ấm; màu bổ trợ khai báo, không mặc định là trạng thái lịch hẹn |
| `light-tertiary-container` | `#925136` | Nền bổ trợ nâu; thuộc palette khai báo |
| `light-surface`, `light-background` | `#F7FAF8` | Nền trang sáng, tách nhẹ với các khối trắng |
| `light-surface-container-lowest`, `light-surface-bright` | `#FFFFFF` | Bề mặt header, form, card và khối nội dung |
| `light-surface-container-low` | `#F1F4F3` | Lớp bề mặt thấp được khai báo |
| `light-surface-container` | `#EBEFED` | Nhóm lựa chọn, nền trung tính, ô giờ không khả dụng |
| `light-surface-container-high` | `#E6E9E7` | Lớp bề mặt cao được khai báo |
| `light-surface-container-highest` | `#E0E3E2` | Lớp bề mặt cao nhất được khai báo |
| `light-on-surface`, `light-on-background` | `#181C1C` | Chữ chính |
| `light-on-surface-variant` | `#3E4947` | Mô tả, nhãn phụ, thông tin thứ cấp |
| `light-outline` | `#6E7977` | Viền/chi tiết nhấn phụ |
| `light-outline-variant` | `#BEC9C7` | Viền khối, input, đường phân cách; HTML có dùng biến thể opacity |
| `light-error` / `light-on-error` | `#BA1A1A` / `#FFFFFF` | Cặp màu lỗi đã khai báo; chưa đủ bằng chứng có đầy đủ UI lỗi form |
| `light-error-container` / `light-on-error-container` | `#FFDAD6` / `#93000A` | Cặp nền/chữ lỗi đã khai báo |

### 2.2. ĐÃ CÓ — màu ngữ nghĩa lịch hẹn

| Trạng thái | Màu chính | Nền badge | Chữ badge |
|---|---|---|---|
| Chờ xác nhận | `status-pending: #92400E` | `#FEF3C7` | `#78350F` |
| Đã xác nhận | `status-confirmed: #065F46` | `#D1FAE5` | `#064E3B` |
| Đề nghị thời gian khác | `status-reschedule: #3730A3` | `#E0E7FF` | `#312E81` |

Các badge dùng màu nền/chữ cùng icon và nhãn; viền có biến thể `status-*/20`. Màu trên là giá trị token gốc; khi lớp có `/20`, `/40`, `/50` thì kết quả hiển thị còn phụ thuộc độ trong suốt và nền phía sau. Không coi màu badge là màu thương hiệu mới.

### 2.3. Theme tối và giới hạn xác minh

Nguồn có khai báo theme tối, ví dụ primary `#84D5CD`, on-primary `#003734`, surface/background `#101414`, on-surface `#E0E3E2`, outline `#889391`. Tuy nhiên body của cả sáu HTML đang dùng `bg-light-surface text-light-on-surface`; chưa xác nhận có công tắc hoặc quy tắc đổi toàn bộ giao diện sang tối. Theme tối là **khai báo hiện có, chưa xác nhận áp dụng hoàn chỉnh**.

Tài liệu gốc có tuyên bố tương phản đạt WCAG AA; lần phân tích này chưa đo tất cả cặp màu, trạng thái và nội dung hiển thị. Không lặp lại tuyên bố đó như kết quả kiểm định. Các giá trị bổ sung đầy đủ được giữ nguyên trong tài liệu nguồn ở thư mục `assets`.

## 3. Typography Rules

### 3.1. ĐÃ CÓ — font và phân vai

- **Plus Jakarta Sans:** headline/display; HTML cũng dùng `font-headline` ở tên phòng khám và tên bác sĩ.
- **Be Vietnam Pro:** nội dung, form, nhãn và thao tác; các alias `title`, `body`, `label` được khai báo cùng font này.
- **Source Code Pro:** mã yêu cầu, giờ và các dữ liệu cần căn số; HTML dùng `font-mono` và `tabular-nums` ở nhiều chỗ.
- **Material Symbols Outlined:** bộ icon; có khai báo kích thước 16/18/20/22px trong các phần đã đọc. Đây là font icon, không phải font nội dung.

HTML liên kết Google Fonts cho ba font chữ và font icon. Đây là bằng chứng có yêu cầu tải font, không chứng minh font luôn tải thành công trong mọi môi trường hoặc bản demo offline.

### 3.2. ĐÃ CÓ — thang chữ khai báo

| Token | Cỡ / chiều cao dòng | Độ đậm | Giãn chữ | Vai trò trong thiết kế |
|---|---|---|---|---|
| `display-lg` | 36 / 44px | 700 | −0.5px | Tiêu đề lớn được khai báo |
| `display-lg-mobile` | 28 / 36px | 700 | −0.25px | Biến thể mobile khai báo; không tự khẳng định đã áp dụng breakpoint |
| `headline-lg` | 28 / 36px | 700 | −0.25px | Tiêu đề trang; tìm thấy trong HTML |
| `headline-md` | 22 / 30px | 600 | −0.15px | Tiêu đề bước/nhóm |
| `title-lg` | 18 / 26px | 600 | 0px | Tên bác sĩ/khối, nhận diện header |
| `title-md` | 16 / 24px | 600 | 0px | Thông tin nhấn trong khối |
| `body-lg` | 16 / 24px | 400 | 0px | Mô tả chính |
| `body-md` | 14 / 22px | 400 | 0px | Nội dung thường, mô tả, form |
| `label-lg` | 14 / 20px | 600 | 0px | Nhãn thao tác chính |
| `label-md` | 12 / 16px | 600 | +0.2px | Nhãn trường, filter, badge |
| `label-sm` | 11 / 16px | 500 | +0.2px | Nhãn nhỏ/footer |
| `mono-md` | 13 / 18px | 500 | 0px | Mã và khung giờ |

Các con số trong bảng là token trong source, không phải đo từ ảnh. Font thực tế của một phần tử phải xem thêm lớp `font-*`; không suy ra font chỉ từ tên `title-lg` hoặc `headline-*` của cỡ chữ.

### 3.3. ĐÃ CÓ — nội dung giao diện

- Thuật ngữ “Yêu cầu đặt lịch” và “Gửi yêu cầu đặt lịch” xuất hiện cùng giải thích gửi chưa đồng nghĩa đã xác nhận.
- Ba trạng thái chính: “Chờ xác nhận”, “Đã xác nhận”, “Đề nghị thời gian khác”.
- Mã dùng tiền tố `YC-`, giờ định dạng 24h, ngày hiển thị `DD/MM/YYYY` trong dữ liệu mẫu.
- Màn hình đặt đã tách “Người đặt / Người liên hệ” và “Người được khám”, có lựa chọn đặt cho người thân hoặc chính mình.

## 4. Component Stylings

### 4.1. ĐÃ CÓ — Buttons

Nút chính là khối xanh ngọc đậm `#00544F`, chữ trắng, góc 8px. CTA gửi yêu cầu trong HTML dùng chiều cao tối thiểu 44px, padding ngang 24px/dọc 8px; hover sang `#0D6E68`, có lớp focus-visible cho viền nhấn cách phần tử 2px. Các liên kết điều hướng được tạo hình giống nút, nên không coi mọi CTA là phần tử `<button>`.

Lựa chọn phụ thường là nền trắng/trung tính, viền xanh xám, chữ xanh đậm hoặc chữ phụ. Chuyển vai trò, lọc chuyên khoa và chế độ đặt hộ dùng nhóm lựa chọn; phần đang chọn được phân biệt bằng nền/viền/chữ.

Chưa thấy trạng thái loading chung được xác lập trong tập tài nguyên. Không khẳng định nút có đầy đủ ngữ nghĩa disabled và thao tác bàn phím chỉ vì hình thức giống nút.

### 4.2. ĐÃ CÓ — Inputs & Forms

Input nền trắng, viền `#BEC9C7`, góc 8px, padding ngang 16px/dọc 8px; nhãn đặt phía trên. Trong màn hình chọn lịch, label liên kết với input bằng `for`/`id`. Focus được khai báo bằng viền và ring primary. Trường số điện thoại dùng `type="tel"`, font mono; trường “Lý do khám” được ghi không bắt buộc.

Nhóm thông tin người đặt và người được khám được tách bằng nhãn cùng đường phân cách. Đây là cách phân nhóm đang có, không phải đề xuất mới của tài liệu này.

Token màu lỗi đã có nhưng không tìm thấy `aria-invalid` trong sáu HTML. Điều đó chưa chứng minh không có mọi cách validation; chỉ chưa đủ bằng chứng về một hệ thống lỗi form đầy đủ, liên kết thông báo với trường và trạng thái gửi không hợp lệ.

### 4.3. ĐÃ CÓ — Cards & Containers

- Thẻ bác sĩ: nền trắng, góc 12px, padding 24px, cấu trúc tên/chuyên khoa/phòng/mô tả và footer. Thẻ đang chọn có viền primary 2px và nhãn “Đang chọn”; thẻ thường viền 1px, có lớp đổi màu viền khi hover.
- Avatar: dạng tròn, dùng chữ viết tắt trong dữ liệu mẫu và nền trung tính/xanh nhạt.
- Tóm tắt yêu cầu: góc 16px, nền trắng, viền mảnh, padding 24px; đặt bên phải trên bố cục desktop. Chiều sâu đến từ tương phản bề mặt, không phải bóng đổ nặng.
- Khối thông báo quy trình: nền pending pha trong suốt, viền pending nhạt, icon thông tin và nội dung giải thích.

Tên component dạng `card-interactive-2`/`card-elevated` trong source là định danh, không được suy ra hành vi đã kiểm thử chỉ từ tên đó.

### 4.4. ĐÃ CÓ — Ô chọn ngày và khung giờ

Ngày hiển thị dạng nút/thẻ có thứ và ngày. Ngày đang chọn dùng viền primary 2px, nền secondary-container pha trong suốt; ngày khác dùng nền trắng và viền nhẹ.

Ô giờ chia sáng/chiều. Trong từng buổi, lưới có ba cột và khoảng cách 8px. Góc 8px, font Source Code Pro 13px, padding 8px:

| Trạng thái giờ | Biểu hiện trong HTML |
|---|---|
| Khả dụng | Nền trắng, chữ chính, viền nhẹ, hover viền primary |
| Đang chọn | Nền primary, chữ trắng, viền primary 2px |
| Không khả dụng | `disabled`, nền surface-container, chữ phụ, gạch ngang và con trỏ không cho phép |

Màn hình ghi khung giờ 30 phút. Đây là thông số bối cảnh mô phỏng hiện có, không phải quy tắc thiết kế bắt buộc cho mọi phòng khám. Chưa kiểm tra hành vi khi hai yêu cầu cùng chọn hoặc khung giờ vừa mất khả dụng.

### 4.5. ĐÃ CÓ — Status Badges

Badge dạng viên thuốc, góc 9999px, padding ngang 8px/dọc 4px, khoảng cách icon/chữ 4px. Nhãn dùng cỡ 12px, icon thường 16px, kết hợp nền/chữ/viền theo trạng thái ở mục 2.2. Tìm thấy `role="status"` ở nhiều badge và `aria-hidden="true"` ở icon trang trí.

Không dùng primary xanh ngọc để thay thế tùy ý ba màu trạng thái. Trạng thái được giải thích bằng chữ; không buộc người dùng chỉ suy ra từ màu.

### 4.6. ĐÃ CÓ — Danh sách và bảng nhân viên

Màn hình danh sách có vùng thống kê/lọc phía trên và bảng yêu cầu. Các ô dữ liệu có padding ngang/dọc 16px ở các phần đã đọc; tên người đặt và người khám được phân biệt; mã/giờ dùng cách căn số nhất quán. Badge và thao tác được đặt theo từng dòng.

Tài liệu nguồn mô tả không cần cuộn ngang; lần này chưa thử chiều rộng nhỏ và nội dung dài nên chưa xác nhận tuyên bố đó. Các liên kết trong HTML có đường dẫn prototype logic; chưa khẳng định ZIP xuất ra chạy liền mạch nếu mở trực tiếp.

## 5. Layout Principles

### 5.1. ĐÃ CÓ — khung trang và lưới

- Header và main dùng vùng căn giữa, giới hạn `max-width: 1280px` trong HTML, lề/padding ngang 24px. Header sticky ở đầu trang.
- Màn hình đặt: một cột ở cấu hình nền, chuyển thành lưới 12 cột ở biến thể `lg`; phần chọn/nhập chiếm 8, tóm tắt chiếm 4; khoảng cách 32px. Tóm tắt có `lg:sticky lg:top-24`.
- Danh sách nhân viên: main một cột rộng, phân nhóm lọc/thống kê và bảng. Các màn hình chi tiết/kết quả được giữ trong cùng app shell.
- HTML chứa lớp responsive `sm`, `md`, `lg`; đây là bằng chứng có khai báo đáp ứng, chưa phải kết quả kiểm tra đủ mobile/tablet.
- Wrapper trang có `min-h-[1024px]` cùng dữ liệu chuyển đổi từ `min-h-screen` trong bản xuất. Không biến 1024px thành yêu cầu chiều cao mọi thiết bị.

### 5.2. ĐÃ CÓ — spacing và hình khối

| Token | Giá trị | Vai trò |
|---|---|---|
| `gutter-xs` | 4px | Icon–chữ, khoảng vi mô |
| `gutter-sm` | 8px | Ô giờ, lựa chọn nhỏ, padding badge |
| `gutter-md` | 16px | Nhóm thông tin, cột form, khoảng cách nội dung |
| `gutter-lg` | 24px | Padding card và lề trang |
| `gutter-xl` | 32px | Khoảng giữa khối lớn/cột |
| `section` | 48px | Khoảng section được khai báo; không mặc định mọi section đều dùng |
| `page-margin` | 24px | Token lề trang được khai báo |

Bo góc khai báo: 4, 8, 12, 16, 24 và 9999px. HTML áp dụng 8px cho nút/input/ô giờ, 12px cho thẻ bác sĩ, 16px cho tóm tắt, dạng tròn/viên thuốc cho avatar/badge.

Tài liệu nguồn nói khoảng cách theo bước 8px, có bước nhỏ 4px. HTML vẫn có ngoại lệ như `mt-0.5`, viền 1/2px và kích thước icon riêng; không khẳng định mọi giá trị hình học đều là bội số 8.

### 5.3. ĐÃ CÓ — chuyển động khai báo

Cấu hình có state-change 120ms, surface-enter 200ms, surface-exit 150ms. Nút và lựa chọn có lớp chuyển màu theo state-change. Tài liệu nguồn yêu cầu tôn trọng `prefers-reduced-motion`, nhưng không tìm thấy chuỗi này trong sáu HTML. Chưa kiểm tra CSS được sinh hoặc hiệu ứng lúc chạy; không ghi là đã đáp ứng giảm chuyển động.

## 6. ĐỀ XUẤT BỔ SUNG — chưa áp dụng lên project

| Ưu tiên rà soát | Đề xuất | Lý do / phần đang thiếu |
|---|---|---|
| Form | Bổ sung ví dụ lỗi trường, thông báo liên kết với trường và trạng thái gửi đang xử lý | Đã có palette lỗi, chưa thấy bộ minh họa validation/loading hoàn chỉnh |
| Lựa chọn | Kiểm tra focus, thao tác phím và trạng thái được chọn của card/ngày/giờ | Có role/tabindex/lớp trạng thái ở một số chỗ, chưa thử end-to-end bằng bàn phím |
| Trạng thái trước gửi | Cân nhắc nhãn “Trạng thái sau khi gửi: Chờ xác nhận” ở tóm tắt | Hiện badge “Chờ xác nhận” xuất hiện cả trước khi gửi, có thể bị hiểu là đã tạo yêu cầu; cần thử với người dùng |
| Màu và chữ | Đo tương phản trên cặp thực dùng, gồm opacity, trạng thái và chữ nhỏ | Không dùng tuyên bố trong tài liệu gốc thay cho kết quả kiểm tra |
| Responsive | Kiểm tra bảng nhân viên, tên dài và tóm tắt trên chiều rộng nhỏ | Có lớp responsive nhưng chưa chứng minh không tràn/cụt |
| Motion | Rà cách giảm chuyển động ở bản chạy nếu giữ yêu cầu đó | Nguồn tuyên bố nhưng chưa tìm thấy bằng chứng HTML đủ rõ |
| Thư viện | Làm rõ vị trí các file `components/*.html` hoặc cập nhật các tham chiếu | Tài liệu gốc trỏ tới sticker sheet component, nhưng các file này không có trong ZIP đã xuất |
| Prototype | Rà các đường dẫn logic giữa màn hình và cách đóng gói bản xuất | Tên thư mục ZIP khác đường dẫn href nội bộ; không coi bản xuất đã được kiểm thử điều hướng |

Không tự đặt palette, font hoặc spacing mới vào phần “ĐÃ CÓ”. Nếu nhóm chọn một đề xuất, cần cập nhật trạng thái và kiểm tra lại trước khi áp dụng lên Stitch bằng skill khác.

## 7. Nguồn đối chiếu và giới hạn

### 7.1. Tài nguyên đi kèm

Thư mục `assets` giữ nguyên file nguồn xuất từ project. Đây là dữ liệu đầu vào để tái kiểm tra, không phải bản nguồn đã sửa:

| Mã | Nguồn tương đối | Nội dung |
|---|---|---|
| DS0 | [Design System gốc](./assets/an-tâm-healthcare-portal-design-system.md) | Palette, typography, spacing và ý đồ thiết kế khai báo |
| S01 | [Chọn bác sĩ và thời gian](./assets/người-đặt-khám-chọn-bác-sĩ-và-thời-gian/code.html) | Card, ngày/giờ, form, tóm tắt, CTA |
| S02 | [Kết quả gửi yêu cầu](./assets/người-đặt-khám-kết-quả-gửi-yêu-cầu-chờ-xác-nhận/code.html) | Trạng thái chờ và chi tiết yêu cầu mẫu |
| S03 | [Đề nghị thời gian khác](./assets/người-đặt-khám-đề-nghị-thời-gian-khác/code.html) | Bối cảnh reschedule phía người đặt |
| S04 | [Chi tiết yêu cầu nhân viên](./assets/nhân-viên-tiếp-nhận-chi-tiết-yêu-cầu-yc-1046/code.html) | Thông tin và xử lý yêu cầu |
| S05 | [Danh sách yêu cầu](./assets/nhân-viên-tiếp-nhận-danh-sách-yêu-cầu/code.html) | Bộ lọc, bảng, badge, thao tác dòng |
| S06 | [Kết quả xác nhận](./assets/nhân-viên-tiếp-nhận-kết-quả-xác-nhận-lịch/code.html) | Trạng thái đã xác nhận |

Đối chiếu tự động cho thấy đoạn cấu hình `globalThis.tailwind.config` của sáu HTML giống nhau. Điều này xác nhận tính nhất quán của cấu hình trong tập xuất, không chứng minh mọi component dùng đúng token hoặc mọi tương tác hoạt động.

### 7.2. Hồ sơ xuất và phương pháp

- Project: https://stitch.google.com/projects/17731225245642953956.
- ZIP tải về: `C:/Users/ACER/Downloads/stitch_c_ng_t_l_ch_kh_m_agile.zip`.
- SHA256 ZIP: `E6B55434273D3C8DE6E73E8F5B69BEABEE34A97F5DA173F2D4A355F817D798AD`.
- Skill local: `C:/Users/ACER/.codex/skills/design-md/SKILL.md`.
- Tuyến thu thập thay thế: Opera GX → Export ZIP → đọc tài liệu gốc, cấu hình, lớp và nội dung HTML. Chưa lấy project/screen metadata hoặc screen ID qua MCP.
- Đã thử mở hướng dẫn prompting tại https://stitch.withgoogle.com/docs/learn/prompting/ nhưng công cụ đọc web không trích được nội dung. Không tuyên bố đã áp dụng đầy đủ nội dung hướng dẫn chưa đọc được.
- Chưa chạy audit tương phản, responsive, bàn phím, runtime font hoặc kiểm thử tương tác. Các đề xuất không được xem là lỗi đã chứng minh bằng kiểm thử người dùng.
- Chỉ chọn/xuất tài nguyên trên canvas và ghi tài liệu local; không sửa nội dung, theme, màn hình hay logic của project Stitch.
