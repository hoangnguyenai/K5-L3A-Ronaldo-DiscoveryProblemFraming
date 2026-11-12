# Kịch bản mô phỏng — Nhập mì tại tiệm tạp hóa

> Toàn bộ số lượng, thời gian, ngưỡng và quy cách trong tài liệu này là dữ liệu tổng hợp để làm bài tập trên lớp, không phải số liệu cửa hàng hay thông số được xác minh của sản phẩm. Quan sát thật duy nhất do học viên cung cấp là Hảo Hảo bán chạy hơn, Kokomi còn nhiều hơn tại cửa hàng được quan sát.

## 1. Bối cảnh và sổ hàng

Tiệm A có một người chốt đơn nhập. Bài tập xét hai mã minh họa, không gộp tất cả vị hoặc quy cách của cùng nhãn thành một mã. D0 là ngày lập đơn; dữ liệu bán thuộc 14 ngày ngay trước D0. Tiệm mở đủ 14 ngày, không có ngày hết hàng, không trả hàng, thất thoát hoặc nhập bổ sung trong kỳ mô phỏng.

| Mã minh họa | Nhãn tham chiếu | Tồn đầu kỳ (gói) | Nhập trong kỳ | Bán trong 14 ngày | Tồn tại D0 | Hàng đang về |
|---|---|---:|---:|---:|---:|---:|
| HH01 | Hảo Hảo | 164 | 0 | 140 | 24 | 0 |
| KK01 | Kokomi | 112 | 0 | 28 | 84 | 0 |

Kiểm tra: tồn cuối = tồn đầu + nhập − bán. HH01: 164 − 140 = 24; KK01: 112 − 28 = 84. Tốc độ bán bình quân lần lượt 10 và 2 gói/ngày. Nếu nhịp bán giữ nguyên, tồn hiện tại tương ứng 2,4 và 42 ngày bán; đây là tỷ số mô phỏng, không phải dự báo được kiểm chứng.

## 2. Chính sách nhập để tính thử

Giả lập thời gian giao 2 ngày; chu kỳ xem xét nhập mỗi ngày; quy cách nhập 30 gói/thùng cho cả hai mã. Không coi quy cách này là thông số thực của mọi sản phẩm mang hai nhãn trên. Bài tập không xét hạn dùng cụ thể và giá vốn; người duyệt vẫn phải kiểm các yếu tố này trước khi áp dụng ngoài lớp.

| Mã | Ngưỡng thấp Min | Mức đích Max | Giải thích trong mô hình |
|---|---:|---:|---|
| HH01 | 30 gói | 84 gói | Min bằng 3 ngày bán bình quân, gồm 2 ngày giao và 1 ngày đệm |
| KK01 | 6 gói | 30 gói | Min cũng bằng 3 ngày bán; mức đích thấp hơn vì bán chậm |

Max là tham số chính sách đặt cho bài tập, chưa tối ưu bằng chi phí, vốn hoặc nhu cầu bất định. Khoảng đệm 1 ngày không bảo đảm tránh hết hàng nếu sức bán hoặc thời gian giao thay đổi.

**Rule thử nghiệm:**

1. Kiểm dữ liệu, đơn vị và lịch hàng đang về. Thiếu hoặc mâu thuẫn thì chuyển người kiểm, không điền số.
2. Hàng đang về chỉ cộng khi ngày về đã xác nhận nằm trong 2 ngày xét; vẫn phải kiểm có đủ hàng dùng đến từng lần nhận. Đơn về muộn hoặc chưa rõ ngày chuyển kiểm thủ công để tránh đặt trùng.
3. Nếu tồn khả dụng dự kiến nhỏ hơn Min, tính lượng thô = Max − tồn khả dụng; làm tròn lên theo thùng 30 gói. Nếu bằng hoặc trên Min thì chưa nhập.
4. Nếu làm tròn khiến vượt Max, hoặc có nguy cơ hết hàng trước khi lô mới đến, hiển thị ngoại lệ để người duyệt; không tự đặt đơn.

Với dữ liệu chính không có hàng đang về: HH01 cần 84 − 24 = 60 gói, đúng 2 thùng. KK01 đang có 84 gói, cao hơn Max 30 gói, nên không đề nghị nhập thêm và đưa vào danh sách rà soát. Chênh 54 gói so với Max là chênh theo chính sách mô phỏng, không phải lượng thiệt hại hay lượng chắc chắn phải thanh lý.

“24 + 60 = 84” là vị thế tồn ngay khi lập đề xuất, chưa trừ lượng bán trong thời gian giao. Nếu bán đúng bình quân trong 2 ngày chờ, HH01 còn 4 gói trước nhận và 64 gói sau nhận. Không nhầm 84 là tồn thực ở ngày nhận hàng.

## 3. Thời gian quy trình dùng cho bài tập

| Bước | Quy trình hiện tại | Thời gian mô phỏng |
|---:|---|---:|
| 1 | Kiểm đếm và đối chiếu tồn | 5 phút |
| 2 | Rà số bán và đơn đang về | 8 phút |
| 3 | So sánh từng mã, chọn lượng nhập | 12 phút |
| 4 | Kiểm quy cách, hạn dùng và vốn | 6 phút |
| 5 | Chốt danh sách | 4 phút |
| Tổng | | 35 phút |

Đây là ngân sách thời gian dựng cho tình huống, không phải baseline đo thật. Mục tiêu thiết kế là tối đa 28 phút cho cùng đầu việc, tức giảm 20%; chưa có kết quả đạt mục tiêu. Không suy ra rằng phần mềm đã giúp giảm tồn hoặc tăng doanh thu.

## 4. Mười cặp input/đầu ra mong đợi

Mặc định dùng HH01, Min 30, Max 84, 30 gói/thùng, giao trong 2 ngày; mỗi dòng chỉ thay dữ liệu nêu trong input. Đây là mẫu kiểm tra Rule, không phải dữ liệu phỏng vấn hoặc eval đầu ra AI.

| # | Input | Đầu ra mong đợi |
|---:|---|---|
| 1 | HH01 tồn 24, đang về 0 | Đề nghị 60 gói = 2 thùng; vị thế tồn 84 |
| 2 | KK01 tồn 84, Min 6, Max 30 | Không nhập; cảnh báo vượt Max 54 gói |
| 3 | HH01 tồn 30 | Không nhập vì tồn bằng Min |
| 4 | HH01 tồn 29 | Lượng thô 55, làm tròn 60 gói; vị thế 89 vượt Max 5, cần duyệt ngoại lệ |
| 5 | HH01 tồn 24, có 60 gói về sau 1 ngày | Vị thế 84; chưa nhập thêm; kiểm 24 gói đủ dùng tới ngày nhận theo nhịp 10 gói/ngày |
| 6 | HH01 tồn 24, có 60 gói về sau 5 ngày | Chuyển kiểm thủ công vì có đơn về muộn; không tự đặt chồng đơn |
| 7 | Không có số tồn | Không đưa số lượng nhập; yêu cầu kiểm đếm |
| 8 | Tồn 2 thùng nhưng chưa biết số gói/thùng | Không cộng với dữ liệu đơn vị gói; yêu cầu quy đổi |
| 9 | Tồn ghi sổ 24 nhưng kiểm đếm 12 | Chặn đề xuất; đối soát chênh lệch trước |
| 10 | HH01 tồn 0, không có hàng đang về | Báo đã hết hàng; nếu áp Rule lượng thô 84, làm tròn 90 gói, vượt Max 6; chuyển người quyết định phương án khẩn, không chỉ tạo đơn bình thường |

Tính đúng các trường hợp này chỉ chứng minh tính nhất quán của Rule trong kịch bản, không xác nhận nhu cầu người dùng hoặc hiệu quả vận hành.

## 5. Phân bổ buổi làm 120 phút

| Thời gian | Công việc |
|---|---|
| 0–10 phút | Đọc yêu cầu, phân biệt dữ liệu thật và mô phỏng |
| 10–30 phút | Rà CP1, hoàn thiện card ưu tiên CP2 |
| 30–45 phút | Nhóm tự pitch và phản biện CP3, ghi lại thảo luận thực tế |
| 45–60 phút | Kiểm nguồn research CP4 và đối chiếu phép tính kịch bản |
| 60–85 phút | Hoàn thiện sơ đồ và Problem Statement CP5 |
| 85–105 phút | So sánh mức can thiệp, rà eval và quyết định CP6 |
| 105–120 phút | Từng người tự viết reflection CP7 và rà cấu trúc nộp |

Phần mô phỏng không thay thế yêu cầu kiểm chứng người thật ở CP4 theo đề gốc. Kết quả hiện tại phù hợp để phân tích tình huống trên lớp, chưa được coi là hoàn thành kiểm chứng thực địa.
