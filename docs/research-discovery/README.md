# Healthcare Portal — Research & Discovery

Cập nhật: **21/11/2026, Asia/Saigon**. Bộ tài liệu hiện tại phục vụ nghiên cứu sản phẩm và chuẩn bị Design System & Prototype.

Healthcare Portal là dự án phát triển sản phẩm hỗ trợ đặt và điều phối lịch khám. Hồ sơ này phục vụ quyết định đầu tư phát triển, xác định nhu cầu, phạm vi sản phẩm và điều kiện vận hành thực tế. Phòng khám tư nhân nhỏ/vừa tại Việt Nam là phân khúc giả thuyết; một cơ sở độc lập là phạm vi đề xuất để nghiên cứu sâu trước khi mở rộng.

## Trạng thái và cách dùng

Đã lập 24 giả định, chuẩn bị kịch bản phỏng vấn, nghiên cứu tài liệu công khai và refactor sáu artifact. Chưa có phỏng vấn, quan sát tác vụ, cơ sở nhận thử, prototype đã thử hoặc kiểm chứng kỹ thuật. Định hướng làm sản phẩm thực tế là yêu cầu của chủ dự án, không phải bằng chứng rằng khách hàng cần sản phẩm.

Ba câu hỏi cốt lõi là: vấn đề lịch hẹn có đủ quan trọng (VAL-01), cách phối hợp có làm tăng việc cho nhân viên (USE-03), và quy tắc lịch có thể nhất quán (FEA-01). Song song cần làm rõ người quyết định sử dụng/chi trả, chi phí triển khai và hỗ trợ, tiếp cận cơ sở, dữ liệu, nguồn lực và khả năng duy trì sử dụng. Các rủi ro này thuộc phạm vi discovery hiện tại.

## Tài liệu đầu vào

Bảy file dưới đây giữ nguyên nội dung. Mọi kết quả, nhận xét và cập nhật phát sinh được lưu trong `outputs/`; README cung cấp mục lục và hướng dẫn đọc. Đây là các mốc đầu vào, không phải bản quyết định hiện hành. Khi tầm nhìn, phạm vi hoặc quy tắc có điều chỉnh, dùng bộ `outputs/` để thiết kế và truy về tài liệu đầu vào khi cần xem giả định ban đầu.

| Tài liệu | Mục đích |
|---|---|
| [Giả định](./01-assumptions.md) | 24 giả định trong tám nhóm, căn cứ và cách kiểm chứng |
| [Ưu tiên giả định](./02-prioritized-assumptions.md) | Ma trận rủi ro và kế hoạch thu bằng chứng |
| [Product Vision](./02-product-vision.md) | Tầm nhìn và kết quả sản phẩm kỳ vọng |
| [Lean Canvas](./03-lean-canvas.md) | Mô hình giá trị, phân khúc, chi phí và nguồn tài chính cần kiểm chứng |
| [Interview Guide](./03-interview-guide.md) | Phỏng vấn người đặt, người điều phối và người quyết định |
| [Proto-personas](./04-proto-personas.md) | Vai trò giả thuyết, chưa phải phân khúc đã xác thực |
| [Research Plan](./05-research-plan.md) | Các bước nghiên cứu và điều kiện chuyển sang thử nghiệm |

## Kết quả nghiên cứu

Bộ đầu ra gồm **6 tài liệu Research & Discovery**. Cách trình bày được chọn theo nội dung: đoạn văn để giải thích, sơ đồ và bước đánh số cho hành trình, bảng ngắn để so sánh, gạch đầu dòng cho cách đo và việc cần làm. Mã tham chiếu đặt ở chỗ cần tra cứu. Các tài liệu tập trung vào vấn đề, người dùng, hành trình, giải pháp hiện có và định hướng giá trị; chưa chốt quy tắc nghiệp vụ chi tiết hoặc phạm vi MVP.

| Tài liệu | Nội dung chính |
|---|---|
| [Problem Statement](./outputs/problem-statement.md) | CP-01, SP-01–SP-04; nhu cầu N01–N05; phát hiện R01–R06 và trạng thái 24 giả định |
| [Competitor Analysis](./outputs/competitor-analysis.md) | Giải pháp hiện có, cơ hội định vị và phụ lục nguồn S01–S14 |
| [User Personas](./outputs/user-personas.md) | P01/P02/P03 cùng cấu trúc goals, JTBD, hành vi giả thuyết, nhu cầu và tình huống UX |
| [Customer Journey Map](./outputs/customer-journey-map.md) | Reference Journey, hiện trạng giả định HJ, mức chưa có Validated As-Is và luồng prototype TJ |
| [Product Vision v2](./outputs/product-vision-v2.md) | Tầm nhìn, giá trị kỳ vọng và ranh giới sản phẩm |
| [Lean Canvas v2](./outputs/lean-canvas-v2.md) | Hướng giải pháp SH-01–SH-04; mô hình kinh doanh giả thuyết, chi phí và phép đo |

Kết quả desk research giúp làm rõ câu hỏi nghiên cứu; VAL-01 và USE-03 còn thiếu bằng chứng trực tiếp, FEA-01 mới được hỗ trợ ở việc nhận diện quy tắc. Trạng thái 24 giả định nằm tại [phụ lục Problem Statement](./outputs/problem-statement.md#trang-thai-gia-dinh). Journey minh họa một phương án để khám phá prototype; cần xác nhận quy trình và điều kiện sử dụng trước khi chốt thiết kế chi tiết. Phép đo đề xuất ở Lean Canvas; kế hoạch nghiên cứu ban đầu ở [Research Plan](./05-research-plan.md).

## Những điểm đã sửa qua review

| Nhóm vấn đề | Điều chỉnh thực chất |
|---|---|
| Clarity — diễn giải còn trừu tượng | Một core problem, bốn tình huống hỗ trợ; Vision, giá trị đề xuất và tính năng được phân biệt |
| Evidence — dễ lẫn công bố và thực tế | Dùng năm loại phát biểu: Evidence-backed, Inference, Hypothesis, Proposed Decision, Unknown; giữ nguồn và giới hạn riêng |
| Completeness — thiếu bối cảnh và tình huống | Bổ sung tình huống đặt, đổi/hủy, ca nghỉ, khách trực tiếp và đặt hộ; ghi rõ những điểm còn cần nghiên cứu |
| Consistency — chưa nối được nhu cầu và hướng giải pháp | Dùng chung mã CP/SP/N/SH/P/HJ/TJ; nối nhu cầu trong Problem Statement với Personas, Journey và Canvas |

Luồng prototype trong Journey là phương án đề xuất cần kiểm chứng. Review do cùng agent thực hiện dưới góc nhìn sản phẩm, nghiệp vụ và UX; chưa có review độc lập hoặc thử với người dùng thật.

## Nguồn và phương pháp

- D1/E01–E09 là dấu vết tài liệu ý tưởng ban đầu được hồ sơ trước ghi nhận. Các nhân vật Tâm An/Bác sĩ Nam và số liệu nhập vai là mô phỏng, không phải người tham gia hoặc dữ liệu thực địa. Vòng cập nhật này không đọc lại tài liệu Word gốc.
- S01–S14 là các nguồn công khai trong [phụ lục phân tích đối thủ](./outputs/competitor-analysis.md#phu-luc-nguon), có ngày truy cập và giới hạn riêng. Tài liệu nhà cung cấp chứng minh điều họ công bố, không tự chứng minh hiệu quả thực tế hoặc nhu cầu của phân khúc mục tiêu.
- Mã tham chiếu tài liệu nền: D01 = README; D02 = Assumptions; D03 = Prioritized Assumptions; D04 = Product Vision; D05 = Lean Canvas; D06 = Proto-personas; D07 = Interview Guide; D08 = Research Plan.
- Nhãn cũ: DA là định hướng dự án; H là giả thuyết; SL là suy luận; CB là nội dung công bố; CX là chưa xác định. Bảng phân loại mới được giải thích tại Problem Statement. Đồng thuận nội bộ không thay thế bằng chứng khách hàng.
- Các skills áp dụng: `identify-assumptions-new`, `prioritize-assumptions`, `interview-script`, `competitor-analysis`, `user-personas`, `customer-journey-map`, `product-vision`, `lean-canvas`. Bản local nằm trong `.agents/skills`; tài liệu dự án là đầu ra áp dụng, không phải skill mới.

## Quyết định còn mở

Xác định phân khúc cụ thể, cơ sở tiếp cận, người quyết định sản phẩm/nghiệp vụ; thu hiện trạng, số đo ban đầu, điều kiện đổi công cụ, ngân sách và nguồn lực. Canvas đề xuất nghiên cứu gói dịch vụ định kỳ theo cơ sở và so với phương án cấp ngân sách nội bộ; chưa chọn mô hình hoặc mức giá. Trước dùng thật cần xác nhận quy trình, dữ liệu, xác thực, tích hợp và trách nhiệm hỗ trợ/phục hồi. Các điểm còn thiếu được nêu trong Problem Statement và từng artifact liên quan; chưa có người nhận trách nhiệm thực tế.


## Tra cứu các tên đầu ra trước khi gộp

Một số tài liệu đầu vào được giữ nguyên còn có liên kết tới các tên file đã gộp. Các đường dẫn lịch sử đó không còn là file hiện hành; dùng bảng tra cứu dưới đây. Liên kết trong README và bộ `outputs/` trỏ trực tiếp tới nội dung hiện tại.

| Tên trước đây | Nơi lưu nội dung hiện tại |
|---|---|
| `evidence-log.md` | [Phụ lục nguồn của Competitor Analysis](./outputs/competitor-analysis.md#phu-luc-nguon) |
| `research-findings.md` | [Problem Statement](./outputs/problem-statement.md), phần phát hiện và kiểm chứng |
| `discovery-review.md` | [Trạng thái 24 giả định](./outputs/problem-statement.md#trang-thai-gia-dinh) và các câu hỏi nghiên cứu còn mở trong [Problem Statement](./outputs/problem-statement.md) |
| `research-summary.md` | Mục lục và tóm tắt trong README này; kết quả nghiên cứu tại [Problem Statement](./outputs/problem-statement.md) |
