# Healthcare Portal — Lean Canvas v2

Cập nhật ngày 21/11/2026.

Lean Canvas trình bày những giả thuyết về vấn đề, cách giải quyết, khách hàng và khả năng duy trì sản phẩm. Báo cáo xét một cơ sở độc lập thuộc phân khúc phòng khám tư nhân nhỏ và vừa. Thông tin công bố của các dịch vụ khác giúp hiểu thị trường, chưa chứng minh khách hàng sẽ chọn hoặc trả tiền cho Healthcare Portal.

## 1. Vấn đề

Người đặt và lễ tân cần cùng biết yêu cầu đã được xác nhận chưa, lịch nào đang áp dụng và ai xử lý thay đổi. Dự án đang tìm hiểu ba nhóm tình huống: người đặt chưa rõ kết quả; phòng khám cần đối chiếu khả năng nhận và bàn giao khi đổi/hủy hoặc bác sĩ nghỉ; thông tin cần được kiểm tra thêm khi đặt hộ và nhận khách trực tiếp.

Ảnh hưởng và mức ưu tiên của những tình huống này chưa được đo tại cơ sở mục tiêu. Điện thoại, trò chuyện hoặc phần mềm đang dùng có thể đã đáp ứng tốt. [Problem Statement](./problem-statement.md) giải thích từng vấn đề, căn cứ, nhu cầu và trạng thái 24 giả định; việc có nhiều đối thủ cung cấp lịch hẹn chưa đủ xác nhận nhu cầu đổi công cụ.

## 2. Hướng giải pháp

### SH-01 — Rõ kết quả và lịch hiện hành

Hướng thứ nhất là làm rõ kết quả và lịch đang áp dụng: phân biệt yêu cầu chờ, lịch được nhận, hướng dẫn và kết quả thay đổi. Hướng này mang mã SH-01, gắn với vấn đề chưa rõ kết quả đặt và nhu cầu N01. Cần kiểm tra người đặt có hiểu đúng và hoàn thành tác vụ hay không.

### SH-02 — Điều phối theo khả năng tiếp nhận

Hướng thứ hai là hỗ trợ điều phối dựa trên ca làm và khả năng tiếp nhận. Yêu cầu từ web, điện thoại hoặc quầy cần được đối chiếu theo nguồn lịch mà cơ sở tin cậy, thay vì chỉ thêm một nơi nhập thông tin. Hướng SH-02 gắn với vấn đề về khả năng nhận và nhu cầu N02; cần biết công việc nào được thay thế, công việc nào vẫn phải làm và cách mới có tăng việc không.

### SH-03 — Có người chịu trách nhiệm xử lý thay đổi

Hướng thứ ba là theo dõi việc thay đổi tới người chịu trách nhiệm: đề nghị đổi riêng, xử lý ca bị ảnh hưởng, lịch sử cập nhật và việc liên hệ. Hướng SH-03 giải quyết nhu cầu N03, N05 và tình huống đổi/hủy hoặc bác sĩ đổi ca. Phải hiểu chính sách cơ sở, quyền xử lý và cách người đặt nhận kết quả trước khi chọn cách triển khai.

### SH-04 — Đối chiếu đúng người khi tiếp nhận

Hướng thứ tư là đối chiếu đúng người khi tiếp nhận. Ghi riêng người đặt và người khám, xem xét người đến trực tiếp trong khả năng nhận chung và ghi giờ đến là những phương án đang được cân nhắc. Hướng SH-04 gắn với nhu cầu N04, cần kiểm chứng dữ liệu định danh cần thiết và tác vụ tại quầy.

Đây là các phương án để thử, chưa phải tính năng được chứng minh mới hơn hoặc tốt hơn đối thủ, cũng chưa chốt phạm vi MVP. [User Personas](./user-personas.md) giải thích công việc của từng vai trò, còn [Journey Map](./customer-journey-map.md) minh họa cách những hướng này có thể kết nối trong một lượt hẹn.

## 3. Giá trị đề xuất

> Biết lịch nào đã được xác nhận, ai xử lý thay đổi và cần làm gì khi đến khám.

Giá trị này phù hợp [tầm nhìn sản phẩm](./product-vision-v2.md) và là lý do sử dụng đang được nghiên cứu. Cần biết người dùng có thực sự gặp khó khăn liên quan và cách mới có phù hợp hơn lựa chọn hiện tại không. Tên ô trong Lean Canvas là Unique Value Proposition, nhưng không có nghĩa tính năng hoặc lợi thế đã độc nhất.

## 4. Lợi thế khó sao chép

Hiện chưa xác định được lợi thế khó sao chép. Đầu vào chưa chứng minh dự án có dữ liệu độc quyền, quan hệ triển khai, kênh tiếp cận hoặc năng lực đặc biệt. Sử dụng AI, skills hoặc giao diện đơn giản chưa đủ làm lợi thế cạnh tranh.

Hiểu sâu nghiệp vụ của phân khúc và có khả năng triển khai lặp lại có thể là hướng xây năng lực về sau. Tuy nhiên, cần phân biệt hướng muốn xây với tài sản đã có và được chứng minh.

## 5. Khách hàng và người dùng

Khách hàng tổ chức ưu tiên nghiên cứu là một phòng khám độc lập có người chịu trách nhiệm lịch và tiếp nhận cả yêu cầu hẹn trước lẫn khách trực tiếp. Cần chọn chuyên khoa, hiểu công cụ đang dùng, tác động vấn đề và điều kiện cơ sở có thể tham gia thử. Chưa có cơ sở đầu tiên hoặc ngưỡng nhân sự, lượt khám để xác định cụ thể thế nào là nhỏ và vừa.

Người dùng chính dự kiến là người tự đặt hoặc đặt hộ và nhân viên điều phối, tương ứng P01, P02. Bác sĩ là bên cung cấp khả năng làm việc và có thể cần giao diện trực tiếp nếu tác vụ thực tế cho thấy cần thiết. Quản lý tham gia chính sách và quyền; người quyết định dùng, người duyệt chi và người chịu chi phí vẫn cần được xác định riêng.

Chưa có dữ liệu để ước lượng quy mô thị trường hoặc xác nhận nhóm khách hàng đầu tiên. Một cơ sở đồng ý phỏng vấn chưa tự trở thành khách mua phần mềm; một người có thể kiêm nhiều vai trò nhưng chức danh không đủ để suy ra hành vi hoặc quyền quyết định.

## 6. Kênh tiếp cận

Để tiếp cận cơ sở, dự án đang cân nhắc đầu mối chuyên môn, sự giới thiệu và trao đổi trực tiếp với người có thẩm quyền. Điều cần kiểm tra là có tiếp cận đúng vai trò không, vì sao họ chọn hoặc từ chối tìm hiểu và dưới điều kiện nào họ dành thời gian thử. Chưa có kênh được cam kết hoặc được chứng minh hiệu quả.

Nếu có cơ sở phù hợp, việc bắt đầu sử dụng có thể cần quản lý và nhân viên điều phối phối hợp cấu hình, đào tạo và thử quy trình. Dấu hiệu có ý nghĩa hơn việc đồng ý xem giới thiệu là cơ sở chỉ định người xử lý và dành thời gian thực hiện công việc qua giải pháp.

Người bệnh có thể biết cách đặt qua đường dẫn hoặc hướng dẫn do cơ sở công bố trên kênh họ đang dùng, đồng thời có hỗ trợ từ nhân viên. Quyền công bố, cách người đặt tìm tới và khả năng hoàn thành tác vụ đều còn cần kiểm tra. Các kênh trong S14 chỉ là ví dụ của một cơ sở, không chứng minh dự án có thể khai thác chúng để thu hút khách hàng. Tìm kiếm web và phỏng vấn là cách thu bằng chứng, không được tính như kênh bán hàng.

## 7. Nguồn tài chính và mô hình kinh doanh

Giả thuyết ưu tiên nghiên cứu là cung cấp dịch vụ theo gói định kỳ cho một địa điểm phòng khám. Phí cấu hình, đào tạo hoặc tiếp nhận nếu có cần được làm rõ riêng. Trong giả thuyết này, người đặt khám không trả phí đặt lịch. Dự án chưa chọn mức giá, chu kỳ thu tiền hoặc gói dịch vụ.

Một phương án khác là sản phẩm dùng nội bộ do một cơ sở cấp ngân sách phát triển và vận hành. Lựa chọn phụ thuộc người sở hữu sản phẩm, người duyệt chi và điều kiện hỗ trợ; chưa được xem là mô hình đã quyết định. Trước khi định giá cần hỏi hành vi mua phần mềm gần nhất, khoản chi đang có, chi phí chuyển đổi và người chịu chi phí vận hành, gắn với VIA-01 và VIA-02.

Giá đối thủ chỉ là tham khảo có thời điểm, không tự trở thành giá phù hợp của dự án. Chưa có dữ liệu để tính doanh thu, chi phí thu hút khách hàng hay giá trị vòng đời khách hàng, thường được gọi là CAC và LTV. Cũng chưa có căn cứ để lập dự báo tăng trưởng.

## 8. Chi phí cần tìm hiểu

- **Phát triển ban đầu.** Chi phí phát triển ban đầu gồm nghiên cứu, thiết kế, kỹ thuật, kiểm tra và rà soát nghiệp vụ. Cần xác định thời lượng theo trách nhiệm, phạm vi và năng lực còn thiếu trước khi ước lượng ngân sách, thay vì suy năng lực từ số người hoặc kỳ vọng AI tiết kiệm thời gian.

- **Tiếp nhận cơ sở.** Khi tiếp nhận một cơ sở, các công việc có thể gồm cấu hình ca và quyền, chuẩn bị dữ liệu nếu cần, đào tạo và hỗ trợ ban đầu. Cần ghi số giờ công trên mỗi cơ sở, những bước bàn giao và yêu cầu hỗ trợ. Đây là phần dễ bị bỏ sót nếu chỉ tính chi phí viết phần mềm.

- **Vận hành và dịch vụ ngoài.** Chi phí vận hành định kỳ còn gồm hạ tầng, sao lưu, giám sát, bảo vệ dữ liệu, bảo trì và xử lý sự cố. Nếu chọn dịch vụ xác thực, thông báo hoặc tích hợp, cần kiểm tra điều kiện và giá tại thời điểm chọn. Prototype có thể mô phỏng những phần đó, nhưng chi phí mô phỏng chưa phản ánh vận hành thật.

Hiện chưa có tổng ngân sách hoặc đơn giá. Không dùng tiền trong AI nhập vai hay nhãn gói miễn phí của đối thủ làm bằng chứng rằng dự án có chi phí thấp.

## 9. Những kết quả có thể đo

Các phép đo dưới đây là đề xuất, chưa có kết quả hoặc KPI số. Trước khi thu thập, cần thống nhất điều kiện tác vụ, người tham gia, kỳ quan sát và cách ghi dữ liệu. Phải tách tác vụ thử trên prototype khỏi lượt khám và hoạt động thật.

### M01 — Hiểu đúng kết quả

- **Cách đo:** Có thể ghi số tình huống người đặt giải thích đúng yêu cầu chờ, lịch xác nhận, lịch đang áp dụng và bước tiếp theo trên tổng tình huống hợp lệ đã hỏi.
- **Khi đọc kết quả:** Các bước gửi, xem kết quả và đổi lịch trong Journey Map là nơi phù hợp để thử. Cần ghi cả lỗi hiểu và mức trợ giúp; hiểu đúng chưa đồng nghĩa hài lòng.

### M02 — Hoàn thành tác vụ

- **Cách đo:** Có thể tính số tác vụ đặt, đổi, hủy hoặc tiếp nhận được thực hiện đúng điều kiện đã thống nhất mà không cần trợ giúp trên tổng tác vụ hợp lệ.
- **Khi đọc kết quả:** Kết quả cần tách theo vai trò và loại tác vụ. Một mẫu người thử prototype chưa đại diện cho mọi người sử dụng.

### M03 — Xử lý yêu cầu chờ

- **Cách đo:** Khi có hoạt động có thể ghi mốc thời gian, đo khoảng từ gửi tới quyết định đầu tiên, đồng thời thống kê riêng yêu cầu còn chờ, bị từ chối hoặc hết hạn.
- **Khi đọc kết quả:** Không nên chỉ lấy những yêu cầu thành công rồi bỏ phần chưa xử lý. Prototype chủ yếu giúp kiểm tra cách hiểu trạng thái; thời gian vận hành cần dữ liệu thực tế.

### M04 — Công việc của nhân viên

- **Cách đo:** So thời gian thao tác, số nguồn bắt buộc đọc và ghi, cùng bước nhập lại trên những tình huống tương đương trước và sau khi thử.
- **Khi đọc kết quả:** Cần tính cả công cụ song song và ảnh hưởng của việc người dùng còn đang học cách mới. Ít màn hình hoặc nhiều thao tác được tự động hóa chưa đủ thay phép đo công việc.

### M05 — Khả năng tiếp tục dùng

- **Cách đo:** Khi có thử nghiệm lặp theo thời gian, ghi cơ sở nào thực sự điều phối công việc qua công cụ trong kỳ đã thống nhất, so với số cơ sở tham gia đủ thời gian quan sát.
- **Khi đọc kết quả:** Cần biết họ còn dùng nguồn nào khác và vì sao ngừng. Đăng nhập, xem giới thiệu hoặc thử một lần không đủ chứng minh tiếp tục sử dụng.

Nếu sau này có mô hình tài chính và giao dịch, có thể bổ sung doanh thu thực thu, chi phí hỗ trợ hoặc tiếp nhận trên mỗi cơ sở và điều kiện tiếp tục trả phí. Chưa nên dùng số tài liệu, số tính năng hoặc số yêu cầu gửi thay cho giá trị sử dụng thực tế.

## 10. Cách cập nhật Canvas

Thứ tự khám phá nghiệp vụ vẫn là xác nhận giá trị vấn đề, kiểm tra công việc nhân viên rồi kiểm tra quy tắc và ngoại lệ, tương ứng VAL-01, USE-03 và FEA-01. Nghiên cứu tài chính, tiếp cận và vận hành cần tiến hành song song. Dùng [Interview Guide](../03-interview-guide.md) để hỏi trải nghiệm đã xảy ra, [Journey Map](./customer-journey-map.md) để chuẩn bị tình huống thử và các phép đo ở trên để ghi nhận kết quả.

Nếu chỉ thu được lời khen hoặc mô tả tính năng, các nhận định vẫn là giả thuyết. Nếu cách mới làm tăng việc chưa được giải thích, cần sửa phương án. Có thể khám phá wireframe và prototype từ những hướng hiện có, nhưng trước thiết kế chi tiết cần xác nhận quy trình, quyền, khả năng tiếp nhận và dữ liệu tại cơ sở; chưa có căn cứ để cam kết giá, lịch triển khai hoặc vận hành thật.
