# Healthcare Portal — Phát biểu vấn đề

Cập nhật ngày 21/11/2026.

## 1. Vấn đề cần tìm hiểu

Healthcare Portal hướng tới việc hỗ trợ đặt và điều phối lịch khám tại phòng khám tư nhân nhỏ và vừa ở Việt Nam. Để nghiên cứu đủ sâu, dự án đề xuất bắt đầu với một cơ sở độc lập tại một địa điểm. Chuyên khoa, quy mô hoạt động và cơ sở cụ thể vẫn chưa được chọn.

Vấn đề trọng tâm là người đặt khám và lễ tân cần cùng biết yêu cầu đã được xác nhận chưa, lịch nào đang áp dụng và ai xử lý khi có thay đổi. Chẳng hạn, một người đã gửi yêu cầu qua website có thể nghĩ rằng mình đã có lịch, trong khi phòng khám vẫn đang chờ nhân viên kiểm tra. Khi người đó muốn đổi giờ hoặc bác sĩ thay đổi ca làm, các bên còn cần biết thông tin mới đã được chấp thuận và thông báo tới đâu. Vấn đề này được lưu với mã CP-01 để truy vết.

Đây là giả thuyết cần nghiên cứu, chưa phải tình trạng đã được quan sát tại một phòng khám mục tiêu. Nếu sự thiếu thống nhất thực sự xảy ra, người đặt và nhân viên có thể phải liên hệ lại, sửa thông tin hoặc xử lý thêm tại quầy. Dự án cần tìm hiểu những việc đã xảy ra để biết ảnh hưởng có đủ lớn và đáng ưu tiên giải quyết hay không.

Phạm vi tìm hiểu đi từ lúc gửi yêu cầu tới khi người bệnh được tiếp nhận tại quầy. Việc đặt lịch chưa đồng nghĩa bác sĩ bắt đầu khám đúng phút. Tương tự, chưa có dữ liệu để khẳng định phòng khám thường xuyên trùng lịch, nhân viên đang quá tải hoặc người bệnh phải chờ lâu vì công cụ hiện tại.

## 2. Bằng chứng hiện có được hiểu như thế nào?

Phần đã thực hiện là nghiên cứu tài liệu công khai: đọc hướng dẫn, chính sách và thông tin sản phẩm do các nhà cung cấp hoặc đơn vị khám công bố. Một hướng dẫn có thể cho biết dịch vụ mô tả cách đặt và hủy lịch ra sao, nhưng chưa chứng minh người dùng làm được, hài lòng hoặc gặp khó khăn với quy trình đó. Bộ nguồn này được ghi bằng mã S01–S14 trong [phụ lục nguồn](./competitor-analysis.md#phu-luc-nguon).

Các loại nhận định được đọc theo bảng sau:

| Loại | Ý nghĩa | Cách dùng trong báo cáo |
|---|---|---|
| Thông tin có căn cứ | Truy được về nội dung một nguồn công bố | Chưa đồng nghĩa hiệu quả thực tế; nhãn cũ CB |
| Suy luận | Diễn giải từ nguồn hiện có | Giữ liên kết với căn cứ; nhãn cũ SL |
| Giả thuyết | Nhu cầu, hành vi hoặc kết quả còn cần kiểm chứng | Chưa coi là phát hiện thực địa; nhãn cũ H |
| Phương án đề xuất | Cách giải quyết hoặc luồng đang được cân nhắc | “Proposed — Needs Validation” nghĩa là cần xác nhận thêm |
| Chưa xác định | Điểm còn thiếu dữ liệu | Ghi câu hỏi và bằng chứng cần tìm; nhãn cũ CX |

Hiện chưa có phỏng vấn, quan sát ca làm, thử tác vụ hoặc kiểm chứng kỹ thuật mới. Những nhân vật và con số xuất hiện trong phần AI nhập vai của tài liệu đầu vào được giữ đúng bản chất mô phỏng, không được dùng làm dữ liệu khách hàng.

## 3. Những tình huống cụ thể cần nghiên cứu

### Người đặt chưa biết kết quả yêu cầu — SP-01

**Tình huống cần kiểm tra.** Sau khi gửi thông tin, người đặt cần biết mình đã có lịch hay vẫn phải chờ phòng khám phản hồi. Nếu thông báo không rõ, họ có thể gọi hỏi lại hoặc đến cơ sở khi chưa được nhận lịch. Đây là một khả năng cần kiểm tra, chưa phải sự việc đã được người tham gia báo cáo.

**Căn cứ và cách tìm hiểu.** Các nguồn về quy trình cho thấy cách xác nhận và ý nghĩa giờ hẹn khác nhau giữa dịch vụ. Vì vậy, nghiên cứu tiếp theo nên hỏi người đặt về lần gần nhất họ sắp xếp khám, xem thông tin xác nhận đã loại dữ liệu nhận diện và nhờ họ giải thích bước tiếp theo. Cần ghi cả trường hợp họ hiểu rõ và cách hiện tại hoạt động tốt.

### Nhân viên chưa rõ khả năng tiếp nhận — SP-02

**Tình huống cần kiểm tra.** Một tình huống cần tìm hiểu là hai yêu cầu cùng đề nghị một bác sĩ trong khoảng thời gian giao nhau, hoặc một yêu cầu đến qua điện thoại trong lúc có người đặt trên web. Nhân viên cần dựa vào nguồn lịch nào đó để quyết định có thể nhận thêm hay phải đề nghị giờ khác.

**Căn cứ và cách tìm hiểu.** Trang sản phẩm KiotViet có công bố cảnh báo trùng lịch và quá tải (S12), nhưng điều này chưa chứng minh cơ sở mục tiêu đang gặp trùng lịch. Cần theo dõi một ca làm thực tế để biết nhân viên xem lịch ở đâu, tính khả năng nhận như thế nào và xử lý yêu cầu cạnh tranh ra sao. Sau khi hiểu hiện trạng, có thể diễn tập tình huống để kiểm tra quy tắc.

### Thay đổi chưa được xử lý tới nơi — SP-03

**Tình huống cần kiểm tra.** Khi người đặt xin đổi hoặc hủy, họ cần biết yêu cầu đã được xử lý chưa và lịch cũ còn được sử dụng hay không. Khi bác sĩ nghỉ hoặc thay đổi ca, phòng khám cũng cần xác định những lượt bị ảnh hưởng, người liên hệ lại và kết quả sắp xếp mới. Nếu bàn giao chưa đầy đủ, các bên có thể tiếp tục dựa vào thông tin cũ.

**Căn cứ và cách tìm hiểu.** Nguồn công khai cho thấy nhiều chính sách đổi/hủy và nhiều kênh liên hệ khác nhau. Cách kiểm chứng phù hợp là truy lại một trường hợp đã xảy ra: ai biết thay đổi trước, ai quyết định, thông tin được sửa ở đâu và người đặt nhận kết quả bằng cách nào. Không nên suy toàn bộ công việc nội bộ chỉ từ việc người bệnh kể rằng họ đã phải gọi lại.

### Thông tin chưa khớp khi tới quầy — SP-04

**Tình huống cần kiểm tra.** Người đặt có thể là người thân, còn người tới khám là một người khác. Phòng khám cũng có thể tiếp nhận người đến trực tiếp bên cạnh người đã hẹn. Những tình huống này cần được tìm hiểu để biết nhân viên đối chiếu đúng người, đúng lượt và khả năng tiếp nhận như thế nào.

**Căn cứ và cách tìm hiểu.** CarePlus có hướng dẫn đặt cho thành viên gia đình (S13), còn tài liệu KiotViet phân biệt thao tác lưu lịch với bắt đầu khám (S11). Đây là căn cứ để đặt câu hỏi, chưa chứng minh có nhầm người hoặc sai sót tại cơ sở mục tiêu. Quan sát tiếp nhận và hỏi ví dụ về đặt hộ, dùng chung số liên hệ hoặc đến không hẹn sẽ giúp làm rõ công việc thực tế.

## 4. Nhu cầu và hướng giải quyết đang được cân nhắc

Đối với người đặt, nhu cầu đầu tiên là biết yêu cầu đang chờ hay đã có lịch, hiểu ý nghĩa giờ hẹn và biết bước tiếp theo. Nhu cầu này mang mã N01. Hướng giải pháp tương ứng là tách rõ việc gửi yêu cầu, xác nhận và thông tin lịch đang áp dụng, được ghi là SH-01.

Đối với nhân viên điều phối, nhu cầu là biết ca làm và khả năng còn nhận được để quyết định nhận lịch. Dự án đang cân nhắc một nơi theo dõi lịch, hàng yêu cầu chờ xử lý và bước kiểm tra lại trước khi xác nhận. Nhu cầu và hướng giải pháp này lần lượt là N02 và SH-02. Cần kiểm tra liệu cách mới thay thế được công việc hiện tại hay chỉ tạo thêm một nguồn phải duy trì.

Khi có thay đổi, cả người đặt và nhân viên cần biết ai xử lý, kết quả nào đang có hiệu lực và người liên quan đã được báo tới đâu. Hướng đang cân nhắc là ghi nhận đề nghị đổi riêng với lịch hiện hành, theo dõi lịch sử và công việc liên hệ. Đây là nhu cầu N03 và hướng giải pháp SH-03.

Việc đặt hộ và tiếp nhận tại quầy cần phân biệt người đặt với người khám, đồng thời xem xét người đến trực tiếp trong cùng khả năng tiếp nhận của cơ sở. Nhu cầu N04 được nối với hướng giải pháp SH-04: ghi thông tin người khám riêng và hỗ trợ đối chiếu tại quầy.

Bác sĩ cần có cách báo thay đổi khả năng làm việc để người điều phối xử lý các lượt liên quan. Nhu cầu N05 thuộc hướng xử lý thay đổi SH-03. Chưa có căn cứ bắt buộc phải làm một giao diện bác sĩ riêng nếu trao đổi qua lễ tân đã đáp ứng công việc.

Các nhu cầu này vẫn là giả thuyết. Chi tiết về người dùng nằm trong [User Personas](./user-personas.md), các bước tương tác nằm trong [Journey Map](./customer-journey-map.md), còn quan hệ giữa vấn đề và hướng giải pháp được tổng hợp trong [Lean Canvas](./lean-canvas-v2.md).

## 5. Những điều rút ra từ nguồn công khai

**R01 — Thị trường đã có công cụ cho phía phòng khám.** BookingCare DX, YouMed HCP, Nano Smart Clinic và KiotViet có công bố khả năng phục vụ cơ sở y tế; Medpro Clinic là ứng viên còn hạn chế về xác minh (S03, S06, S08, S10–S12). Vì vậy, chỉ có web đặt khám hoặc nhắc hẹn chưa đủ làm lý do tồn tại của Healthcare Portal. Mức đáp ứng và chất lượng sử dụng tại phân khúc mục tiêu vẫn chưa biết.

**R02 — Quy trình và chính sách phụ thuộc bối cảnh.** Các nguồn S01, S04, S07 và S13 mô tả điều kiện xác nhận, thanh toán và đổi/hủy khác nhau hoặc chưa đầy đủ. Dự án cần chọn cơ sở và hiểu chính sách cụ thể trước khi mô hình hóa; không thể ghép các nguồn thành một quy trình chuẩn chung.

**R03 — Giờ hẹn không luôn là giờ bắt đầu khám.** BookingCare nêu thời điểm thực tế có thể lệch giờ hẹn (S02). Điều này cho thấy cần nghiên cứu người đặt hiểu thời gian ra sao, nhưng chưa cho biết mức chờ hay nguyên nhân ở cơ sở mục tiêu và cũng chưa chứng minh portal có thể cải thiện chúng.

**R04 — Có căn cứ để nghiên cứu bàn giao giữa các kênh.** Hướng dẫn tại Bình An có nhiều kênh tiếp cận (S14), còn tài liệu KiotViet mô tả tác vụ nhân viên (S11). Đây là lý do để tìm hiểu nơi đọc, ghi và chuyển thông tin; sự tồn tại nhiều kênh chưa chứng minh nhân viên đang nhập trùng hoặc cách mới sẽ giảm việc.

**R05 — Cần phân biệt người đặt và người khám.** Luồng chọn người khám/gia đình trong S13 cho thấy đây là một bối cảnh có thật ở dịch vụ tham chiếu. Tần suất đặt hộ, mức thành thạo và nhu cầu hỗ trợ tại cơ sở mục tiêu vẫn cần nghiên cứu trực tiếp.

**R06 — Nguồn có giới hạn về thời điểm, phạm vi và chất lượng.** Một số nguồn có mốc thời gian, điều khoản hoặc nội dung tiếp thị chưa nhất quán; S06 chỉ đọc được đầy đủ qua chỉ mục (S04, S06, S07, S09, S12–S14). Vì vậy, giá, khả năng tích hợp và cam kết hiệu quả phải được kiểm tra theo sản phẩm và thời điểm sử dụng. Lỗi truy cập không chứng minh sản phẩm không tồn tại; nội dung quảng cáo không phải kết quả thực nghiệm.

## 6. Những việc cần làm tiếp

1. **Xác nhận vấn đề có đáng ưu tiên.** Trước hết, cần biết vấn đề lịch hẹn có đủ quan trọng để người dùng thay đổi cách làm hay không. Đây là giả định VAL-01, hiện có mức tin tưởng thấp và rủi ro cao nếu dự án tiếp tục đầu tư dựa trên một vấn đề chưa rõ. Bằng chứng cần là tình huống cụ thể, hậu quả, cách khắc phục và hành vi giữ hoặc đổi công cụ. Chỉ có lời khen về ý tưởng hoặc mô tả tính năng chưa đủ xác nhận nhu cầu.

2. **Kiểm tra công việc của lễ tân.** Tiếp theo, cần kiểm tra cách phối hợp mới có làm tăng việc cho lễ tân không. Với giả định USE-03, nên lập lại công việc đọc, ghi và bàn giao trong một ca thực tế, sau đó so tình huống tương đương khi thử giải pháp. Nếu nhân viên vẫn phải nhập hai nơi hoặc duy trì công cụ cũ mà chưa có lý do thỏa đáng, phải sửa phương án trước khi nói rằng sản phẩm giảm tải.

3. **Kiểm tra quy tắc và ngoại lệ.** Giả định thứ ba là có thể mô tả quy tắc lịch và ngoại lệ một cách nhất quán, mang mã FEA-01. Nguồn hiện tại mới hỗ trợ việc nhận diện câu hỏi và biến cần làm rõ. Cần người vận hành rà chính sách, kiểm tra chéo các tình huống và thực hiện kiểm chứng kỹ thuật ở bước phù hợp. Mô hình tự nhất quán chưa đồng nghĩa phần mềm đã xử lý đúng các thao tác đồng thời.

Cả ba giả định đều có tác động và rủi ro cao theo đánh giá định tính. Mức tin tưởng trung bình của FEA-01 chỉ nói về việc đã nhận diện một phần quy tắc, không phải xác nhận khả thi toàn bộ. Không có dữ liệu để tính điểm ưu tiên; công sức được hiểu là phần có thể phải làm lại khi dựa trên giả định sai.

Song song với ba việc này, cần chọn cơ sở và phân khúc cụ thể, xác định người quyết định dùng và chi trả, tìm hiểu dữ liệu, nguồn lực, chi phí và hỗ trợ. Dùng [Interview Guide](../03-interview-guide.md) để hỏi trải nghiệm đã xảy ra và [phép đo trong Canvas](./lean-canvas-v2.md) để chuẩn bị đánh giá giải pháp. Nếu công cụ hiện tại đáp ứng tốt và không có đánh đổi đáng kể, dự án cần điều chỉnh vấn đề hoặc định vị.

<a id="trang-thai-gia-dinh"></a>

## 7. Phụ lục tra cứu trạng thái giả định

Phần diễn giải trên tập trung vào những điều quan trọng để đọc như một báo cáo. Bảng dưới giữ đủ 24 mã để đối chiếu với [Assumptions](../01-assumptions.md) và [Prioritized Assumptions](../02-prioritized-assumptions.md). Đây là trạng thái sau nghiên cứu tài liệu ngày 21/11/2026; chưa có giả định nào được xác thực hoặc bác bỏ toàn bộ.

| Mã | Trạng thái | Căn cứ hoặc phần còn thiếu |
|---|---|---|
| VAL-01 | **Chưa đủ** | Nguồn quy trình không chứng minh mức ảnh hưởng/động lực đổi cách làm; R02–R04 |
| VAL-02 | Chưa đủ; chưa cam kết mở rộng phân hệ | Pain points nhập vai vẫn không phải thực địa |
| VAL-03 | Chưa đủ | Có công bố nhắc hẹn, không có nguyên nhân no-show hoặc thử tác động |
| USE-01 | Chưa đủ | Hướng dẫn thao tác không chứng minh người mục tiêu tự hoàn thành |
| USE-02 | Chưa đủ; hoãn | Không nghiên cứu tác vụ kê đơn/phím tắt |
| USE-03 | **Chưa đủ** | Có tác vụ nhân viên và nhiều kênh, chưa có tải ca làm hoặc đối chiếu trước/sau |
| VIA-01 | Chưa đủ; cần nghiên cứu sớm | Chưa xác định người quyết định/chi trả, ngân sách và điều kiện mua/sử dụng |
| VIA-02 | Chưa đủ; cần nghiên cứu sớm | Chưa đánh giá chi phí tiếp nhận, hỗ trợ và vận hành bền vững |
| VIA-03 | Chưa đủ; cần xử lý trước pilot | Chưa đánh giá điều kiện dữ liệu/nghiệp vụ hoặc sẵn sàng dùng thật |
| FEA-01 | **Hỗ trợ một phần về nhận diện quy tắc; chưa xác thực** | R02 giúp tìm biến/ngoại lệ; chưa có quy tắc thống nhất, kiểm tra chéo hay thử đồng thời |
| FEA-02 | Chưa đủ; đánh giá trước cam kết tích hợp | Không thử API/tài khoản/dịch vụ; S06 không đủ chứng minh liên thông |
| FEA-03 | Chưa đủ; đánh giá trước nhập dữ liệu nếu chọn | Không có bộ dữ liệu nguồn thực tế để đánh giá chuẩn hóa |
| ETH-01 | Hỗ trợ trong phạm vi desk research này | Đã nghiên cứu quy trình bằng tài liệu công khai mà không cần hồ sơ bệnh nhân; chưa suy ra mọi nghiên cứu sau đều đã có quy trình dữ liệu phù hợp |
| ETH-02 | Chưa đủ; hoãn | Không thử AI tư vấn hoặc mẫu kê đơn |
| ETH-03 | Có căn cứ nghiên cứu, chưa xác thực bao phủ | Có luồng đặt hộ/kênh hỗ trợ; chưa biết người khó dùng công nghệ có được phục vụ phù hợp |
| GTM-01 | Chưa đủ | Chưa có người tham gia/đầu mối xác nhận; tìm được trang web không phải tiếp cận người dùng |
| GTM-02 | Chưa đủ; cần nghiên cứu sớm | Chưa có bằng chứng chuyển đổi hoặc tiếp tục sử dụng; lời khen không phải cam kết |
| GTM-03 | Chưa đủ | Có bối cảnh tham chiếu, chưa xác nhận phân khúc/kênh hiệu quả cho nhóm |
| STR-01 | Có định hướng dự án; giả định chưa xác thực | Chủ dự án yêu cầu phát triển sản phẩm thực tế, trọng tâm lịch hẹn; chưa có quyết định phạm vi dựa trên dữ liệu người dùng và phân công đầy đủ |
| STR-02 | Chưa xác thực khoảng trống; cần sửa lập luận | R01 phản bác lập luận thiếu tính năng đơn giản, không bác bỏ mọi nhu cầu chưa được đáp ứng |
| STR-03 | Hỗ trợ ở mức định nghĩa cách đo | Canvas v2 có khung đo kế thừa; chưa baseline, thử nghiệm hoặc KPI duyệt |
| TEAM-01 | Chưa đủ | Chưa có kế hoạch năng lực, thời lượng, ngân sách và mốc dự án |
| TEAM-02 | Chưa đủ | Cần xác định chủ quyết định sản phẩm, người rà nghiệp vụ và trách nhiệm vận hành |
| TEAM-03 | Có minh họa truy vết trong bộ này; chưa xác thực cả nhóm | Skill và nguồn được ghi, chưa quan sát các thành viên kiểm tra/giải thích |
