# Healthcare Portal — Research & Discovery

Cập nhật định hướng: **21/11/2026, Asia/Saigon**.

Healthcare Portal là dự án phát triển sản phẩm hỗ trợ đặt và điều phối lịch khám. Hồ sơ này phục vụ quyết định đầu tư phát triển, xác định nhu cầu, phạm vi sản phẩm và điều kiện vận hành thực tế. Phòng khám tư nhân nhỏ/vừa tại Việt Nam là phân khúc giả thuyết; một cơ sở độc lập là phạm vi đề xuất để nghiên cứu sâu trước khi mở rộng.

## Trạng thái và cách dùng

Đã lập 24 giả định, chuẩn bị kịch bản phỏng vấn và hoàn thành vòng nghiên cứu tài liệu công khai ngày 21/11/2026. Chưa có phỏng vấn, quan sát tác vụ, cơ sở nhận thử hay kiểm chứng kỹ thuật. Chưa phê duyệt MVP. Định hướng làm sản phẩm thực tế là yêu cầu của chủ dự án, không phải bằng chứng rằng khách hàng cần sản phẩm.

Ba câu hỏi cốt lõi là: vấn đề lịch hẹn có đủ quan trọng (VAL-01), cách phối hợp có làm tăng việc cho nhân viên (USE-03), và quy tắc lịch có thể nhất quán (FEA-01). Song song cần làm rõ người quyết định sử dụng/chi trả, chi phí triển khai và hỗ trợ, tiếp cận cơ sở, dữ liệu, nguồn lực và khả năng duy trì sử dụng. Các rủi ro này thuộc phạm vi discovery hiện tại.

## Tài liệu nền

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

Đọc [Research Summary](./outputs/research-summary.md) để xem toàn bộ 10 đầu ra. Các kết quả chính nằm trong [Evidence Log](./outputs/evidence-log.md), [Competitor Analysis](./outputs/competitor-analysis.md), [Research Findings](./outputs/research-findings.md), [Product Vision v2](./outputs/product-vision-v2.md), [Lean Canvas v2](./outputs/lean-canvas-v2.md) và [Discovery Review](./outputs/discovery-review.md).

Các tài liệu nền và đầu ra đã được đồng bộ theo định hướng dự án hiện tại. V2 bổ sung lập luận từ nguồn công khai; tên phiên bản không hàm ý bản nền là một bản lưu trữ bất biến.

## Nguồn và phương pháp

- D1/E01–E09 là dấu vết tài liệu ý tưởng ban đầu được hồ sơ trước ghi nhận. Các nhân vật Tâm An/Bác sĩ Nam và số liệu nhập vai là mô phỏng, không phải người tham gia hoặc dữ liệu thực địa. Vòng cập nhật này không đọc lại tài liệu Word gốc.
- S01–S14 là các nguồn công khai trong Evidence Log, có ngày truy cập và giới hạn riêng. Tài liệu nhà cung cấp chứng minh điều họ công bố, không tự chứng minh hiệu quả thực tế hoặc nhu cầu của phân khúc mục tiêu.
- DA là định hướng dự án; H là giả thuyết; SL là suy luận; CB là nội dung công bố. Đồng thuận nội bộ không thay thế bằng chứng khách hàng.
- Các skills áp dụng: `identify-assumptions-new`, `prioritize-assumptions`, `interview-script`, `competitor-analysis`, `user-personas`, `customer-journey-map`, `product-vision`, `lean-canvas`. Bản local nằm trong `.agents/skills`; tài liệu dự án là đầu ra áp dụng, không phải skill mới.

## Quyết định còn mở

Xác định phân khúc cụ thể, cơ sở tiếp cận, người quyết định sản phẩm và người rà soát nghiệp vụ; thu thập hiện trạng, baseline, điều kiện thay đổi công cụ, ngân sách và nguồn lực. Chưa mặc định mô hình SaaS, thuê bao hoặc mức giá. Trước thử nghiệm vận hành cần thống nhất quy trình, trách nhiệm hỗ trợ, điều kiện sử dụng dữ liệu và cách xử lý sự cố. Các quyết định này phải gắn với bằng chứng và người chịu trách nhiệm.
