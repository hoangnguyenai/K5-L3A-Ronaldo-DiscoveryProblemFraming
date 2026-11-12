# Research sơ bộ — Chờ thanh toán tại quán

> Nhóm: ronaldo. Hướng được Nguyễn Lâm Hoàng chọn phát triển từ trải nghiệm cá nhân; chưa có kết quả chốt tập thể CP3. Research ngày 09/11/2026. Chưa có phỏng vấn/survey hoặc số liệu hiệu quả giải pháp. Không phải Problem Statement hay quyết định do AI viết thay nhóm.

## 1. Điều đã biết và chưa biết

**Đã biết từ người học:** chờ thanh toán tại quán 5–15 phút/lần, khoảng 2–3 lần/tuần; thường gọi nhân viên nhiều lần hoặc đợi tại bàn. Đây là khoảng chờ tự thuật, chưa xác định chính xác điểm bắt đầu/kết thúc.

**Bổ sung từ người học:** khoảng 19h30 tối thứ Bảy, quán bia, nhóm khách 9 người. Chờ lâu ở gọi nhân viên và nhận bill; đã gọi vài lần. Khoảng chờ 10–15 phút bắt đầu từ lần gọi tính tiền đầu tiên, chưa xác nhận mốc kết thúc. Một người ứng tiền rồi tự tính và nhắc chuyển khoản.

**Chưa biết:** ngày lịch cụ thể; quán dùng POS hay ghi tay; từng bước mất bao lâu; khách và nhân viên khác có cùng vấn đề không; giữa tiếp nhận yêu cầu và mang bill, bước nào nghẽn chính. Không lấy trung điểm của khoảng tự thuật làm baseline đã đo.

**Phạm vi cần phân biệt:** (A) chờ tiếp nhận và nhận bill tại quán; (B) chia tiền và thu lại từ nhóm sau khi một người ứng trước. Dữ liệu mới xác nhận cả hai xảy ra, chưa chứng minh giải pháp cho A giải được B. Chưa có số phút hoặc tần suất riêng của B.

## 2. Giải pháp đã có — nguồn chính thức

Các trang đã được công cụ web mở và đọc. Học viên cần tự mở và kiểm nội dung theo RULES.md trước khi đưa vào bảng research chính thức.

| Công cụ/pattern | Nguồn | Nội dung nguồn xác nhận | Bước có thể hỗ trợ | Điều còn phải kiểm tra ở quán cụ thể |
|---|---|---|---|---|
| Toast Mobile Order & Pay | [FAQ của Toast](https://support.toasttab.com/en/article/Toast-Mobile-Order-and-Pay-FAQs) | Khách quét QR tại bàn để gọi món và thanh toán từ thiết bị của mình; tài liệu cũng mô tả việc quay về phục vụ trực tiếp khi mất internet | Giảm phụ thuộc vào việc nhân viên mang phương tiện thanh toán đến bàn | Mô hình vận hành và khả năng triển khai tại quán; không suy ra dịch vụ hỗ trợ thị trường Việt Nam từ nguồn này |
| iPOS O2O trả trước | [Hướng dẫn thao tác khách hàng](https://huongdan.ipos.vn/docs/huong-dan-su-dung-o2o-tra-truoc/van-hanh/thao-tac-khach-hang/) | Khách kiểm tra món, chọn phương thức thanh toán; một số bước vẫn có trạng thái chờ thu ngân xác nhận | Thay đổi thứ tự thanh toán, hỗ trợ luồng gọi món và thanh toán từ thiết bị khách | Đây là mô hình trả trước, không tự coi là cùng quy trình với ăn xong mới thanh toán; cần xem quán có chấp nhận đổi mô hình không |
| KiotViet thanh toán QR | [Trang giải pháp KiotViet](https://finance.kiotviet.vn/thanh-toan.html) | Nhà cung cấp mô tả thông báo tiền về và xác nhận giao dịch trên màn hình thu ngân khi khách thanh toán QR cho đơn hàng | Hỗ trợ bước xác nhận tiền đã về | Chưa chứng minh giảm bước chờ gọi nhân viên hoặc chờ lập bill; kiểm tra hệ thống quán đang dùng trước khi đề xuất |

**Suy luận từ research:** QR thanh toán đã có sẵn, nên chưa có cơ sở gọi việc “thêm QR” là đột phá. Tính năng được nhà cung cấp mô tả không phải bằng chứng tiết kiệm thời gian ở quán của người học.

## 3. Điểm đáng thử nếu dữ liệu xác nhận

Khảo sát một quy trình **yêu cầu thanh toán có trạng thái rõ**: khách chủ động báo muốn thanh toán; nhân viên biết yêu cầu đã được tiếp nhận chưa; bill chỉ chuyển sang chờ trả tiền khi đã kiểm tra; trạng thái hoàn tất lấy từ người có trách nhiệm hoặc hệ thống đã xác thực.

Giả thuyết giá trị là giảm lần gọi nhắc và chờ không biết yêu cầu đã tới ai. Cần kiểm tra xem đây có thực sự là nguyên nhân gây chờ; nếu nghẽn ở sửa món sai thì luồng báo yêu cầu chưa giải quyết được gốc vấn đề.

Chưa cần xây app. Một thử nghiệm giấy có mã bàn và trạng thái có thể giúp quan sát luồng xử lý trước khi tích hợp POS. Chỉ thực hiện thử ở quán khi được người phụ trách đồng ý, không tự can thiệp thanh toán thực tế.

## 4. Phản biện các mức can thiệp để nhóm tự cân nhắc

| Mức | Khả năng cần kiểm tra | Căn cứ cần có trước khi chọn |
|---|---|---|
| No AI | Một người nhận yêu cầu rõ ràng, hàng đợi theo bàn, bill được kiểm tra theo checklist | Chờ có phải do yêu cầu bị bỏ sót hoặc phân công không rõ? |
| Rule | Yêu cầu theo mã bàn, trạng thái tiếp nhận/xử lý, thông báo quá hạn theo ngưỡng nhóm chọn | Có dữ liệu mã bàn, trạng thái và người chịu trách nhiệm cập nhật không? |
| Workflow có AI | AI hỗ trợ hiểu yêu cầu ngôn ngữ tự do, con người xác nhận trước tác động đến bill | Có nhiều yêu cầu diễn đạt khác nhau mà nút chọn cố định không đáp ứng? |
| Agent | Chưa thấy nhu cầu từ dữ liệu hiện tại | Bằng chứng nào cho thấy bước tiếp theo không thể định sẵn và Rule/Workflow không đủ? |

Đây là gợi ý phản biện cho CP5–CP6, không phải kết quả thảo luận CP3. Nhóm tự chọn mức và tự viết lập luận. Không mặc định phải có AI để đạt điểm.

## 5. Cách lấy baseline và kiểm chứng kết quả

Ghi rõ cho từng lần quan sát được phép: giờ khách yêu cầu thanh toán; giờ nhân viên tiếp nhận; giờ khách nhận bill; giờ bill được xác nhận đúng; giờ thanh toán được xác nhận hoàn tất; số lần gọi nhắc; có sửa bill không. Không ghi thông tin ngân hàng hoặc thông tin cá nhân của khách.

Từ đó tách thời gian chờ từng đoạn, xác định bottleneck và tổng thời gian. Trường hợp chưa xong phải ghi “chưa hoàn tất”, không loại khỏi mẫu chỉ để kết quả đẹp hơn. Khoảng 5–15 phút người học nhớ lại là bối cảnh ban đầu, không thay thế số đo này.

Nếu thử quy trình mới, đo trong khung giờ và mức đông tương tự; tính cả công cập nhật trạng thái của nhân viên. Cần giữ chất lượng hóa đơn và xác nhận thanh toán, không chỉ giảm số phút.

Nhóm tự chốt target và ngưỡng dừng sau khi có baseline. Chưa điền các tỷ lệ cải thiện hoặc kết quả pilot khi chưa thử.

## 6. Việc cần hoàn thành trực tiếp

- Người học chốt top 3 từ CP1, viết card và bổ sung thời gian từng bước dựa trên lần thật.
- Nhóm thực hiện CP3: pitch, phản biện, cluster, OST, chấm điểm và chọn candidate.
- Nếu chọn chờ thanh toán, kiểm chứng với 2–3 người thật bên ngoài nhóm đã gặp/vận hành quy trình này, hoặc survey 5–10 người; ghi nguồn, thời điểm, cách hỏi và tín hiệu phản bác.
- Sau kiểm chứng, nhóm tự viết Problem Statement để AI phản biện; bổ sung workflow bằng Mermaid từ quy trình thật.
- Từng người tự ghi đóng góp và viết reflection.

Tình trạng hiện tại: chưa đủ dữ liệu để kết luận Go/Not Yet/No-Go thay nhóm.
