# Healthcare Portal — Kịch bản phỏng vấn nghiên cứu người dùng

Ngày lập: 17/11/2026; cập nhật định hướng: 21/11/2026, múi giờ Asia/Saigon. Trạng thái: hướng dẫn chuẩn bị, chưa thực hiện phỏng vấn và chưa có câu trả lời.

## 1. Skill, đầu vào và mục tiêu

- Skill áp dụng: `interview-script`.
- File gốc: `.agents/skills/interview-script/SKILL.md`.
- Repository: https://github.com/phuryn/pm-skills/blob/main/pm-product-discovery/skills/interview-script/SKILL.md.
- Đã đọc: [01-assumptions.md](./01-assumptions.md) và [02-prioritized-assumptions.md](./02-prioritized-assumptions.md).
- Bối cảnh: nghiên cứu nhu cầu và điều kiện vận hành Healthcare Portal như một sản phẩm thực tế. Tài liệu ý tưởng và các cuộc phỏng vấn AI nhập vai không phải dữ liệu khách hàng.

Áp dụng cách hỏi theo hành vi đã xảy ra, khơi lại một sự việc cụ thể và tìm công việc người tham gia cần hoàn thành (Jobs to Be Done). Không giới thiệu giải pháp, không hỏi có muốn dùng app, không tạo câu trả lời giả.

### Liên kết mục tiêu với ba giả định ưu tiên

| Giả định | Mục tiêu phỏng vấn | Quyết định nghiên cứu được hỗ trợ | Giới hạn |
|---|---|---|---|
| **VAL-01** — Lịch hẹn là vấn đề đủ quan trọng | Tìm sự việc cụ thể, hậu quả, cách xử lý và lý do giữ/đổi cách làm | Điều chỉnh vấn đề và giá trị trong Vision/Canvas | Có khó khăn chưa chứng minh họ sẽ đổi sang sản phẩm của nhóm; một cuộc phỏng vấn không đại diện thị trường |
| **USE-03** — Quy trình chung không tăng việc cho lễ tân | Làm rõ công cụ, bước đọc/ghi/nhập lại, bàn giao và nguồn lịch được tin cậy | Mô tả hiện trạng và điều kiện cần cho hướng phối hợp lịch | Phỏng vấn chỉ cung cấp hiện trạng được kể lại, chưa chứng minh quy trình mới giảm tải |
| **FEA-01** — Quy tắc lịch và ngoại lệ có thể mô tả nhất quán | Tìm hiểu cách xác nhận, đổi/hủy, xử lý công suất và thay đổi lịch qua sự việc thật | Lập và kiểm tra bộ quy tắc cho bối cảnh thử nghiệm sau nghiên cứu | Không chứng minh khả năng chống trùng lịch đồng thời của phần mềm |

Giữ cả tình huống diễn ra thuận lợi và thông tin phản bác giả định. Chưa đặt ngưỡng tỷ lệ xác thực, không tìm người để chỉ đồng ý với ý tưởng.

## 2. Nhóm người đề xuất và cách chọn

| Nhóm | Điều kiện phù hợp | Lý do chọn | Phần không nên yêu cầu họ suy đoán |
|---|---|---|---|
| A1. Lễ tân/người trực tiếp tiếp nhận | Đã trực tiếp nhận, xác nhận hoặc cập nhật lịch ở cơ sở thuộc bối cảnh nghiên cứu; có thể kể một trường hợp họ đã xử lý | Nắm thao tác, kênh liên hệ, cập nhật và ngoại lệ; phù hợp USE-03, FEA-01 và VAL-01 | Không mặc định họ quyết định chính sách hoặc có quyền mua phần mềm |
| A2. Người quản lý phòng khám | Đã trực tiếp điều phối hoặc quyết định quy tắc lịch; nêu được trường hợp đã tham gia | Làm rõ quyền hạn, công suất, thay đổi ca và lý do chọn công cụ | Nếu chỉ biết báo cáo, tách lời tổng thuật khỏi trải nghiệm trực tiếp; cần bổ sung người thực hiện khi có thể |
| B1. Người đã tự đặt lịch/đặt hộ | Có trải nghiệm thực tế có thể nhớ lại; ghi rõ ai đặt, ai đi khám và loại cơ sở | Hiểu mục tiêu, kênh sử dụng, xác nhận và thay đổi từ phía người đặt | Không suy đoán công việc nội bộ của nhân viên |
| B2. Người đã đi khám nhưng không đặt trước | Có thể kể lần đến trực tiếp và cách được tiếp nhận | Tìm lý do chọn kênh này và phối hợp khách trực tiếp; tránh chỉ tuyển người đã dùng web | Không giả định họ đã trải qua đặt/xác nhận trực tuyến |

Ưu tiên bối cảnh phòng khám tư nhân phù hợp hướng đang nghiên cứu. Nếu người tham gia chỉ có trải nghiệm bệnh viện hoặc bối cảnh khác, ghi khác biệt và giới hạn áp dụng; không gộp thành cùng một hiện trạng.

Không đặt số mẫu đại diện trong tài liệu này vì chưa có kế hoạch tuyển người. Nếu tiếp cận được nhiều người, tìm sự khác biệt về công cụ/cách đặt và trường hợp có/không gặp khó khăn, không tuyển chỉ vì họ phàn nàn. Không suy ra năng lực dùng công nghệ chỉ từ tuổi.

Chưa liên hệ, mời hoặc gửi tin cho người tham gia. Bạn bè/người trong nhóm chỉ được xem là người dùng thật khi có trải nghiệm phù hợp và đang kể trải nghiệm đó; buổi tập đóng vai phải ghi **diễn tập**, không nhập vào bằng chứng phỏng vấn thực tế.

## 3. Chuẩn bị và cách điều phối

- Đề xuất mỗi buổi có một người hỏi và một người ghi; thông báo rõ ai có mặt, giữ số người tham dự phù hợp để người tham gia thoải mái kể chuyện.
- Gán mã khi có người thực sự tham gia: `PK-###` cho nhóm phòng khám, `ND-###` cho nhóm người đi/đặt khám. Đây là quy ước mã, không phải danh sách người đã được tuyển.
- Hai lịch trình bên dưới dài khoảng **25 phút**, có thể co giãn trong **20–30 phút**. Khi chỉ có 20 phút, bớt câu đào sâu và nhánh ngoại lệ; giữ mở đầu, một câu chuyện chính và kết thúc. Chỉ dùng phần mở rộng nếu còn thời gian, không hỏi hết mọi nhánh.
- Hỏi câu chính trước, chỉ hỏi đào sâu khi người tham gia chưa nói rõ. Để họ kể phần lớn thời gian; không đọc liên tục cả bảng như khảo sát.
- Khi người tham gia nói quy tắc chung, hỏi ví dụ họ từng xử lý; nếu không nhớ thì ghi “chưa có ví dụ”, không yêu cầu bịa tình huống.
- Không cần bệnh án, chẩn đoán, tên/số điện thoại bệnh nhân hoặc ảnh màn hình chứa dữ liệu nhận diện. Chỉ ghi phần quy trình cần nghiên cứu. Không yêu cầu họ đăng nhập hoặc thực hiện lịch khám thật.

### Lời mở đầu dùng cho cả hai kịch bản — khoảng 3 phút

> Chúng tôi đang nghiên cứu sản phẩm Healthcare Portal để hỗ trợ đặt và điều phối lịch khám. Hôm nay chúng tôi muốn nghe trải nghiệm thực tế của anh/chị, gồm cả những việc thuận lợi và chưa thuận lợi. Mục đích buổi này là hiểu cách làm hiện tại, không giới thiệu hay bán sản phẩm.
>
> Cuộc trao đổi dự kiến khoảng 25 phút. Không có câu trả lời đúng hoặc sai; anh/chị có thể bỏ qua câu hỏi hoặc dừng bất cứ lúc nào. Anh/chị không cần chia sẻ bệnh lý, tên người bệnh hay thông tin riêng tư. Thời lượng này có phù hợp và anh/chị có đồng ý tham gia không ạ?

Chờ trả lời trước khi hỏi tiếp. Nếu không đồng ý, cảm ơn và kết thúc; không tự ghi đồng ý trong mẫu.

**Nếu chỉ ghi chép:** nói rõ dùng mã người tham gia trong bản tổng hợp và xin phép ghi chép.

**Nếu muốn ghi âm:** trước buổi phỏng vấn, nhóm phải điền người được truy cập, nơi lưu và mốc xóa; chưa dùng các chỗ trống như cam kết đã hoàn tất.

> Để ghi lại chính xác, anh/chị có đồng ý cho chúng tôi ghi âm không? Bản ghi được dùng để tổng hợp nghiên cứu sản phẩm, được lưu tại [nơi lưu nhóm đã xác định], chỉ [người được truy cập] được đọc/nghe và dự kiến xóa vào [mốc đã xác định]. Trong bản tổng hợp chúng tôi dùng mã người tham gia. Nếu anh/chị không muốn ghi âm, chúng tôi có thể chỉ ghi chép.

Không bật ghi âm trước khi được đồng ý. Nếu không có sự đồng ý phù hợp cho ghi chép/ghi âm, kết thúc buổi trao đổi. Không hứa “ẩn danh hoàn toàn” vì giọng nói hoặc bối cảnh vẫn có thể nhận diện; bản tổng hợp chỉ đưa nội dung cần thiết đã loại nhận diện.

## 4. Kịch bản A — Lễ tân hoặc người quản lý phòng khám

### Lịch trình 25 phút đề xuất

| Phần | Thời lượng | Câu hỏi |
|---|---|---|
| Mở đầu và đồng ý | 3 phút | Lời mở đầu chung |
| Bối cảnh/vai trò | 3 phút | A01 |
| Một lịch hẹn cụ thể | 7 phút | A02–A03 |
| Công việc phối hợp và tác động | 5 phút | A04–A05 |
| Ngoại lệ và quy tắc | 4 phút | A06–A07, chọn nhánh phù hợp |
| Kết thúc | 3 phút | A08–A09 |

### Câu hỏi chính và đào sâu

| Mã | Câu hỏi chính | Đào sâu khi cần | Giả định / bằng chứng muốn tìm |
|---|---|---|---|
| **A01** | Anh/chị phụ trách những việc gì liên quan đến lịch khám? Trong ca làm gần nhất, anh/chị trực tiếp xử lý phần nào? | Những việc nào do người khác làm? Anh/chị đang kể từ trải nghiệm trực tiếp hay thông tin được báo lại? Không cần nêu tên cơ sở/người bệnh | USE-03, FEA-01: vai trò và giới hạn hiểu biết của người trả lời |
| **A02** | Anh/chị có thể kể lần gần nhất mình nhận và xử lý một yêu cầu hẹn khám, từ lúc nhận yêu cầu đến khi kết thúc việc xử lý không? | Yêu cầu đến từ đâu? Anh/chị xem thông tin nào trước? Sau đó làm gì? Dùng công cụ gì? Ai khác tham gia? Nếu ca đó chưa kết thúc, dừng ở bước đã thực sự xảy ra | VAL-01, USE-03, FEA-01: chuỗi hành động của một sự việc cụ thể |
| **A03** | Trong lần đó, lúc nào anh/chị coi lịch đã được xác nhận, và người đặt biết điều đó bằng cách nào? | Ai quyết định? Căn cứ nào cho biết còn khả năng tiếp nhận? Giờ hẹn khi đó được hiểu là giờ đến hay giờ bắt đầu khám? Nếu phải chờ duyệt, việc gì đã xảy ra trong lúc chờ? | FEA-01: ý nghĩa trạng thái, thời điểm, quyền hạn và công suất |
| **A04** | Với yêu cầu vừa kể, anh/chị đã đọc hoặc ghi thông tin ở những đâu, và bàn giao cho ai? | Có thông tin nào phải ghi lại ở chỗ khác không? Nếu có: nội dung nào, vì sao? Khi dữ liệu khác nhau, lần đó anh/chị dựa vào đâu để xử lý? Nếu chỉ dùng một nơi, hỏi cách họ giữ thông tin cập nhật | USE-03: công cụ, nguồn dữ liệu, việc nhập lại; không mặc định có nhập trùng |
| **A05** | Trong lần đó, phần nào thuận lợi và phần nào cần anh/chị xử lý thêm? | Nếu có việc phát sinh: việc cụ thể là gì, tác động tới ai, xử lý ra sao? Thời gian nếu nhớ được thì khoảng bao lâu, dựa vào trí nhớ hay có ghi nhận? Trước đây anh/chị đã làm gì để cải thiện và kết quả lần đó ra sao? Nếu không có khó khăn, hỏi điều gì giúp công việc thuận lợi | VAL-01, USE-03: ảnh hưởng, đánh đổi, cách khắc phục và bằng chứng phản bác |
| **A06** | Anh/chị có nhớ lần gần nhất một lịch đã tiếp nhận cần thay đổi hoặc không diễn ra như dự kiến không? Nếu có, chuyện bắt đầu như thế nào? | Chọn tình huống họ đã gặp: ai báo, ai sửa, sửa ở đâu, ai được thông báo, lịch cũ được ghi nhận thế nào, cuối cùng kết thúc ra sao? Nếu không có/không nhớ, bỏ nhánh | FEA-01, USE-03, VAL-01: ngoại lệ có thật, trách nhiệm và thao tác phát sinh |
| **A07** | Trong những ca anh/chị đã làm, các yêu cầu hẹn trước và người đến trực tiếp đã được tiếp nhận như thế nào? | Xin một ví dụ thật nếu có; ai quyết định lượt/công suất? Nếu họ tự kể hai yêu cầu cùng giờ, bác sĩ đổi ca, khách đến muộn hoặc đặt hộ, hỏi điều kiện trước/sau và kết quả. Không hỏi giả định “nếu xảy ra thì anh/chị sẽ…” | FEA-01, USE-03: phối hợp và quy tắc trong ca thực tế; ghi không áp dụng nếu cơ sở không có nhóm khách đó |
| **A08** | Với công việc anh/chị vừa kể, lần nào anh/chị thấy việc xử lý lịch diễn ra tốt? Điều gì cho anh/chị biết là tốt? | So với tình huống trước có gì khác? Có cách làm nào anh/chị đã thử rồi giữ lại hoặc bỏ đi? Căn cứ nào khiến anh/chị quyết định như vậy? | VAL-01, USE-03: kết quả mong muốn bằng ngôn ngữ người dùng, hành vi lựa chọn công cụ/quy trình |
| **A09** | Có điều quan trọng nào về xử lý lịch chúng tôi chưa hỏi không? Phần nào cần trao đổi với người trực tiếp làm để hiểu đúng hơn? | Có thể xin gợi ý vai trò, không cần thông tin liên hệ người khác. Nếu cần hỏi lại, xin phép về cách liên hệ riêng. Cảm ơn và kết thúc đúng giờ | Xác định giới hạn của VAL-01, USE-03, FEA-01; không coi gợi ý liên hệ là người đã đồng ý tham gia |

**Điều chỉnh cho người quản lý:** giữ cùng kịch bản nhưng ưu tiên trường hợp họ trực tiếp tham gia. Nếu mô tả chính sách, hỏi chính sách được áp dụng thế nào trong một ca đã xảy ra; ghi rõ “quy định được kể lại” khác “cách làm đã trực tiếp thực hiện”. Nếu người tham gia có quyền quyết định sử dụng/chi trả, dùng nhánh mở rộng bên dưới để hiểu hành vi lựa chọn và chi phí thực tế; không biến phỏng vấn thành chào bán.

### Nhánh mở rộng — Người quyết định sử dụng hoặc chi trả

Dành một buổi riêng hoặc thống nhất thêm thời gian; không ép vào lịch trình 25 phút. Không mặc định lễ tân hoặc bác sĩ là người mua.

| Câu hỏi về hành vi đã xảy ra | Bằng chứng cần tìm |
|---|---|
| Lần gần nhất cơ sở lựa chọn hoặc thay đổi công cụ quản lý lịch diễn ra thế nào? | Ai đề xuất, đánh giá, quyết định và phê duyệt ngân sách; VIA-01, GTM-02 |
| Khi đó cơ sở đã cân nhắc những lựa chọn nào và vì sao giữ hoặc loại từng lựa chọn? | Giải pháp thay thế, điều kiện chuyển đổi, lý do từ chối; STR-02 |
| Việc triển khai phát sinh những công việc và chi phí nào? Nếu có thể chia sẻ, khoản nào đã thực chi? | Đào tạo, nhập dữ liệu, hạ tầng, hỗ trợ và người chịu chi phí; VIA-01/02 |
| Sau khi bắt đầu dùng, điều gì khiến cơ sở tiếp tục hoặc ngừng dùng? | Hành vi duy trì, chi phí phục vụ và ảnh hưởng vận hành; GTM-02 |
| Ai đã xử lý khi công cụ gặp sự cố hoặc nhân viên cần hỗ trợ? | Trách nhiệm, thời gian gián đoạn, phương án dự phòng; VIA-02/03 |

Ghi rõ khoản chi là báo cáo từ trí nhớ hay có tài liệu được phép xem. Phỏng vấn này chưa xác nhận khả năng mua Healthcare Portal; cần kiểm chứng đề xuất giá trị và điều kiện thử riêng.

## 5. Kịch bản B — Người từng đặt lịch hoặc đi khám

### Lịch trình 25 phút đề xuất

| Phần | Thời lượng | Câu hỏi |
|---|---|---|
| Mở đầu và đồng ý | 3 phút | Lời mở đầu chung |
| Bối cảnh trải nghiệm | 3 phút | B01 |
| Một lần đặt/đi khám cụ thể | 7 phút | B02–B03 |
| Thay đổi hoặc tiếp nhận | 5 phút | B04–B05, chọn nhánh phù hợp |
| Tác động và cách đã lựa chọn | 4 phút | B06–B07 |
| Kết thúc | 3 phút | B08–B09 |

### Câu hỏi chính và đào sâu

| Mã | Câu hỏi chính | Đào sâu khi cần | Giả định / bằng chứng muốn tìm |
|---|---|---|---|
| **B01** | Anh/chị có thể chọn một lần đặt lịch hoặc đi khám mà mình còn nhớ rõ để kể không? Lần đó anh/chị tự làm, nhờ người khác hay đặt cho người thân? | Khoảng khi nào, loại cơ sở nào? Không cần tên cơ sở, bệnh lý, ngày khám chính xác hoặc danh tính người thân. Ai là người thực hiện từng phần? | VAL-01, FEA-01: bối cảnh và phân biệt người đặt/người khám |
| **B02** | Từ lúc quyết định đi khám đến khi biết cách đến khám, anh/chị đã làm những gì trong lần đó? | Chuyện gì diễn ra trước, rồi tiếp theo? Tìm thông tin ở đâu? Vì sao đã dùng kênh đó? Ai đã hỗ trợ? Nếu đến trực tiếp không hẹn trước, hỏi cách họ quyết định và được tiếp nhận; không ép kể trải nghiệm đặt lịch chưa có | VAL-01: hành trình thật và cách giải quyết hiện có; USE-03 chỉ tham khảo phần tiếp xúc với nhân viên |
| **B03** | Sau khi liên hệ hoặc gửi yêu cầu lần đó, anh/chị nhận được thông tin gì và dựa vào đâu để biết bước tiếp theo? | Nếu có lịch hẹn: ai xác nhận, qua đâu, giờ hẹn được hiểu thế nào? Nếu chưa rõ, anh/chị đã làm gì? Nếu không đặt trước, hỏi họ biết thời gian/lượt tiếp nhận bằng cách nào | VAL-01, FEA-01: bằng chứng xác nhận, ý nghĩa thời gian, mức hiểu đúng trạng thái từ phía người đặt |
| **B04** | Lần đó việc sắp xếp có thay đổi gì so với dự định ban đầu không? | Nếu có: ai biết trước, đã liên hệ thế nào, phản hồi gì, sau đó làm gì? Nếu không có thay đổi, không giả định đã gặp lỗi; nếu còn thời gian, hỏi một lần đổi/hủy khác mà họ thực sự nhớ | FEA-01, VAL-01: thay đổi, hủy và hậu quả có thật |
| **B05** | Nếu lần đó anh/chị đã đến cơ sở, từ khi đến đến lúc được tiếp nhận đã diễn ra thế nào? | Họ được hỏi/xác nhận thông tin gì? Có phải liên hệ lại không? Điều gì họ trực tiếp thấy hoặc được nhân viên nói? Nếu chưa đến hoặc đã hủy, hỏi đoạn kết thực tế rồi bỏ nhánh tiếp nhận | VAL-01, FEA-01; USE-03 chỉ cung cấp phần bàn giao nhìn thấy từ phía người bệnh, không xác nhận công việc nội bộ |
| **B06** | Trong trải nghiệm vừa kể, phần nào thuận lợi và phần nào làm anh/chị phải xử lý thêm? | Nếu có phát sinh: anh/chị làm gì, ảnh hưởng lịch cá nhân ra sao, đã nhờ ai? Có khoảng thời gian hoặc khoản chi thực tế nào họ nhớ không? Không gợi sẵn con số; phân biệt ước lượng với ghi nhận. Nếu không có vướng mắc, hỏi điều gì đã hoạt động tốt | VAL-01: mức ảnh hưởng và đánh đổi theo lời kể, gồm cả trường hợp không có pain point |
| **B07** | Trước lần đó, anh/chị từng chọn cách đặt hoặc đến khám khác chưa? Điều gì xảy ra trong lần khiến anh/chị giữ hoặc đổi cách làm? | Nếu có, xin một ví dụ và kết quả thực tế. Nếu chưa, ghi nhận chưa đổi, không hỏi họ có muốn chuyển sang ứng dụng mới | VAL-01: hành vi thay đổi, lý do giữ kênh hiện tại; không suy ra sẵn sàng mua/dùng sản phẩm nhóm |
| **B08** | Sau lần vừa kể, điều gì khiến anh/chị đánh giá việc sắp xếp khám là ổn hoặc chưa ổn? | Dấu hiệu cụ thể là gì? Có điều nào trước buổi trao đổi chúng tôi chưa hiểu đúng về câu chuyện không? | VAL-01, FEA-01: kết quả mong muốn, xác nhận lại cách hiểu của người hỏi |
| **B09** | Có điều gì về trải nghiệm đó mà chúng tôi chưa hỏi không? | Nếu cần bổ sung sau, xin phép hỏi lại qua cách họ đồng ý. Không xin giới thiệu danh tính người bệnh khác. Cảm ơn và kết thúc | Giới hạn và phần còn thiếu của VAL-01/FEA-01; không mở rộng sang giới thiệu giải pháp |

**Phân nhánh bắt buộc:** người chỉ đến khám trực tiếp vẫn là nguồn hợp lệ về tiếp nhận và lý do không đặt trước. Các mục đặt/xác nhận/đổi lịch không xảy ra phải ghi “không áp dụng” hoặc “chưa có trải nghiệm”, không điền bằng giả định. Người đặt hộ chỉ kể những phần họ trực tiếp biết.

## 6. Cách đào sâu và tránh dẫn dắt

Có thể dùng: “Anh/chị kể thêm đoạn đó được không?”, “Sau đó chuyện gì xảy ra?”, “Anh/chị biết điều đó từ đâu?”, “Có ví dụ cụ thể anh/chị nhớ không?”, “Điều gì khiến anh/chị chọn cách đó lúc ấy?”. Hỏi lần lượt, không ép người tham gia nhớ chính xác nếu họ không chắc.

| Tránh hỏi | Thay bằng câu trung tính |
|---|---|
| “Có phải dùng Excel nên hay trùng lịch không?” | “Trong ca vừa kể, anh/chị quản lý thông tin ở đâu? Việc tiếp nhận diễn ra thế nào?” |
| “Một ứng dụng tập trung sẽ giúp anh/chị đỡ việc đúng không?” | “Với yêu cầu đó, anh/chị đã đọc, ghi hoặc chuyển thông tin ở những đâu?” |
| “Anh/chị có muốn dùng ứng dụng của nhóm không?” | “Lần gần nhất anh/chị đổi cách sắp xếp lịch, điều gì đã xảy ra và kết quả ra sao?” |
| “Bệnh nhân thường chờ lâu lắm đúng không?” | “Trong lần anh/chị vừa kể, từ khi đến tới lúc được tiếp nhận diễn ra thế nào?” |

Nếu người tham gia hỏi về giải pháp, ghi nhận và giải thích nhóm đang tìm hiểu trải nghiệm trước; không giới thiệu tính năng để lấy phản hồi trong phần phỏng vấn này. Lời khen ý tưởng không được ghi như bằng chứng nhu cầu.

## 7. Mẫu ghi chép cho từng cuộc phỏng vấn

Mẫu dưới đây để trống; không phải dữ liệu một người tham gia. Chỉ tạo bản ghi thực tế sau khi người đó đồng ý tham gia. Mã không chứa tên, số điện thoại hay ngày sinh.

### 7.1. Thông tin buổi trao đổi

| Trường | Nội dung điền sau |
|---|---|
| Mã người tham gia | [PK-### hoặc ND-###, chưa gán] |
| Ngày/giờ, múi giờ | [Chưa có] |
| Người hỏi / người ghi | [Chưa phân công] |
| Thời lượng thực tế | [Chưa diễn ra] |
| Loại buổi | [Phỏng vấn trải nghiệm thật / diễn tập — không trộn hai loại] |
| Vai trò, loại cơ sở, trải nghiệm liên quan | [Chưa có, không ghi danh tính không cần thiết] |
| Đồng ý tham gia / ghi chép | [Chưa xin; ghi câu trả lời thực tế] |
| Đồng ý ghi âm | [Chưa xin / có / không / không đề nghị] |
| Người truy cập, nơi lưu, mốc xóa nếu có ghi âm | [Chưa xác định; cần xác định trước khi xin ghi âm] |
| Nguồn lời kể | [Trực tiếp làm/trải qua / nghe kể / không rõ; ghi theo từng ý nếu khác nhau] |

### 7.2. Nhật ký bằng chứng theo câu hỏi

| Câu hỏi | Giả định | Trích nguyên văn hoặc lời kể tóm tắt, ghi rõ loại | Sự việc/hành động và công cụ | Tác động/kết quả, gồm cả thuận lợi | Vị trí nguồn/thời điểm trong bản ghi | Điều chưa rõ hoặc trái giả định |
|---|---|---|---|---|---|---|
| [Chưa hỏi] | [Chưa gán] | [Chưa có dữ liệu] | [Chưa có] | [Chưa có] | [Chưa có] | [Chưa có] |

Chỉ dùng dấu ngoặc kép cho câu chép chính xác và được phép sử dụng. Lời diễn giải của người ghi phải ghi “tóm tắt lời kể”. Gắn nhãn phân biệt: **lời kể**, **quan sát trực tiếp**, **quy định được mô tả**, **suy luận nhóm**. Nếu không có bản ghi, trỏ tới mã câu hỏi/đoạn ghi chú; không tạo mốc thời gian giả.

### 7.3. Bảng luồng hiện trạng — chỉ điền bước có căn cứ

| Tình huống | Bước | Ai thực hiện | Nguồn thông tin đọc/ghi | Có ghi lại/bàn giao ở nơi khác? | Trạng thái trước/sau theo cách người tham gia gọi | Căn cứ câu hỏi/nguồn | Chưa rõ |
|---|---|---|---|---|---|---|---|
| [Chưa có] | [Chưa có] | [Chưa có] | [Chưa có] | [Chưa xác định] | [Chưa có] | [Chưa có] | [Chưa có] |

Không tự đổi thuật ngữ người dùng thành các trạng thái PENDING/CONFIRMED của Word khi chưa đối chiếu ý nghĩa.

### 7.4. Tổng hợp công việc và phát hiện

| Nội dung | Ghi nhận sau buổi phỏng vấn |
|---|---|
| Công việc cần hoàn thành / kết quả mong muốn | [Chưa có bằng chứng] |
| Cách giải quyết hiện tại | [Chưa có bằng chứng] |
| Điều đang hoạt động tốt | [Chưa có bằng chứng] |
| Vướng mắc và mức ảnh hưởng theo lời người tham gia | [Chưa có bằng chứng; không tự gán mức cao/thấp] |
| Thời gian/công sức/chi phí hiện đã bỏ ra nếu tự kể và liên quan | [Chưa có; ghi nguồn và mức chắc chắn, không hỏi ngân sách giả định] |
| Dấu hiệu giữ/đổi cách làm | [Chưa có bằng chứng] |
| Điều bất ngờ / thông tin phản bác | [Chưa có bằng chứng] |
| Mức hài lòng theo cách diễn đạt của họ | [Chưa có; không tự tạo điểm khảo sát] |
| Suy luận của nhóm, tách khỏi dữ liệu | [Chưa suy luận] |
| Thông tin cần hỏi thêm | [Chưa có] |

Có thể ghi chi phí thực tế nếu người tham gia có thẩm quyền và tự nguyện chia sẻ; không suy mức sẵn sàng trả từ lời khen hay câu hỏi giả định. Trường đánh đổi chỉ ghi hành vi đã xảy ra. Nếu ngoài phạm vi hoặc không biết, ghi “không hỏi/không có dữ liệu”.

### 7.5. Đánh giá bằng chứng và việc tiếp theo

| Giả định | Hỗ trợ phần nào | Phản bác phần nào | Phần chưa chứng minh | Nhận định tạm thời và căn cứ |
|---|---|---|---|---|
| VAL-01 | [Chưa có] | [Chưa có] | [Chưa đánh giá] | [Chưa đánh giá] |
| USE-03 | [Chưa có] | [Chưa có] | [Chưa đánh giá] | [Chưa đánh giá] |
| FEA-01 | [Chưa có] | [Chưa có] | [Chưa đánh giá] | [Chưa đánh giá] |

| Việc tiếp theo | Người phụ trách | Hạn dự kiến | Căn cứ / có được phép hỏi lại không |
|---|---|---|---|
| [Chưa xác định] | [Chưa phân công] | [Chưa có] | [Chưa có] |

## 8. Cách dùng kết quả sau này

1. Người hỏi và người ghi đối chiếu ghi chú, giữ nguyên điều không nhớ hoặc chưa rõ. Chỉ sửa trích dẫn theo bản ghi được phép sử dụng; không nhờ AI tự lấp câu trả lời.
2. Liên kết bằng chứng với mã câu hỏi và giả định. Lời người đi khám không xác nhận tải công việc nội bộ; lời quản lý nghe kể không tự trở thành quan sát trực tiếp.
3. Đối chiếu tiêu chí đề xuất trong `02-prioritized-assumptions.md`. Một người nói có khó khăn chưa chứng minh mức độ phổ biến; lời kể về chính sách chưa chứng minh phần mềm chống trùng đúng; luồng ngắn hơn chưa chứng minh giảm việc.
4. Chỉnh Vision/Canvas/proto-personas khi có căn cứ phù hợp, giữ dấu vết nguồn và phản chứng. Có thể dùng `summarize-interview` khi đã có ghi chép/bản chép lời thật; chưa chạy skill đó trong tài liệu này.
5. Nếu chưa tiếp cận được người thật, giữ file này là **kế hoạch phỏng vấn chưa thực hiện**. Tiếp tục desk research có nguồn và giới hạn; không thay bằng AI nhập vai rồi ghi là kết quả nghiên cứu thực tế.

Đầu ra hiện tại chỉ là kịch bản và mẫu ghi chép. Chưa có người tham gia được gán mã, câu trả lời, kết luận xác thực, quyết định MVP hoặc triển khai tính năng.
