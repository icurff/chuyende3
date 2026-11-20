# Healthcare Portal — Giả định nghiên cứu sản phẩm

Ngày lập: 17/11/2026. Cập nhật định hướng: 21/11/2026. Trạng thái: giả định cần kiểm chứng, chưa phê duyệt MVP.

## 1. Mục tiêu và phương pháp

Phát triển sản phẩm hỗ trợ đặt và điều phối lịch khám trong vận hành thực tế. Phân khúc phòng khám tư nhân nhỏ/vừa và phạm vi một cơ sở độc lập là đề xuất cần nghiên cứu. Quy mô đội ngũ, thời lượng, ngân sách và người sở hữu từng quyết định chưa được xác định trong kế hoạch hiện tại.

Áp dụng `identify-assumptions-new` từ `.agents/skills`, phân tích tám nhóm rủi ro qua góc nhìn Product Manager, Designer và Engineer của cùng một agent. Mỗi giả định có căn cứ, mức tin tưởng, hậu quả nếu sai và cách kiểm chứng. Dùng [ma trận ưu tiên](./02-prioritized-assumptions.md) để chọn hành động, không coi mã giả định là thứ tự triển khai.

## 2. Nguồn và giới hạn

D1 là tài liệu ý tưởng ban đầu được hồ sơ trước phân tích. E01–E09 và ký hiệu `§` giữ dấu vết các đoạn trong bản Word đó; vòng cập nhật hiện tại không đọc lại Word hoặc xác nhận độc lập các trích dẫn. Nhãn NHOM là đề xuất nội bộ; AI là nhập vai; CHUA-RO là chưa có nguồn xác minh; SUY-LUAN là diễn giải của agent. Các nhãn này không phải dữ liệu khách hàng. Tâm An/Bác sĩ Nam là nhân vật mô phỏng.

| Mã | Vị trí và nội dung đã ghi trong hồ sơ | Phân loại và cách sử dụng |
|---|---|---|
| E01 | D1 §003–044, “Tổng quan thị trường”, “Phân tích các đối thủ”: hướng lịch hẹn, BookingCare, Medpro, YouMed | NHOM + CHUA-RO đối với khẳng định bên ngoài. Chưa kèm nguồn trực tiếp cho từng tính năng, thời điểm hoặc phân khúc so sánh |
| E02 | D1 §049–085, SWOT, khả thi và MVP ban đầu | NHOM. Nhóm tự ghi thiếu nghiệp vụ, chưa có dữ liệu người dùng thực tế và đề xuất phạm vi lịch hẹn |
| E03 | D1 §087–118, phương pháp, persona giả định, “Raw Data từ AI Role-play” | AI. không xem Tâm An/Bác sĩ Nam là người tham gia nghiên cứu thật |
| E04 | D1 §119–156, sáu pain points và feature mapping | NHOM + AI. Phần tổng hợp gọi là “khảo sát thực tế” tại §120 nhưng chưa có dữ liệu thật kèm theo; nguồn trước đó là nhập vai |
| E05 | D1 §158–198, bảng câu hỏi phân nhánh | NHOM. Là công cụ khảo sát dự kiến, không phải kết quả trả lời; thời gian hoàn thành 3–4 phút chưa có dữ liệu đo kèm theo |
| E06 | D1 §201–595, mục tiêu nghiệp vụ, actors, quy trình và BPMN | NHOM. Quy trình và business rules là mô hình đề xuất; chưa phải quy trình đã được một phòng khám xác nhận |
| E07 | D1 §596–754, entities, KPI, giả định, MVP và kế hoạch xác thực | NHOM. KPI là chỉ số được đề xuất, chưa có baseline hoặc kết quả đo; checklist không chứng minh các việc đã hoàn thành |
| E08 | D1 §788–853, các phân hệ Patient, Front Desk, EMR, Lab, Pharmacy, Admin, Telemedicine | NHOM. Các nhãn Must-have/Nice-to-have là phân loại trong Word, chưa phải ưu tiên đã kiểm chứng |
| E09 | D1 §855–884, Technical Discovery | NHOM + CHUA-RO. Đề xuất công nghệ/tích hợp; năng lực thực tế, chi phí và mức tiết kiệm chưa có dữ liệu xác nhận |


Kết quả tra cứu nguồn công khai mới nằm trong [Evidence Log](./outputs/evidence-log.md) và [Discovery Review](./outputs/discovery-review.md). Không dùng ngân sách, lượt khám, thời gian thao tác hoặc mức tiết kiệm từ nhập vai làm dữ liệu lập kế hoạch.

## 3. Phạm vi và vai trò cần nghiên cứu

Hướng trọng tâm là người đặt khám và người điều phối cùng hiểu được lịch, bước tiếp theo và trách nhiệm khi có thay đổi. Cần xác định người khám có khác người đặt không; bác sĩ có thao tác trực tiếp không; ai quyết định sử dụng, ai chi trả và ai chịu trách nhiệm dữ liệu.

Kê đơn, kho thuốc, bệnh án, AI, thanh toán và đa chi nhánh là các hướng mở rộng chưa được đưa vào phạm vi. Việc giữ chúng ngoài trọng tâm dựa trên nhu cầu ưu tiên và độ phức tạp chưa được làm rõ. Các giả định về tính bền vững, chi phí vận hành, tiếp cận khách hàng và duy trì sử dụng phải được nghiên cứu ngay cùng vấn đề lịch hẹn.

## 4. Cách đọc mức tin tưởng

Thấp: chưa có bằng chứng trực tiếp phù hợp. Trung bình: có căn cứ cho một phần, chưa xác thực toàn bộ. Cao: cần bằng chứng trực tiếp có thể truy vết; hiện chưa gán mức này cho giả định nào. Đây là đánh giá định tính, không phải xác suất. Kế hoạch kiểm chứng bên dưới chưa được thực hiện; kết quả desk research không tự nâng mức tin tưởng thành xác thực nhu cầu.

## 5. Danh sách giả định theo tám nhóm rủi ro

### 5.1. Value — Giá trị đối với người dùng

#### VAL-01 — Vấn đề lịch hẹn đủ quan trọng để người dùng thay đổi cách làm

- **Giả định:** sai sót, trao đổi nhiều lần hoặc khó tổng hợp lịch gây ảnh hưởng đáng kể cho phòng khám mục tiêu và bệnh nhân.
- **Căn cứ:** E01 §004, §044; E06 §205–212; NHOM. Mức độ và tần suất thực tế CHUA-RO.
- **Tin tưởng: Thấp.** Có mô tả vấn đề nhưng chưa có nhật ký, ví dụ từ người thật hoặc đối chiếu với vấn đề vận hành khác.
- **Nếu sai:** nhóm đầu tư vào một luồng ít giá trị; người dùng tiếp tục điện thoại, Zalo, sổ hoặc phần mềm cũ.
- **Kiểm chứng đề xuất:** hỏi lễ tân/quản lý và người đi khám về lần đặt/đổi lịch gần nhất; ghi công cụ, bước làm lại, hậu quả và trường hợp không có khó khăn. Xin xem mẫu lịch đã loại thông tin nhận diện khi phù hợp. Bằng chứng cần là tình huống cụ thể, không chỉ lời đồng ý với ý tưởng.

#### VAL-02 — Các pain points từ nhập vai phản ánh ưu tiên của phòng khám thật

- **Giả định:** nhập liệu lặp, kho thuốc và tra cứu hồ sơ là những vấn đề ưu tiên của phân khúc định chọn.
- **Căn cứ:** E03 §109–118, E04 §125–156; AI + NHOM. Mô hình Tâm An là mô phỏng; mục này chỉ tham khảo nếu nhóm quay lại hướng vận hành nội bộ.
- **Tin tưởng: Thấp.** Danh sách có thể giúp đặt câu hỏi nhưng chưa có phản hồi thực địa.
- **Nếu sai:** phạm vi chuyển sang EMR/kho/thu ngân theo một tình huống không đại diện; lệch nhu cầu thực tế.
- **Kiểm chứng đề xuất:** hỏi mở về việc khó nhất trong ca làm trước khi đưa danh sách pain points; tìm ví dụ gần đây, cách xử lý, ảnh hưởng và vấn đề được người dùng tự ưu tiên. Ghi cả phát hiện trái với nhập vai.

#### VAL-03 — Nhắc lịch sẽ thay đổi hành vi đến khám

- **Giả định:** quên lịch là một nguyên nhân đáng kể của no-show và nhắc lịch có thể cải thiện việc đến khám hoặc báo hủy sớm.
- **Căn cứ:** E06 §361–369, E07 §651–653, E09 §876–878; NHOM. Quan hệ nguyên nhân là SUY-LUAN cần kiểm chứng.
- **Tin tưởng: Thấp.** Chưa có số liệu no-show, lý do bỏ hẹn hoặc dữ liệu về nhắc lịch đang dùng.
- **Nếu sai:** nhóm tối ưu thông báo nhưng không giải quyết nguyên nhân chính như đổi kế hoạch, chờ lâu hoặc khó di chuyển.
- **Kiểm chứng đề xuất:** tìm hiểu các trường hợp bỏ/đổi hẹn đã xảy ra; xem dữ liệu lịch ẩn danh nếu có và cách tính no-show. Chỉ đề xuất thử nhắc lịch có kiểm soát sau khi xác định nguyên nhân; thống nhất baseline và tiêu chí đánh giá trước khi thử.

### 5.2. Usability — Khả năng sử dụng

#### USE-01 — Bệnh nhân có thể tự hoàn thành luồng đặt khám

- **Giả định:** người dùng mục tiêu có thiết bị, kỹ năng và mức sẵn sàng phù hợp để chọn dịch vụ/bác sĩ, cung cấp thông tin, xác thực và quản lý lịch.
- **Căn cứ:** E06 §247–338; E08 §789–799; NHOM. Khả năng sử dụng thực tế là SUY-LUAN.
- **Tin tưởng: Thấp.** Word mô tả luồng hệ thống, chưa có quan sát người dùng; chưa xác định rõ nhóm đặt hộ.
- **Nếu sai:** bệnh nhân cần gọi nhân viên hỗ trợ, bỏ dở hoặc nhập nhầm người được khám.
- **Kiểm chứng đề xuất:** quan sát cách người tham gia từng đặt khám bằng kênh hiện tại; làm rõ ai thao tác và ai đi khám, khó khăn xác thực và chọn chuyên khoa. Thử tác vụ với mẫu minh họa ở giai đoạn sau nếu cần; vòng nghiên cứu này chưa thiết kế prototype.

#### USE-02 — Một màn hình và phím tắt thực sự làm công việc của bác sĩ dễ hơn

- **Giả định:** gom thao tác và dùng mẫu kê đơn phù hợp với cách làm của bác sĩ mục tiêu, không tăng nhầm lẫn hoặc khó học.
- **Căn cứ:** E03 §101–117, E04 §152, E08 §817; AI + NHOM. “Dưới 30 giây” là kỳ vọng, chưa là kết quả.
- **Tin tưởng: Thấp.** Thiết kế được suy ra từ nhập vai; chưa quan sát bác sĩ thật, không được khái quát khả năng sử dụng chỉ theo tuổi.
- **Nếu sai:** màn hình quá tải, thao tác nhanh hơn nhưng sai hơn hoặc không được nhân viên chấp nhận.
- **Kiểm chứng đề xuất:** tìm hiểu cách bác sĩ đang ghi nhận một lượt khám và những bước thường phải sửa; ghi thao tác/công cụ với dữ liệu mô phỏng. Nếu sau này thử phương án, đánh giá cả lỗi và hiểu đúng nội dung, không chỉ thời gian.

#### USE-03 — Quy trình dùng chung không làm tăng việc cho lễ tân

- **Giả định:** có thể phối hợp lịch web, điện thoại và khách trực tiếp trong một quy trình mà nhân viên theo được trong giờ đông.
- **Căn cứ:** E06 §339–392, E08 §801–808; NHOM. Khả năng áp dụng khi làm việc đồng thời là SUY-LUAN.
- **Tin tưởng: Thấp.** Chưa có sơ đồ hiện trạng hoặc quan sát ca làm thực tế.
- **Nếu sai:** xuất hiện sổ phụ, nhập liệu hai lần, cập nhật chậm và bỏ sót lịch.
- **Kiểm chứng đề xuất:** nhờ lễ tân kể lại một ca có nhiều kênh tiếp nhận, mô tả ai cập nhật nguồn lịch nào và lúc nào. Thu thập các ngoại lệ đến muộn, bác sĩ đổi ca, lịch chưa duyệt; nhận diện bước tăng việc thay vì chỉ hỏi họ có thích hệ thống không.

### 5.3. Viability — Khả năng duy trì và phù hợp kinh doanh

#### VIA-01 — Có người quyết định mua và ngân sách thực tế cho vấn đề đã chọn

- **Giả định:** người có quyền quyết định ở phòng khám sẵn sàng dành ngân sách cho giải pháp, ở mức đủ duy trì việc cung cấp.
- **Căn cứ:** E03 §118; E05 §197; AI + NHOM. Các mức giá trong nhập vai và lựa chọn bảng hỏi chưa là bằng chứng sẵn sàng trả tiền.
- **Tin tưởng: Thấp.** Chưa có trao đổi với người duyệt chi, chi tiêu hiện tại hay hành vi mua trước đó.
- **Nếu sai:** mô hình trả phí không phù hợp; nhóm nhầm lời khen hoặc câu trả lời khảo sát với quyết định mua.
- **Kiểm chứng đề xuất:** tìm hiểu ai duyệt mua, quy trình mua phần mềm gần nhất, khoản chi đang có và điều kiện đổi công cụ. Xác định người chịu chi phí, nguồn ngân sách và điều kiện duy trì sản phẩm; không chốt giá từ khoảng tiền mô phỏng.

#### VIA-02 — Chi phí chuyển đổi, vận hành và hỗ trợ nằm trong khả năng cung cấp

- **Giả định:** nhóm hoặc đơn vị cung cấp có thể chuẩn hóa dữ liệu cũ, hướng dẫn sử dụng, duy trì dịch vụ và hỗ trợ với nguồn lực phù hợp.
- **Căn cứ:** E03 §114, E04 §155, E09 §869–881; AI + NHOM; chi phí tổng là CHUA-RO.
- **Tin tưởng: Thấp.** Chưa có dữ liệu mẫu, khối lượng công việc hoặc bảng chi phí dịch vụ và nhân công.
- **Nếu sai:** gói trọn gói không đủ bù công sức; sản phẩm không thể được bàn giao, vận hành hoặc hỗ trợ bền vững.
- **Kiểm chứng đề xuất:** xin cấu trúc file mẫu đã làm sạch, liệt kê công việc chuyển đổi và hỗ trợ; ước lượng dựa trên dữ liệu kiểm tra được. Khi chọn dịch vụ, tra điều kiện/giá chính thức tại thời điểm đánh giá; không dùng tên dịch vụ trong Word làm bằng chứng chi phí thấp.

#### VIA-03 — Có thể đáp ứng các ràng buộc dữ liệu và nghiệp vụ trong bối cảnh sử dụng dự kiến

- **Giả định:** việc thu thập thông tin đặt khám, phân quyền, lưu giữ và chia sẻ dữ liệu trong phạm vi sản phẩm có thể được thực hiện với quy trình, thẩm quyền và nguồn lực phù hợp. Nếu mở rộng sang hồ sơ chuyên môn, kê đơn hoặc thanh toán, phải đánh giá riêng các ràng buộc liên quan.
- **Căn cứ:** E06 §434, §470, §505; E07 §663–668; NHOM. Tính phù hợp khi áp dụng thật CHUA-RO.
- **Tin tưởng: Thấp.** Có nhắc quyền hạn và audit nhưng chưa xác định bối cảnh triển khai, yêu cầu áp dụng hay người duyệt nghiệp vụ.
- **Nếu sai:** sản phẩm được đưa vào sử dụng khi điều kiện vận hành chưa được xác minh hoặc phạm vi vượt khả năng xác minh của nhóm.
- **Kiểm chứng đề xuất:** xác định dữ liệu cần dùng, quyền hạn, trách nhiệm và câu hỏi nghiệp vụ trước thử nghiệm vận hành. Nghiên cứu nguồn chính thức hiện hành theo phạm vi dự kiến và nhờ người phù hợp rà soát. Báo cáo này chưa đánh giá hay kết luận tuân thủ pháp luật.

### 5.4. Feasibility — Khả năng thực hiện kỹ thuật

#### FEA-01 — Có thể mô hình hóa lịch và các ngoại lệ nhất quán

- **Giả định:** lịch bác sĩ, sức chứa, khách trực tiếp, giữ chỗ, duyệt/đổi/hủy có thể được mô tả đủ rõ để xử lý xung đột.
- **Căn cứ:** E02 §080; E06 §331–338, §373–392; E08 §792–804; NHOM.
- **Tin tưởng: Trung bình.** Tài liệu đã nhận diện xung đột và kiểm tra đồng thời, nhưng chưa có chính sách vận hành được xác nhận hoặc kiểm chứng kỹ thuật của nhóm.
- **Nếu sai:** vẫn nhận lịch vượt công suất, giữ chỗ sai hoặc nhân viên phải sửa tay nhiều.
- **Kiểm chứng đề xuất:** trước hết cùng người vận hành kiểm tra các tình huống giấy: hai yêu cầu cùng giờ, bác sĩ nghỉ, khách trực tiếp chen lịch, hủy khi chờ duyệt. Ghi quy tắc chưa thống nhất. Thử nghiệm kỹ thuật đồng thời chỉ được đề xuất cho bước sau, chưa viết code trong lần này.

#### FEA-02 — Các tích hợp được nêu có điều kiện sử dụng phù hợp dự án

- **Giả định:** các dịch vụ thông báo, đăng nhập, thanh toán và AI mà nhóm xem xét có quyền truy cập, môi trường thử, chi phí và điều kiện dữ liệu phù hợp.
- **Căn cứ:** E09 §870–881; NHOM. Tình trạng API/model/gói dịch vụ hiện tại CHUA-RO.
- **Tin tưởng: Thấp.** Word liệt kê công cụ, chưa có kết quả kiểm tra quyền truy cập hoặc điều kiện tích hợp.
- **Nếu sai:** kế hoạch bị chặn bởi đăng ký, xác minh tài khoản, chi phí hoặc phụ thuộc dịch vụ ngoài.
- **Kiểm chứng đề xuất:** lập bảng điều kiện cần, người sở hữu tài khoản, chi phí và phương án mô phỏng; đối chiếu tài liệu chính thức hiện hành khi thực hiện nghiên cứu tích hợp. Vòng nghiên cứu này chỉ lập câu hỏi và kế hoạch xác minh, không tự đăng ký, gửi tin hoặc thanh toán.

#### FEA-03 — Dữ liệu hiện có đủ nhất quán để nhập và liên kết đúng

- **Giả định:** hồ sơ, danh mục thuốc và hóa đơn hiện tại có thể chuẩn hóa mà không gây ghép nhầm người hoặc sai đơn vị/số lượng.
- **Căn cứ:** E03 §109–114; E04 §153–155; E07 §600–643; AI + NHOM; chất lượng dữ liệu thật CHUA-RO.
- **Tin tưởng: Thấp.** Danh sách entities không chứng minh dữ liệu nguồn sạch hoặc có định danh đáng tin cậy.
- **Nếu sai:** báo cáo sai, tồn kho sai hoặc thông tin khám gắn sai người; tăng công chuyển đổi.
- **Kiểm chứng đề xuất:** xin mẫu cấu trúc hoặc bộ dữ liệu giả theo định dạng thực tế; kiểm tra trường thiếu, trùng, quy đổi và trường hợp nhiều người dùng chung số điện thoại. Ghi vấn đề chất lượng và quyền tiếp cận trước khi đề xuất import dữ liệu.

### 5.5. Ethics — Đạo đức và tác động tới con người

#### ETH-01 — Có thể nghiên cứu nhu cầu mà không cần thu thập dữ liệu sức khỏe nhận diện cá nhân

- **Giả định:** câu hỏi, mẫu biểu và bằng chứng về quy trình có thể được thu thập ở mức cần thiết, có sự đồng ý phù hợp và không lộ dữ liệu người bệnh.
- **Căn cứ:** E05 §160, §198; E07 §663–665; NHOM. Khả năng thực hiện của nhóm là SUY-LUAN.
- **Tin tưởng: Thấp.** Lời hứa bảo mật trong bảng hỏi chưa đi kèm cách thu thập, truy cập, lưu giữ và xóa dữ liệu cụ thể.
- **Nếu sai:** người tham gia mất niềm tin hoặc tài liệu nghiên cứu chứa thông tin nhạy cảm ngoài mục tiêu.
- **Kiểm chứng đề xuất:** rà từng trường và câu hỏi, dùng mã người tham gia, ưu tiên ví dụ đã loại nhận diện hoặc dữ liệu giả; ghi mục đích sử dụng, người được đọc và thời hạn giữ theo thỏa thuận. Nếu ghi âm, xin phép trước; không yêu cầu bệnh án thật để chứng minh pain point.

#### ETH-02 — Người dùng hiểu đúng giới hạn của gợi ý AI và mẫu kê đơn

- **Giả định:** nếu tiếp tục nghiên cứu AI gợi ý chuyên khoa hoặc mẫu kê đơn, người dùng không hiểu nhầm chúng là quyết định chuyên môn đã được xác nhận.
- **Căn cứ:** E03 §117, E04 §152, E08 §817–818, E09 §873–875; AI + NHOM; khả năng hiểu nhầm là SUY-LUAN.
- **Tin tưởng: Thấp.** Chưa xác định rõ mục đích, người dùng, giới hạn hoặc người có thẩm quyền rà soát đầu ra.
- **Nếu sai:** người dùng tin quá mức vào gợi ý và làm theo thông tin chưa được đánh giá trong bối cảnh của họ.
- **Kiểm chứng đề xuất:** làm rõ chức năng dự kiến có đưa ra nội dung chuyên môn hay chỉ điều hướng hành chính; nhờ người có chuyên môn xem xét tình huống giả định và cách diễn đạt. Chưa thử gợi ý trên bệnh nhân thật hoặc kết luận độ an toàn của giải pháp trong vòng nghiên cứu này.

#### ETH-03 — Quy trình mới không làm người khó dùng công nghệ bị bỏ lại

- **Giả định:** người không tự dùng web hoặc cần người thân hỗ trợ vẫn có cách tiếp cận và được ghi nhận đúng.
- **Căn cứ:** E06 §283, §337; E08 §799, §804, §808; NHOM; tác động loại trừ là SUY-LUAN.
- **Tin tưởng: Thấp.** Có đề xuất đặt hộ/khách trực tiếp nhưng chưa có nghiên cứu về nhu cầu hỗ trợ và nguyên tắc ưu tiên.
- **Nếu sai:** bỏ sót nhóm người dùng, nhầm người đặt với người khám hoặc phát sinh bất công trong điều phối.
- **Kiểm chứng đề xuất:** tìm hiểu các tình huống có người hỗ trợ, không có điện thoại riêng hoặc đến trực tiếp; nhờ nhân viên mô tả cách hiện tại xác định danh tính và ưu tiên. Không mặc định tuổi quyết định năng lực dùng công nghệ.

### 5.6. Go-to-Market — Tiếp cận và đưa sản phẩm tới người dùng

#### GTM-01 — Nhóm có thể tiếp cận đúng người để nghiên cứu

- **Giả định:** có thể trao đổi với người trực tiếp vận hành và người quyết định, thay vì chỉ nhờ bạn bè đóng vai.
- **Căn cứ:** E07 §731–743 có kế hoạch stakeholders, E02 §051 nêu thiếu dữ liệu thực tế; NHOM. Khả năng tiếp cận hiện tại CHUA-RO.
- **Tin tưởng: Thấp.** Chưa có xác nhận đầu mối, lịch gặp hoặc cam kết tham gia trong đầu vào.
- **Nếu sai:** nhóm tiếp tục dựa trên mô phỏng, khó kiểm chứng nhu cầu hoặc chuẩn bị thử nghiệm thực tế.
- **Kiểm chứng đề xuất:** lập danh sách vai trò có thể tiếp cận, đầu mối do nhóm xác nhận, cách xin tham gia và lịch dự kiến. Chưa liên hệ hoặc gửi tin thay nhóm. Nếu không tiếp cận được, ghi rõ giới hạn của nghiên cứu tài liệu.

#### GTM-02 — Có lợi ích đủ rõ để phòng khám thử và duy trì cách làm mới

- **Giả định:** lợi ích ở một quy trình cụ thể có thể thuyết phục phòng khám dành thời gian đánh giá và thay đổi công cụ hiện tại.
- **Căn cứ:** E01 §043–044; E03 §113–114; E04 §155; NHOM + AI. Lý do chuyển đổi thật CHUA-RO.
- **Tin tưởng: Thấp.** “Đơn giản” hoặc “trọn gói” chưa được chứng minh là lý do đủ mạnh so với công sức đổi hệ thống.
- **Nếu sai:** có thể có lời khen về ý tưởng nhưng không có người sẵn sàng thử hoặc duy trì sử dụng.
- **Kiểm chứng đề xuất:** hỏi về lần tìm, thử, mua hoặc từ chối công cụ gần nhất; ghi người tham gia quyết định, rào cản, điều kiện thử và dấu hiệu cam kết về thời gian. Không coi đồng ý nghe giới thiệu là chấp nhận sử dụng sản phẩm.

#### GTM-03 — Nhóm biết phân khúc và kênh tiếp cận phù hợp

- **Giả định:** thông điệp và kênh tiếp cận có thể nhắm vào một nhóm phòng khám cụ thể và đúng người ảnh hưởng tới quyết định.
- **Căn cứ:** E01 §005, §043 nói nhỏ/vừa và một phòng khám; E03 mô phỏng đa khoa có nhà thuốc; E08 đề cập đa chi nhánh. NHOM + AI; kênh tiếp cận là SUY-LUAN.
- **Tin tưởng: Thấp.** Phân khúc còn rộng, chưa có bằng chứng kênh nào tạo được cuộc trao đổi phù hợp.
- **Nếu sai:** thông điệp quá chung hoặc nghiên cứu sai đối tượng, khiến kết luận nhu cầu không áp dụng được.
- **Kiểm chứng đề xuất:** mô tả tiêu chí chọn người/cơ sở nghiên cứu theo nghiệp vụ và công cụ đang dùng; hỏi họ thường tìm hiểu giải pháp qua đâu. Đánh giá sự phù hợp của người tiếp cận được, không chỉ đếm phản hồi.

### 5.7. Strategy & Objectives — Định hướng và mục tiêu

#### STR-01 — Nhóm có thể thống nhất một vấn đề và kết quả cần nghiên cứu trước

- **Giả định:** sau khi đối chiếu bằng chứng, nhóm chọn được trọng tâm nghiên cứu giữa lịch hẹn và vận hành đầy đủ mà không mặc định mọi phân hệ đều cần thiết.
- **Căn cứ:** E02 §081 đối chiếu E04 §151–156, E07 §721–730, E08 §788–853; NHOM. Khả năng thống nhất là SUY-LUAN.
- **Tin tưởng: Thấp.** Có các hướng và nhãn MVP/Must-have khác nhau, chưa có biên bản quyết định hoặc người chịu trách nhiệm quyết định.
- **Nếu sai:** đầu vào của thiết kế, PRD và Sprint mâu thuẫn; phạm vi tăng liên tục.
- **Kiểm chứng đề xuất:** nhóm lập bảng vấn đề, người gặp, bằng chứng và điều chưa biết cho từng hướng; xác nhận kết quả sản phẩm cần đạt và người chốt quyết định. Chốt câu hỏi nghiên cứu trước; chưa phê duyệt MVP tại đây.

#### STR-02 — Có khoảng trống đáng nghiên cứu trong các cách giải quyết hiện có

- **Giả định:** một phân khúc cụ thể chưa được phục vụ phù hợp về quy trình, khả năng sử dụng hoặc công sức chuyển đổi.
- **Căn cứ:** E01 §007–043 và E02 §084; NHOM + CHUA-RO đối với thông tin đối thủ. Khoảng trống là SUY-LUAN.
- **Tin tưởng: Thấp.** So sánh tính năng chưa chứng minh nhu cầu chưa được đáp ứng, chưa có trải nghiệm người dùng hoặc nguồn đối thủ trực tiếp kèm thời điểm.
- **Nếu sai:** nhóm mô tả khác biệt không tồn tại hoặc dựa vào tính năng đối thủ thực tế đã đáp ứng tốt.
- **Kiểm chứng đề xuất:** ở vòng nghiên cứu thị trường tiếp theo, dùng trang/tài liệu chính thức có ngày truy cập để so sánh cùng đối tượng và công việc; kết hợp lý do người dùng chọn/từ chối công cụ hiện tại. So cả sổ, Excel, điện thoại và Zalo. Kiểm tra lý do khách hàng chọn sản phẩm thay cho giải pháp hiện có; tính mới không thay thế giá trị sử dụng.

#### STR-03 — Có thể đánh giá kết quả bằng thước đo gắn với vấn đề đã chọn

- **Giả định:** nhóm có thể xác định một kết quả quan sát được thay vì chỉ đánh giá số lượng tính năng đã hoàn thành.
- **Căn cứ:** E07 §673–689 liệt kê KPI; E02 §082 nói phản hồi sau Sprint; NHOM. Khả năng đo là SUY-LUAN.
- **Tin tưởng: Thấp.** Chưa có trọng tâm, baseline, dữ liệu đo, mẫu số hoặc mục tiêu được nhóm xác nhận.
- **Nếu sai:** sản phẩm nhiều chức năng nhưng không biết có cải thiện công việc hay không.
- **Kiểm chứng đề xuất:** sau khi rõ vấn đề, mô tả ai đo, nguồn dữ liệu, thời điểm và cách tính một kết quả phù hợp; đo hiện trạng trước khi đặt mức cải thiện. KPI kinh doanh thật và kết quả thử trên dữ liệu giả cần báo cáo riêng. Chưa tự đặt chỉ tiêu giảm thời gian/no-show ở đây.

### 5.8. Team — Đội ngũ và cách phối hợp

#### TEAM-01 — Năng lực và thời gian thực tế đủ cho phạm vi sẽ được xác định

- **Giả định:** đội ngũ có thể hoàn thành nghiên cứu và các bước sau với nguồn lực hiện có.
- **Căn cứ:** E02 §051, §075–082 và E09 nêu rủi ro nguồn lực cùng kỳ vọng tiết kiệm thời gian; NHOM + CHUA-RO. Chưa có kế hoạch năng lực hiện tại được xác nhận.
- **Tin tưởng: Thấp.** Chưa có ngân sách, thời lượng, kỹ năng và phân công cụ thể; kỳ vọng tiết kiệm thời gian chưa có căn cứ đo.
- **Nếu sai:** chia việc quá sức, nghiên cứu không đủ hoặc phải cắt phạm vi sát hạn.
- **Kiểm chứng đề xuất:** xác định kỹ năng, thời lượng khả dụng, ngân sách, trách nhiệm và mốc dự án; lập danh sách năng lực còn thiếu. Ước lượng lại sau khi rõ phạm vi, không suy năng lực từ số người.

#### TEAM-02 — Nhóm có người chịu trách nhiệm quyết định và rà soát nghiệp vụ

- **Giả định:** có người tổng hợp discovery, người quyết định hướng nghiên cứu và đầu mối kiểm tra nghiệp vụ phòng khám.
- **Căn cứ:** E02 §082, E06 §595, E07 §731–754; NHOM. Phân công cụ thể chưa có; SUY-LUAN.
- **Tin tưởng: Thấp.** Chưa có phân công được xác nhận cho quyết định sản phẩm, rà soát nghiệp vụ, vận hành và hỗ trợ.
- **Nếu sai:** mỗi người phát triển một hướng, agent tạo nhiều kết quả nhưng không ai kiểm tra hoặc chốt.
- **Kiểm chứng đề xuất:** ghi tên và trách nhiệm do nhóm tự xác nhận cho thu thập bằng chứng, rà soát và quyết định; thống nhất cách ghi nhận ý kiến chưa giải quyết. Người quyết định sản phẩm và người xác nhận nghiệp vụ cần có trách nhiệm rõ ràng; không mặc định hai vai trò do cùng một người đảm nhiệm.

#### TEAM-03 — Nhóm có thể dùng skill mà vẫn giữ được nguồn gốc và trách nhiệm kiểm tra

- **Giả định:** nhóm hiểu file skill là quy trình, đầu ra agent là bản cần rà soát và AI nhập vai không thay thế nghiên cứu người thật.
- **Căn cứ:** E02 §085, E03 §091 và E04 §120 cho thấy nguy cơ lẫn nguồn; NHOM + AI. Khả năng áp dụng nhất quán là SUY-LUAN.
- **Tin tưởng: Thấp.** Việc cài skill chưa chứng minh các thành viên đã hiểu và kiểm tra đúng đầu ra.
- **Nếu sai:** báo cáo trình bày dữ liệu mô phỏng như bằng chứng thực tế, hoặc nhóm không giải thích được vì sao có kết luận.
- **Kiểm chứng đề xuất:** mỗi thành viên thử giải thích một giả định, chỉ vị trí nguồn và lý do tin tưởng; giữ prompt, phiên bản file skill, kết quả và ghi chú chỉnh sửa. Người rà soát ghi rõ đồng ý/chỉnh sửa/chờ bằng chứng; không coi kết quả agent là tự động được duyệt.


## 6. Kết luận và hành động

24 giả định là danh sách rủi ro, không phải kết quả khảo sát. VAL-01 và USE-03 còn thiếu bằng chứng trực tiếp; FEA-01 mới được nguồn công khai hỗ trợ ở việc nhận diện quy tắc/ngoại lệ. Chưa có giả định nào được xác thực toàn bộ.

Tiếp tục theo [Research Plan](./05-research-plan.md): xác định cơ sở và người tham gia phù hợp, nghiên cứu tác vụ hiện tại, quy trình quyết định sử dụng, chi phí vận hành và nguồn lực. Thu baseline trước khi đặt mục tiêu cải thiện. Mỗi quyết định cần có người chịu trách nhiệm, nguồn và giới hạn áp dụng; xem [Discovery Review](./outputs/discovery-review.md) để theo dõi trạng thái.
