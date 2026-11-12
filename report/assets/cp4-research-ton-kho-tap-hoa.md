# Quyết định nhập hàng tại cửa hàng tạp hóa

Hướng khảo sát hiện tại của nhóm ronaldo: giảm nhập dư hàng bán chậm đồng thời hạn chế thiếu hàng bán chạy. Loại cửa hàng do Nguyễn Lâm Hoàng lựa chọn: tạp hóa. Chưa có dữ liệu của cửa hàng hoặc phỏng vấn; chưa xác nhận kết quả hội tụ CP3.

## Phạm vi dự kiến

Một cửa hàng, một nhóm hàng đóng gói, khoảng 10–20 mã hàng để khảo sát ban đầu. Đây là phạm vi đề xuất, không phải số mã đã thu thập. Chốt nhóm hàng theo khả năng tiếp cận dữ liệu thực tế.

Tập trung vào lần chủ cửa hàng chuẩn bị đơn nhập kế tiếp: cần kiểm tra gì để quyết định mặt hàng nào cần nhập, số lượng bao nhiêu và mặt hàng nào nên tạm hoãn? Chưa mở rộng sang nhiều chi nhánh, tối ưu toàn bộ cửa hàng hoặc đặt hàng tự động.

## Những giả thuyết cần kiểm chứng

| Giả thuyết | Bằng chứng cần có | Tín hiệu phản bác cần ghi nhận |
|---|---|---|
| Khó khăn nằm ở quyết định số lượng nhập | Một lần nhập dư hoặc thiếu cụ thể, cách chủ quán quyết định lúc đó | Quyết định đúng nhưng nhà cung cấp giao thiếu hoặc giao chậm |
| Có thể tổng hợp đủ số bán, tồn và hàng đang về | Ghi chép, báo cáo bán hàng, kiểm đếm và đơn chưa nhận | Không ghi số bán hoặc tồn sổ khác tồn thực tế |
| Dữ liệu cũ đủ hữu ích cho nhóm hàng chọn | Các kỳ bán và nhập liên tiếp, sự kiện bất thường | Hàng mới hoặc nhu cầu biến động không phản ánh trong lịch sử |
| Chủ cửa hàng cần giảm thời gian đối chiếu | Thời gian từng bước trong một lần lập đơn | Chỉ mất ít phút và chủ quán đã hài lòng với cách hiện tại |
| Cảnh báo có thể chuyển thành hành động | Quy cách thùng/lốc, thời gian giao, vốn có thể dùng | Nhận diện đúng nhưng không mua được do tối thiểu đặt hàng hoặc thiếu vốn |

Nhóm tự bổ sung mức quan trọng, mức bằng chứng và ưu tiên trong Assumption Map sau thảo luận.

## Dữ liệu tối thiểu để hiểu một quyết định nhập hàng

| Dữ liệu | Mục đích | Tình trạng |
|---|---|---|
| Mã hàng và đơn vị: chai, gói, lốc, thùng | Tránh cộng hoặc so sánh khác đơn vị | Chưa có |
| Số bán theo ngày và ngày có mở cửa | Hiểu nhịp bán; phân biệt ngày không ghi dữ liệu với bán bằng 0 | Chưa có |
| Tồn kiểm đếm và thời điểm kiểm | Đối chiếu với tồn ghi sổ | Chưa có |
| Hàng đã đặt nhưng chưa về, ngày dự kiến về | Tránh đề nghị nhập trùng | Chưa có |
| Ngày đặt, ngày nhận và số nhận thực tế | Hiểu thời gian giao và chênh lệch đơn nhập | Chưa có |
| Quy cách đặt hàng, hạn dùng nếu có | Kiểm tra khả năng thực hiện và nguy cơ tồn lâu | Chưa có |
| Ngày hết hàng, yêu cầu mua không phục vụ được nếu có ghi | Không nhầm số bán thấp do hết hàng với nhu cầu thấp | Chưa có |
| Lý do chủ quán tăng/giảm số nhập, khuyến mãi hoặc sự kiện | Giải thích ngoại lệ ngoài số bán | Chưa có |

Chỉ thu thập dữ liệu chủ quán đồng ý chia sẻ. Dùng mã thay tên cửa hàng/nhà cung cấp khi cần; không đưa thông tin khách hàng và thông tin thanh toán vào repo.

## Research giải pháp đã có

Nguồn chính thức đã được công cụ web mở ngày 09/11/2026. Người học tự kiểm lại trước khi đưa vào bảng research chính thức.

| Công cụ/pattern | Nguồn | Nội dung được xác nhận | Bài học và giới hạn áp dụng |
|---|---|---|---|
| KiotViet: định mức tồn | [Hướng dẫn danh mục hàng hóa](https://www.kiotviet.vn/huong-dan-su-dung-kiotviet/salon-hang-hoa/danh-muc-hang-hoa/) | Thiết lập tồn ít nhất/nhiều nhất để cảnh báo nhập hàng | Cảnh báo theo ngưỡng đã có sẵn. Trang hướng dẫn thuộc ngành làm đẹp; cần kiểm tra đúng phiên bản bán lẻ mà cửa hàng sử dụng, chưa suy ra chức năng tại cửa hàng cụ thể |
| Sapo: báo cáo nhập hàng | [Tổng quan báo cáo nhập hàng](https://help.sapo.vn/tong-quan-bao-cao-nhap-hang) | Phân tích hàng nhập theo sản phẩm, thời gian, nhà cung cấp và đơn; phân biệt ngày nhập kho với ngày thanh toán | Có thể tận dụng báo cáo có sẵn để hiểu lịch nhập. Báo cáo nhập hàng tự nó chưa chứng minh dự đoán đúng lượng cần nhập |

Suy luận: cần thử cách đối chiếu dữ liệu và ngưỡng đơn giản trước. Chưa có căn cứ chọn AI chỉ vì bài toán có nhiều con số.

## Điểm đáng khám phá

Thay vì chỉ hỏi “hàng nào sắp hết”, khảo sát việc **giải thích vì sao cần nhập hoặc chưa nên nhập**: tồn thực tế bao nhiêu, hàng nào đang về, lịch bán có ngày hết hàng không, đơn vị nhập khác đơn vị bán ra sao và hạn dùng có tạo rủi ro không.

Một danh sách có căn cứ để chủ quán kiểm tra có thể hữu ích hơn con số đề xuất không giải thích được. Đây là giả thuyết thiết kế, chưa phải kết luận từ người dùng.

## Đo lường cho thử nghiệm sau kiểm chứng

- Thời gian lập danh sách nhập: tính cả kiểm tồn, tổng hợp dữ liệu, rà lại và sửa đề xuất. Baseline và target chưa có.
- Số lỗi có thể kiểm tra trong danh sách: sai đơn vị, bỏ qua hàng đang về, dùng tồn cũ hoặc không có căn cứ dữ liệu.
- Số ngày-mã hàng hết hàng trong thời gian theo dõi; ghi cùng cửa sổ và số mã quan sát.
- Giá trị tồn và hàng cận hạn nếu có dữ liệu, theo định nghĩa thống nhất. Không coi giảm tồn đơn thuần là thành công nếu tình trạng thiếu hàng tăng.
- Khi thử trên lịch sử, chỉ dùng dữ liệu có sẵn trước ngày ra quyết định. Không lấy doanh số sau đó để làm đầu vào rồi báo là dự đoán đúng.

Không suy ra doanh thu bị mất chỉ từ số bán bằng 0. Không cam kết giảm tồn một tỷ lệ cụ thể khi chưa có baseline và thử nghiệm.

## Phản biện mức can thiệp

| Mức | Điều cần kiểm tra |
|---|---|
| No AI | Sổ theo dõi thống nhất, kiểm tồn đúng và checklist nhập hàng đã giải quyết được phần lớn pain chưa? |
| Rule | Cảnh báo tồn theo ngưỡng, tính số liệu và quy đổi đơn vị có đủ không? Ai đặt và điều chỉnh ngưỡng? |
| Workflow có AI | Có bước đọc ghi chú rời rạc hoặc giải thích ngoại lệ mà Rule không xử lý đủ không? Chủ quán kiểm lại bằng cách nào? |
| Agent | Hiện chưa có bằng chứng cần AI tự chọn hành động; không mặc định tự đặt đơn hoặc liên hệ nhà cung cấp. |

Nếu dùng công cụ hỗ trợ, số liệu phải truy về nguồn và chủ cửa hàng duyệt đơn. Khi dữ liệu thiếu hoặc mâu thuẫn, chuyển kiểm tra thủ công thay vì tự điền số.

## Bước tiếp theo

Xác nhận cửa hàng có thể tiếp cận, nhóm hàng và một lần nhập thực tế. Sau đó nhóm tự hội tụ CP3 và kiểm chứng CP4 với người thật bên ngoài nhóm theo yêu cầu đề bài. Giữ nguyên năm trải nghiệm cá nhân CP1; hướng tạp hóa hiện xuất phát từ phần brainstorm, chưa coi là trải nghiệm trực tiếp của học viên.
