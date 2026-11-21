# Healthcare Portal — Tầm nhìn sản phẩm

Cập nhật ngày 21/11/2026.

## 1. Tầm nhìn

> Giúp phòng khám và người đặt phối hợp từ đặt hẹn đến tiếp nhận bằng lịch rõ ràng và trách nhiệm xử lý cụ thể.

Healthcare Portal hướng tới một cách sắp xếp lịch mà người đặt hiểu mình đã có lịch hay còn chờ, còn nhân viên phòng khám biết việc nào cần xử lý và ai cần được báo lại. Khi có thay đổi, các bên có thể dựa trên thông tin hiện hành thay vì phải tự suy đoán từ những trao đổi trước đó.

Tầm nhìn này xuất phát từ [vấn đề trọng tâm](./problem-statement.md): người đặt và lễ tân cần cùng biết kết quả đặt, lịch đang áp dụng và trách nhiệm xử lý thay đổi. Nó định hướng lựa chọn sản phẩm, chưa phải khẳng định Healthcare Portal đã giảm thời gian chờ, giảm công việc hoặc ngăn được trùng lịch.

## 2. Sản phẩm hướng tới ai?

Phân khúc đang nghiên cứu là phòng khám tư nhân nhỏ và vừa tại Việt Nam. Dự án đề xuất bắt đầu với một cơ sở độc lập tại một địa điểm để tìm hiểu kỹ chính sách và công việc trước khi mở rộng. Chuyên khoa, quy mô hoạt động và cơ sở đầu tiên chưa được chọn.

Hai nhóm sử dụng chính dự kiến là người sắp xếp khám cho mình hoặc người thân, và nhân viên tiếp nhận, điều phối lịch. Người đặt cần hiểu kết quả và bước tiếp theo; nhân viên cần biết ca làm, khả năng nhận và cách xử lý thay đổi. Những công việc này tương ứng với các nhu cầu N01–N04 trong Problem Statement và các vai trò P01, P02 trong [User Personas](./user-personas.md).

Bác sĩ cung cấp thông tin về khả năng làm việc và là bên cần phối hợp khi ca thay đổi, gắn với nhu cầu N05 và vai trò P03. Quản lý cơ sở có thể quyết định chính sách, cách phân quyền và việc sử dụng phần mềm. Người quyết định dùng và người duyệt chi có thể là cùng một người hoặc khác nhau; hiện chưa có dữ liệu để xác định. Cũng chưa nên mặc định mỗi vai trò đều cần một giao diện riêng.

## 3. Giá trị đề xuất và cách giải quyết

Giá trị đề xuất của Healthcare Portal là: **Biết lịch nào đã được xác nhận, ai xử lý thay đổi và cần làm gì khi đến khám.** Đây là lý do sử dụng đang được nghiên cứu, cần kiểm tra với người đặt và cơ sở thay vì coi là lợi thế đã được chứng minh.

Ba khái niệm giữ vai trò khác nhau:

| Thành phần | Trả lời câu hỏi | Nội dung của Healthcare Portal |
|---|---|---|
| Tầm nhìn | Sản phẩm hướng tới điều gì lâu dài? | Phối hợp từ đặt hẹn đến tiếp nhận bằng lịch rõ và trách nhiệm cụ thể |
| Giá trị đề xuất | Người sử dụng được lợi gì? | Biết lịch đã xác nhận, người xử lý thay đổi và bước tiếp theo |
| Khả năng sản phẩm | Có thể tạo giá trị bằng cách nào? | Gửi yêu cầu, duyệt, đổi/hủy, xử lý ca nghỉ, tiếp nhận và lịch sử |

Các khả năng ở hàng cuối nối với SH-01–SH-04 trong [Lean Canvas](./lean-canvas-v2.md). Chúng là phương tiện đang được cân nhắc, chưa phải phạm vi tính năng đã chốt.

Thị trường đã có công cụ đặt và quản trị lịch cho cơ sở, chẳng hạn [BookingCare DX — S03](https://bookingcare.vn/goi-chuyen-doi-so) và [YouMed HCP — S08](https://youmed.vn/hcp/). Vì vậy, Healthcare Portal cần được đánh giá bằng mức phù hợp với quy trình thực tế và công sức thay đổi so với lựa chọn hiện có. Có web đặt lịch hoặc giao diện đơn giản chưa đủ chứng minh lý do khách hàng sẽ chọn sản phẩm.

## 4. Ranh giới đang theo đuổi

Ranh giới hiện tại được chia như sau:

- **Đang tập trung:** một lượt hẹn từ lúc được đề nghị đến khi người bệnh được tiếp nhận tại quầy.
- **Cần quyết định riêng:** bệnh án, kê đơn, kho thuốc, AI tư vấn, thanh toán, đa chi nhánh và ghi nhận bắt đầu khám. Những hướng này cần căn cứ nhu cầu và khả năng thực hiện trước khi bổ sung.

Việc được nhận lịch chưa đồng nghĩa được bắt đầu khám đúng phút. Tương tự, lưu lịch vào một hệ thống chưa tự chứng minh nhân viên ít việc hơn nếu vẫn phải duy trì nguồn khác. Những khác biệt này cần được giữ rõ khi viết nội dung và thiết kế tương tác.

[Journey Map](./customer-journey-map.md) minh họa một phương án để khám phá giải pháp. Trước khi chốt thiết kế chi tiết, dự án còn cần xác nhận quyền xử lý, cách duyệt, công suất, điều kiện đổi/hủy và kênh thông báo theo cơ sở. Các đề xuất dùng để thử chưa phải chính sách vận hành đã được phê duyệt.

## 5. Vì sao chọn tầm nhìn này?

Hướng giúp người bệnh chủ động và an tâm trong toàn bộ hành trình khám có ý nghĩa nhưng rộng hơn phạm vi lịch hẹn. Hướng giảm công sức đối chiếu cho nhân viên cũng đáng theo đuổi, song hiện chưa có dữ liệu để biến nó thành lời hứa cốt lõi. Tầm nhìn được chọn tập trung vào sự phối hợp từ đặt hẹn đến tiếp nhận, vừa cụ thể cho hai phía vừa cho phép nghiên cứu các nhánh đổi, hủy và bàn giao.

Để tiếp tục, cần kiểm chứng vấn đề và quy trình với người dùng, chọn cơ sở, xác định người chịu trách nhiệm sản phẩm và nghiệp vụ, rồi làm rõ ngân sách cùng năng lực vận hành. Tầm nhìn có thể giữ trong khi cách giải quyết thay đổi theo bằng chứng; khi phạm vi thay đổi, Canvas và hành trình cần được cập nhật cùng nhau.
