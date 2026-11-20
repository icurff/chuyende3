# Healthcare Portal — Kế hoạch Research & Discovery

Cập nhật 21/11/2026. Mục tiêu: quyết định sản phẩm nào đáng phát triển, cho ai, và dưới điều kiện nào có thể vận hành bền vững. Chưa ấn định nhân sự, thời lượng, ngân sách hoặc ngày triển khai khi chưa có dữ liệu nguồn lực.

## Điểm xuất phát

Đã có [desk research](./outputs/research-summary.md), 24 giả định, ba Proto-personas và kịch bản phỏng vấn. Chưa có bằng chứng trực tiếp từ cơ sở mục tiêu, baseline, khách hàng nhận thử hoặc kiểm chứng kỹ thuật. Không dùng mô phỏng như xác nhận nhu cầu.

## Các luồng nghiên cứu

| Luồng | Việc cần thực hiện | Bằng chứng và quyết định |
|---|---|---|
| Phân khúc và tiếp cận | Chọn đặc điểm cơ sở, người đặt/người điều phối/người quyết định phù hợp; tìm đầu mối và xin tham gia | Cơ sở tiếp cận được, vai trò, tiêu chí chọn và giới hạn mẫu; GTM-01/03 |
| Giá trị và hiện trạng | Phỏng vấn về lần đặt/đổi/hủy gần nhất, quan sát tác vụ khi có đồng ý; ghi cả điều thuận lợi | Ví dụ có hậu quả, công cụ, cách khắc phục, lý do giữ/đổi công cụ; VAL-01, USE-03 |
| Chính sách và kỹ thuật | Rà quyền xác nhận, công suất, ngoại lệ và bàn giao cùng người vận hành; sau đó diễn tập và thiết kế thử nghiệm kỹ thuật phù hợp | Quy tắc có người xác nhận, mâu thuẫn còn mở, kế hoạch kiểm tra đồng thời; FEA-01 |
| Quyết định sử dụng và tài chính | Hỏi lần lựa chọn công cụ gần nhất, người duyệt, ngân sách thực, điều kiện tiếp nhận và trách nhiệm hỗ trợ | Người quyết định/chi trả, chi phí chuyển đổi, nguồn tài chính; VIA-01/02, GTM-02 |
| Vận hành và dữ liệu | Xác định dữ liệu tối thiểu, quyền truy cập, trách nhiệm lưu giữ, hỗ trợ, xử lý sự cố và phụ thuộc dịch vụ | Điều kiện nghiên cứu/thử nghiệm, câu hỏi cần chuyên môn xác minh; VIA-03, ETH-01/03, FEA-02/03 |
| Đo lường và nguồn lực | Ghi hiện trạng, xác định phép đo và năng lực cần; ước lượng theo phạm vi có căn cứ | Baseline, tiêu chí tiếp tục/điều chỉnh, ngân sách, mốc và người phụ trách; STR-03, TEAM |

Các luồng có thể phối hợp theo khả năng tiếp cận. Thứ tự VAL-01 → USE-03 → FEA-01 phản ánh phụ thuộc nghiệp vụ, không trì hoãn việc tìm hiểu tính bền vững và điều kiện vận hành.

## Phân công theo trách nhiệm

| Trách nhiệm | Đầu ra cần sở hữu | Trạng thái |
|---|---|---|
| Quyết định sản phẩm | Phân khúc, vấn đề, phạm vi và tiêu chí tiếp tục | Chưa phân công |
| Nghiên cứu người dùng | Tuyển người, xin đồng ý, phỏng vấn, quan sát, tổng hợp | Chưa phân công |
| Rà soát nghiệp vụ | Xác nhận chính sách cơ sở và ngoại lệ | Chưa xác định đầu mối |
| Kỹ thuật và vận hành | Kiểm tra khả thi, chi phí, dữ liệu, hỗ trợ và phục hồi | Chưa phân công |
| Kiểm tra bằng chứng | Truy nguồn, phản chứng, tính nhất quán và quyết định | Chưa phân công |

Một người có thể đảm nhiệm nhiều trách nhiệm nếu năng lực và thời lượng phù hợp. Kế hoạch không mặc định số người hoặc cơ cấu tổ chức.

## Thu thập và tổng hợp

Sử dụng [Interview Guide](./03-interview-guide.md). Tách lời kể, quan sát, tài liệu công bố và suy luận. Ghi mã giả định, nguồn/vị trí, ngày, bối cảnh, điều được hỗ trợ, điều chưa chứng minh và quyết định. Không thu bệnh án hoặc thông tin nhận diện ngoài nhu cầu nghiên cứu; xác định người được truy cập và thời hạn lưu trước khi thu thập.

Nếu chưa tiếp cận được người thật, tiếp tục dùng tài liệu công khai và mô hình giả thuyết để chuẩn bị câu hỏi; ghi rõ việc xác thực còn bị giới hạn. Không xem mô hình tự diễn tập là căn cứ sẵn sàng triển khai.

## Điều kiện chuyển bước

1. Trước xác định phạm vi xây dựng: có vấn đề và đối tượng cụ thể, bằng chứng hành vi phù hợp, chính sách sơ bộ được rà soát, rủi ro ưu tiên và người chịu trách nhiệm.
2. Trước thử prototype: xác định tác vụ, người thử, phép đo và dữ liệu thử phù hợp; kết quả phải phân biệt với hiệu quả vận hành thật.
3. Trước pilot tại cơ sở: xác nhận người tiếp nhận, phạm vi, quy trình và hỗ trợ; đánh giá các ràng buộc dữ liệu/nghiệp vụ, tính đúng kỹ thuật, cách xử lý sự cố và tiêu chí dừng/tiếp tục.
4. Trước mở rộng: đánh giá giá trị so với hiện trạng, duy trì sử dụng, chi phí phục vụ và khả năng vận hành lặp lại. Không dùng một phiên thử thành công làm bằng chứng cho toàn thị trường.

Đây là tiêu chí lập kế hoạch, chưa phải hoạt động đã thực hiện hoặc cam kết triển khai. Cập nhật [Discovery Review](./outputs/discovery-review.md) khi có bằng chứng mới.
