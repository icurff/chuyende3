# Healthcare Portal — Ưu tiên giả định

Cập nhật 21/11/2026. Áp dụng `prioritize-assumptions` cho [24 giả định](./01-assumptions.md). Đây là đánh giá định tính và kế hoạch nghiên cứu, chưa phải kết quả kiểm chứng hoặc phê duyệt MVP.

## 1. Mục tiêu

Ưu tiên bằng chứng cần cho quyết định phát triển và vận hành Healthcare Portal. VAL-01 → USE-03 → FEA-01 là chuỗi khám phá cốt lõi: vấn đề → công việc hiện tại → tính nhất quán của quy tắc. Đồng thời phải làm rõ phân khúc, người quyết định dùng/chi trả, chi phí vận hành, dữ liệu, tiếp cận khách hàng và nguồn lực.

## 2. Cách đánh giá

Impact là hệ quả nếu giả định sai đối với giá trị người dùng, vận hành và quyết định đầu tư. Confidence phản ánh chất lượng bằng chứng; Effort cam kết là công sức làm và sửa lại sản phẩm/quy trình nếu tiếp tục dựa trên giả định sai. Risk được cân nhắc theo `(1 − Confidence) × Effort`, chỉ dùng mức định tính vì chưa có dữ liệu để tính điểm. Công sức kiểm chứng được xem riêng.

Mức cao cần nghiên cứu sớm hoặc xử lý trước cam kết phụ thuộc. Mức trung bình cần theo dõi trong phạm vi liên quan. Mức thấp chỉ áp dụng cho cam kết hiện chưa được chọn; không đồng nghĩa rủi ro đó nhỏ khi đưa vào sản phẩm.

## 3. Ma trận 24 giả định

| Mã | Nội dung rút gọn | Impact | Confidence | Effort cam kết | Risk | Hành động |
|---|---|---|---|---|---|---|
| VAL-01 | Lịch hẹn là vấn đề đủ quan trọng | Cao | Thấp | Cao | Cao | Ưu tiên nghiệp vụ 1: sự việc, hậu quả và hành vi thay đổi |
| VAL-02 | Pain points nhập vai phản ánh thực tế | Trung bình | Thấp | Trung bình | Trung bình | Hỏi mở về ưu tiên; chưa cam kết phân hệ kê đơn/kho |
| VAL-03 | Nhắc lịch thay đổi hành vi | Trung bình | Thấp | Trung bình | Trung bình | Tìm nguyên nhân no-show trước quyết định nhắc hẹn |
| USE-01 | Người đặt tự hoàn thành tác vụ | Cao | Thấp | Cao | Cao | Quan sát cách đặt và thử tác vụ khi có prototype |
| USE-02 | Một màn hình/phím tắt giúp bác sĩ | Thấp | Thấp | Thấp | Thấp | Chưa thuộc phạm vi kê đơn; đánh giá lại nếu mở rộng |
| USE-03 | Quy trình chung không tăng việc | Cao | Thấp | Cao | Cao | Ưu tiên nghiệp vụ 2: bảng tác vụ và công việc duy trì song song |
| VIA-01 | Người quyết định và ngân sách phù hợp | Cao | Thấp | Cao | Cao | Nghiên cứu quyết định sử dụng/chi trả và nguồn tài chính ngay |
| VIA-02 | Chuyển đổi, vận hành, hỗ trợ khả thi | Cao | Thấp | Cao | Cao | Ước lượng chi phí tiếp nhận, bảo trì và hỗ trợ cùng discovery |
| VIA-03 | Phù hợp ràng buộc dữ liệu/nghiệp vụ | Cao | Thấp | Cao | Cao | Xác định điều kiện áp dụng; rà soát trước pilot thực tế |
| FEA-01 | Quy tắc lịch và ngoại lệ nhất quán | Cao | Trung bình | Cao | Cao | Ưu tiên nghiệp vụ 3; mức tin tưởng chỉ phản ánh nhận diện quy tắc |
| FEA-02 | Tích hợp có điều kiện sử dụng phù hợp | Trung bình | Thấp | Trung bình | Trung bình | Xác định phụ thuộc cần thiết; kiểm tra trước cam kết dịch vụ |
| FEA-03 | Dữ liệu có thể chuẩn hóa và liên kết | Trung bình | Thấp | Trung bình | Trung bình | Làm rõ nhu cầu nhập dữ liệu; đánh giá trước migration nếu chọn |
| ETH-01 | Nghiên cứu với dữ liệu tối thiểu | Cao | Thấp | Cao | Cao | Chuẩn bị quy trình đồng ý, truy cập và lưu giữ trước thu thập |
| ETH-02 | Hiểu giới hạn AI/kê đơn | Thấp | Thấp | Thấp | Thấp | Chưa thuộc phạm vi; đánh giá lại trước mở rộng |
| ETH-03 | Người cần hỗ trợ vẫn được phục vụ | Cao | Thấp | Trung bình | Cao | Nghiên cứu đặt hộ, hỗ trợ và khách trực tiếp |
| GTM-01 | Tiếp cận được đúng người | Cao | Thấp | Cao | Cao | Tìm cơ sở và người tham gia; không coi nguồn web là cam kết |
| GTM-02 | Có lợi ích đủ để thử và tiếp tục dùng | Cao | Thấp | Cao | Cao | Hỏi lịch sử đổi công cụ, điều kiện thử; theo dõi dùng lại khi pilot |
| GTM-03 | Phân khúc và kênh phù hợp | Cao | Thấp | Cao | Cao | Thu hẹp tiêu chí, kiểm tra kênh tiếp cận quản lý/cơ sở |
| STR-01 | Thống nhất vấn đề và kết quả | Cao | Thấp | Trung bình | Cao | Ghi quyết định, bằng chứng và người chịu trách nhiệm |
| STR-02 | Có nhu cầu chưa được đáp ứng | Cao | Thấp | Cao | Cao | So giải pháp hiện tại và lý do chọn/không chọn của khách hàng |
| STR-03 | Có thước đo gắn với vấn đề | Cao | Thấp | Trung bình | Cao | Thu baseline, định nghĩa kết quả và cách đo |
| TEAM-01 | Năng lực/thời gian đủ | Cao | Thấp | Cao | Cao | Xác định năng lực, thời lượng và ngân sách trước chốt phạm vi |
| TEAM-02 | Có chủ quyết định và người rà nghiệp vụ | Cao | Thấp | Trung bình | Cao | Phân công trách nhiệm sản phẩm, nghiệp vụ và vận hành |
| TEAM-03 | Dùng skill có truy vết và kiểm tra | Trung bình | Thấp | Trung bình | Trung bình | Rà nguồn và lập luận, không coi đầu ra agent là đã duyệt |

Đánh giá mức cao phản ánh hậu quả của quyết định sai cùng độ thiếu bằng chứng, không phải điểm số được đo. Confidence giữ thận trọng; định hướng của chủ dự án không xác thực giả định về khách hàng hoặc năng lực đội ngũ.

## 4. Phối hợp kiểm chứng

Ba kế hoạch chi tiết bên dưới tập trung nghiệp vụ. Các luồng tài chính, vận hành, tiếp cận và nguồn lực có đầu ra riêng trong [Research Plan](./05-research-plan.md). Không coi hoàn thành ba giả định là đủ điều kiện phát hành sản phẩm. Trạng thái sau desk research xem [Discovery Review](./outputs/discovery-review.md).

## 5. Kế hoạch kiểm chứng ưu tiên 1 — VAL-01

### Câu hỏi và quyết định cần hỗ trợ

Vướng mắc nào trong đặt/xác nhận/đổi/hủy lịch ảnh hưởng đáng kể tới người đặt và cơ sở mục tiêu? Bằng chứng có đủ để ưu tiên giải quyết vấn đề này và đầu tư kiểm tra giải pháp, hay mới chỉ phản ánh ý tưởng nội bộ?

### Phương pháp đề xuất

1. Chọn rõ một bối cảnh nghiên cứu; ghi vì sao nguồn tìm được có liên quan. Không mặc định chính sách bệnh viện lớn áp dụng cho phòng khám nhỏ.
2. Desk research các hướng dẫn, chính sách hoặc mô tả vận hành có nguồn trực tiếp. Phân biệt nguồn chỉ nói “có chức năng” với nguồn mô tả khó khăn và hậu quả cụ thể. Lời quảng cáo giải pháp không tự chứng minh mức độ nghiêm trọng của vấn đề.
3. Nếu có người thật tự nguyện tham gia, hỏi về lần gần nhất đã đặt/đổi lịch hoặc xử lý lịch; ghi hành động, công cụ, bước làm lại và hậu quả. Chưa tự liên hệ hoặc gửi tin thay nhóm.

**Công sức kiểm chứng:** có thể bắt đầu bằng đọc và ghi nguồn; phần xác nhận nhu cầu và thay đổi hành vi cần bằng chứng trực tiếp phù hợp, chưa biết có tiếp cận được hay không. Không ước lượng giờ/chi phí khi chưa có lịch nhóm.

### Bằng chứng cần thu thập

- URL/file, chủ thể, ngày truy cập và đoạn nguồn; bối cảnh, người thực hiện và sự việc mà nguồn thực sự mô tả.
- Chuỗi sự việc: nhu cầu → cách làm → vướng mắc → tác động → cách khắc phục hiện tại, nếu có căn cứ.
- Nếu có ghi chép người thật: tách lời kể với điều quan sát được; ghi cả trường hợp không gặp khó khăn và lý do giữ công cụ cũ. Không thu hồ sơ bệnh nhân để chứng minh tình huống.
- Dấu hiệu người dùng đã tìm cách thay đổi công cụ/quy trình, nếu có. Không suy ra sẵn sàng đổi từ việc họ nói “ý tưởng hay”.

### Chỉ dấu và tiêu chí ra quyết định — ĐỀ XUẤT CHƯA KIỂM CHỨNG

Đánh giá định tính chất lượng chuỗi bằng chứng, độ phù hợp bối cảnh và việc có hành vi cụ thể; chưa đặt tỷ lệ, tần suất tối thiểu hay điểm hài lòng.

- **Có hỗ trợ một phần:** nguồn truy được mô tả khó khăn và hậu quả trong bối cảnh phù hợp. Có thể sửa vấn đề trong Vision/Canvas thành giả thuyết có căn cứ; chưa xác nhận động lực đổi công cụ hoặc mức độ phổ biến nếu thiếu dữ liệu trực tiếp.
- **Có hỗ trợ trực tiếp trong bối cảnh được nghiên cứu:** có lời kể/quan sát đáng tin về sự việc cùng cách người dùng tìm giải pháp hoặc chịu đánh đổi. Chỉ nâng mức tin tưởng cho phần nội dung thực sự được chứng minh, không khái quát thị trường hoặc khẳng định sẽ chuyển sang sản phẩm của nhóm.
- **Cần điều chỉnh:** khó khăn khác với phát biểu ban đầu, hoặc đối tượng/công cụ không khớp. Sửa lại giả định và vấn đề nghiên cứu.
- **Chưa đủ bằng chứng:** chỉ tìm thấy mô tả tính năng, quảng cáo hoặc AI mô phỏng. Giữ trạng thái chưa xác thực; tiếp tục tìm bằng chứng hoặc thu hẹp vấn đề trước khi cam kết xây dựng; không trình bày như nhu cầu đã xác nhận.
- **Có bằng chứng phản bác trong bối cảnh:** cách làm hiện tại đáp ứng tốt và không thấy ảnh hưởng được giả định. Ghi giới hạn và xem xét hẹp lại vấn đề; không kết luận mọi phòng khám đều không có nhu cầu.

## 6. Kế hoạch kiểm chứng ưu tiên 2 — USE-03

### Câu hỏi và quyết định cần hỗ trợ

Nhân viên đang phối hợp các nguồn lịch như thế nào? Cách làm tập trung dự kiến có bỏ bớt hay thêm thao tác, trách nhiệm và nguồn cần đối chiếu?

### Phương pháp đề xuất

1. Từ nguồn công khai phù hợp, mô tả luồng hiện tại kèm nguồn cho từng bước. Nếu nguồn chưa rõ, ghi “chưa biết”; không tự điền bằng AI rồi gọi là hiện trạng.
2. Lập bảng tác vụ cho các tình huống nhận lịch, đổi lịch, khách trực tiếp và bác sĩ đổi ca. Ghi ai làm, nguồn lịch nào được đọc/ghi, bước nào phải chép lại, ai thông báo.
3. Đối chiếu trên giấy với một phương án phối hợp dự kiến để tìm bước thêm, bỏ sót hoặc chưa xác định trách nhiệm. Đây là phân tích quy trình, chưa phải thử khả năng sử dụng và chưa thiết kế giao diện.
4. Nếu có nhân viên vận hành thật, nhờ họ kể lại/đi qua tình huống gần đây và chỉ ra điểm sai trong bảng. Muốn kết luận về khối lượng công việc thực tế cần quan sát hoặc thử trong điều kiện phù hợp ở bước sau.

**Công sức kiểm chứng:** bảng quy trình có thể lập từ desk research; xác nhận “không tăng việc” phụ thuộc nguồn hiện trạng đủ chi tiết và bằng chứng thao tác. Chưa có cơ sở ước lượng thời gian tiết kiệm.

### Bằng chứng cần thu thập

- Bảng `Tình huống | Bước | Người thực hiện | Nguồn đọc/ghi | Nhập lại? | Căn cứ | Điểm chưa rõ`.
- Quy tắc phân công và nguồn lịch được coi là đúng khi dữ liệu khác nhau, nếu có tài liệu hoặc người vận hành xác nhận.
- Những bước đối chiếu, cập nhật hai nơi hoặc liên hệ lại thực sự xuất hiện trong nguồn/quan sát. Số bước chỉ được đếm sau khi có bảng, không đặt sẵn kết quả giảm thao tác.
- Ý kiến người thật, nếu có, phải được phân biệt với việc nhóm tự diễn tập. Nhóm tự đóng vai chỉ phát hiện thiếu sót mô hình, không đại diện lễ tân thực tế.

### Chỉ dấu và tiêu chí ra quyết định — ĐỀ XUẤT CHƯA KIỂM CHỨNG

Chỉ dấu: có/không phải nhập lại, bước chưa xác định người chịu trách nhiệm, nguồn dữ liệu phải duy trì song song và sai lệch giữa mô tả nguồn với mô hình nhóm.

- **Hỗ trợ ở mức mô hình:** nguồn đủ mô tả các bước đang xét và bảng đối chiếu không phát hiện thao tác bắt buộc mới chưa được giải thích. Có thể tiếp tục nghiên cứu hướng phối hợp, chưa kết luận giảm tải thực tế.
- **Cần sửa giả định:** phương án vẫn buộc duy trì nguồn cũ, nhập lại hoặc cần nhân viên thực hiện thêm công việc chưa được tính. Cập nhật hành trình, vai trò và điều kiện áp dụng thay vì tuyên bố “một hệ thống sẽ giảm việc”.
- **Chưa đủ bằng chứng:** nguồn chỉ mô tả phía bệnh nhân hoặc chưa biết khâu nội bộ. Giữ USE-03 chưa xác thực, đánh dấu bước nội bộ là giả thuyết.
- **Chỉ xác nhận hiệu quả sử dụng khi có bằng chứng thao tác phù hợp:** việc nhóm vẽ luồng ngắn hơn không đủ chứng minh lễ tân làm nhanh hơn hoặc ít lỗi hơn. Thiết kế phép đo riêng sau này nếu quyết định cần thử thực tế.

## 7. Kế hoạch kiểm chứng ưu tiên 3 — FEA-01

### Câu hỏi và quyết định cần hỗ trợ

Có thể mô tả quy tắc lịch và ngoại lệ để các thành viên hiểu giống nhau, không nhận lịch vượt giới hạn đã định và không có trạng thái mâu thuẫn không?

### Phương pháp đề xuất

1. Từ nguồn phù hợp, tìm cách xác nhận lịch, ý nghĩa giờ hẹn, xử lý đổi/hủy và khách trực tiếp. Ghi các nguồn dùng chính sách khác nhau, không ghép chúng thành một chính sách “chuẩn”.
2. Lập bộ quy tắc cho cơ sở mục tiêu cùng người vận hành: tách phần có nguồn, phần đã được cơ sở xác nhận và giả thuyết còn mở. Nếu chưa tiếp cận cơ sở, mô hình chỉ dùng để chuẩn bị kiểm chứng, không được coi là chính sách vận hành đã duyệt.
3. Diễn tập tình huống trên giấy, ghi trạng thái trước/sau, tác nhân, điều kiện, công suất và các bên cần biết thay đổi. Không viết code, không tạo prototype hoặc phát sinh lịch khám thật.
4. Kiểm tra chéo: để thành viên khác áp dụng cùng quy tắc vào cùng tình huống, đối chiếu kết quả và giải thích khác biệt.

**Tập tình huống đề xuất, chưa thực hiện:** yêu cầu mới chờ duyệt; hai yêu cầu cạnh tranh cùng công suất; hủy khi còn chờ; đổi khi đã xác nhận; bác sĩ đổi ca; khách trực tiếp khi lịch đã kín; người đặt khác người khám. Giữ chỗ chỉ cần kiểm tra nếu nhóm chọn cơ chế đó; chưa mặc định phải triển khai.

**Công sức kiểm chứng:** rà quy tắc trên giấy phù hợp giai đoạn này; chứng minh tính đúng khi có thao tác đồng thời ở phần mềm cần thử nghiệm kỹ thuật về sau, chưa thuộc kết quả giai đoạn discovery này.

### Bằng chứng cần thu thập

- Bảng quy tắc có nguồn hoặc nhãn “giả thuyết cần cơ sở xác nhận”, phiên bản và người rà soát.
- Với từng tình huống: điều kiện đầu, các sự kiện theo thứ tự, quyết định được phép, trạng thái kết thúc, điểm chưa rõ và nhận xét kiểm tra chéo.
- Danh sách mâu thuẫn/ngoại lệ chưa xử lý; không xóa chúng để làm báo cáo có vẻ hoàn tất.
- Định nghĩa lịch hẹn là giờ tiếp nhận hay giờ khám được cam kết, nếu có thể xác định từ nguồn hoặc quyết định mô phỏng.

### Chỉ dấu và tiêu chí ra quyết định — ĐỀ XUẤT CHƯA KIỂM CHỨNG

Chỉ dấu: tình huống không xác định được kết quả; thành viên đưa ra kết quả khác nhau; trạng thái hoặc công suất mâu thuẫn. Nếu đếm, chỉ báo cáo số thực ghi nhận sau diễn tập, không tự điền số đạt.

- **Đủ nhất quán cho mô hình nghiên cứu đang xét:** toàn bộ tình huống trong tập đề xuất được nhóm giữ lại đều có kết quả giải thích được bằng quy tắc; không còn mâu thuẫn chưa xử lý về công suất/trạng thái; kiểm tra chéo thống nhất. Điều kiện “không còn mâu thuẫn” là tiêu chí đề xuất, chưa có kết quả đo và chưa chứng minh chống trùng lịch bằng code.
- **Cần sửa mô hình:** còn tình huống vượt công suất, không rõ quyền hoặc kết quả tùy người giải thích. Sửa quy tắc/thu hẹp bối cảnh thử nghiệm rồi kiểm tra lại.
- **Chưa đủ căn cứ nghiệp vụ:** quy tắc tự nhất quán nhưng chỉ là lựa chọn nhóm. Ghi “nhất quán trong mô phỏng, chưa xác nhận nghiệp vụ thực tế”, không nâng thành đã xác thực toàn bộ FEA-01.
- **Cần nghiên cứu tiếp:** các nguồn mô tả chính sách khác nhau hoặc không đủ chi tiết. Ghi lựa chọn còn mở; không âm thầm áp dụng cùng quy tắc cho mọi cơ sở.

## 8. Ghi nhận và cập nhật sau kiểm chứng

| Ưu tiên | Mã | Trạng thái hiện tại | Tài liệu có thể cần sửa sau khi có bằng chứng |
|---|---|---|---|
| 1 | VAL-01 | Desk research chưa đủ; chưa có bằng chứng trực tiếp | Vấn đề/giá trị trong Vision và Canvas; nhu cầu của proto-personas |
| 2 | USE-03 | Desk research chưa đủ; chưa quan sát hoặc thử tác vụ | Hành trình và persona điều phối; giới hạn giá trị giảm thao tác |
| 3 | FEA-01 | Có căn cứ nhận diện quy tắc; chưa diễn tập hoặc kiểm chứng kỹ thuật | Ranh giới/quy tắc bối cảnh thử nghiệm; câu hỏi và tình huống nghiên cứu |

Mẫu nhật ký sử dụng sau này:

| Mã | Nguồn/file và vị trí | Điều thực sự quan sát/đọc được | Điều chưa chứng minh | Quyết định/lý do | Người rà soát và ngày |
|---|---|---|---|---|---|
| Chưa điền | Chưa có | Chưa có dữ liệu | Chưa đánh giá | Chưa ra quyết định | Chưa phân công |

Các tiêu chí trên là **đề xuất ra quyết định nghiên cứu, chưa được nhóm duyệt hoặc kiểm chứng**. Nếu chỉ có desk research, có thể hoàn thiện bản nháp có dẫn nguồn, nhưng giữ rõ giới hạn về mức độ nghiêm trọng, động lực thay đổi, khối lượng công việc thực tế và khả thi kỹ thuật.

Không tuyên bố ba giả định đã đúng vì được ưu tiên cao. Chưa phê duyệt MVP, chọn công nghệ hoặc đề xuất triển khai tính năng chỉ từ ma trận này.
