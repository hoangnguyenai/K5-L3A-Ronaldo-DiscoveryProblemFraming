# Báo cáo cá nhân — 2A202603460_NguyenTienKhoa

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Tiến Khoa
- MSSV: 2A202603460
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: 7.1
- Link repo nhóm: https://github.com/hoangnguyenai/K5-L3A-Ronaldo-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi chuẩn bị nộp bài tập lớn/lab lúc sát deadline (22h–23h), tôi muốn đối chiếu nhanh toàn bộ file sản phẩm với rubric và checklist quy định (tên file, cấu trúc thư mục, tiêu chí đủ), để không bị mất điểm oan do sai quy cách format hay thiếu mục bắt buộc | Sinh viên nộp bài, nhóm trưởng, trợ giảng (TA) chấm bài | 3/5 bài lab trước cả nhóm mất 35–45 phút rà soát trước giờ nộp; từng bị trừ 1.0 điểm ở bài Day 01 vì quên đổi tên một file theo quy ước MSSV |
| 2 | Lặp lại | Khi bắt đầu tuần làm việc/học tập mới vào sáng thứ Hai, tôi muốn có danh sách tổng hợp tất cả deadline, task cần hoàn thành và lịch họp từ các môn học ở một nơi duy nhất, để không bị quên hoặc nhầm lẫn thứ tự ưu tiên | Sinh viên (bản thân), các thành viên cùng nhóm đồ án | Mỗi sáng thứ Hai mất 20–25 phút mở 3 nền tảng (LMS trường, Notion, Google Calendar) để ghi chép lại; 2 tuần trước quên 1 quiz online vì lịch thi nằm riêng trong mục thông báo LMS |
| 3 | Lặp lại | Khi kết thúc buổi họp nhóm đồ án hằng tuần, tôi muốn có bản tóm tắt các quyết định đã chốt, đầu việc và hạn chót của từng thành viên, để gửi vào nhóm chat Zalo trong vòng 15 phút mà không cần nghe lại file ghi âm | Cả nhóm đồ án (4 người), nhóm trưởng | 2 cuộc họp/tuần, mỗi lần mất trung bình 25–30 phút ngồi lọc lại từ note nháp; 1 lần thành viên hiểu lầm phân công do recap viết vội thiếu chi tiết |
| 4 | Tốn thời gian | Khi bắt đầu giai đoạn làm cơ sở lý thuyết (Related Work) cho đồ án môn học, tôi muốn trích xuất được phương pháp, tập dữ liệu và kết quả thực nghiệm từ 5–10 bài báo khoa học (paper PDF 10–15 trang), để hoàn thành bảng so sánh tài liệu tham khảo cho báo cáo | Sinh viên làm đồ án, giảng viên hướng dẫn | Tự bấm giờ mất trung bình 35–45 phút cho mỗi bài báo (đọc lướt, tìm mục Methodology và Results); tổng cộng tốn gần 4–5 tiếng/tuần trong đợt làm đồ án |
| 5 | Tốn thời gian | Khi phát sinh lỗi runtime hoặc lỗi test suite trong quá trình chạy bài tập lớn môn lập trình, tôi muốn xác định nhanh vị trí hàm gây lỗi và nguyên nhân từ hàng trăm dòng log console/stack trace, để sửa bug kịp giờ nộp | Sinh viên lập trình (bản thân và bạn cùng nhóm) | Tần suất 2–3 lần/tuần; tuần trước mất 50 phút đọc trace log từ Docker container mới phát hiện lỗi sai định dạng biến môi trường `.env` |
| 6 | Tốn thời gian | Khi chuẩn bị tài liệu kỹ thuật (API document) cho hệ thống backend của bài tập lớn, tôi muốn cập nhật mô tả các endpoint, tham số request và dữ liệu trả về tương ứng với code mới nhất, để các bạn làm frontend có thể kết nối ngay mà không phải hỏi đi hỏi lại | 2 bạn làm backend, 2 bạn làm frontend trong nhóm | Mỗi cuối sprint mất khoảng 90–120 phút dò từng controller để viết file Markdown; có 2 lần frontend bị lỗi do backend đổi response mà chưa kịp update doc |
| 7 | Cần đọc, tổng hợp nhiều thông tin | Khi một tính năng trong đồ án nhóm hoạt động không đúng logic cũ đã bàn, tôi muốn tìm lại nhanh lý do vì sao nhóm lại chọn giải pháp đó từ các thảo luận cũ, để không phải tranh cãi lại từ đầu trong cuộc họp | Toàn bộ 4 thành viên trong nhóm | Mỗi tuần mất khoảng 15–20 phút lục lại lịch sử tin nhắn trong kênh Discord và commit history trên GitHub; có 1 lần nhóm mất gần 45 phút họp chỉ để tranh luận lại một quyết định kiến trúc đã chốt từ 2 tuần trước |
| 8 | Cần đọc, tổng hợp nhiều thông tin | Khi bước vào tuần ôn thi cuối kỳ, tôi muốn tổng hợp các định nghĩa cốt lõi, công thức và dạng bài tập trọng tâm từ slide bài giảng PDF, ghi chú trên lớp và bài tập lab, để có một đề cương ôn tập súc tích dưới 10 trang | Sinh viên môn học (bản thân và nhóm bạn học chung) | Mỗi môn học có trung bình 12 file slide (mỗi slide 40–60 trang), tốn khoảng 4–6 tiếng ngồi tổng hợp thủ công cho 1 môn; kỳ trước trễ hạn ôn tập 1 môn do khối lượng tài liệu quá tải |
| 9 | Pain từ người khác | Khi làm nhóm trưởng đồ án, các thành viên muốn biết rõ quy cách đặt tên branch Git, format commit message và các bước kiểm tra trước khi tạo Pull Request, để không bị từ chối merge code | Nhóm trưởng (tôi) và 3 thành viên trong nhóm | Đếm được 6 lần trong 2 tuần qua các bạn nhắn tin hỏi lại quy tắc dù đã ghi trong file README; tôi mất khoảng 10–15 phút/ngày để trả lời và hướng dẫn lại qua tin nhắn Zalo |
| 10 | Pain từ người khác | Khi sinh viên nộp Pull Request lên repo chung của đồ án, người review trong nhóm muốn nắm được nhanh những thay đổi cốt lõi và mục đích của đoạn code mới, để đánh giá và duyệt PR trong vòng 10 phút thay vì phải đọc từng dòng code lạ | Reviewer (thành viên chịu trách nhiệm merge code), tác giả PR | 3/5 PR trong tuần trước không có mô tả chi tiết, reviewer mất 30–40 phút/PR để đọc code và comment hỏi lại mục đích sử dụng biến/hàm |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Quá trình thực hiện:** Tôi tự scan 8 ý đầu tiên dựa trên trải nghiệm thực tế trong các kỳ học và làm đồ án nhóm. Sau đó dùng AI gợi ý thêm 4 ý bổ sung.
- **Ý AI gợi ý được giữ lại:** Giữ lại ý #9 (Thành viên hỏi lại quy chuẩn Git/PR) và ý #10 (Reviewer tốn thời gian đọc PR thiếu context) vì đây là pain point rất thật của nhóm tôi trong 2 tuần vừa qua khi code chung trên GitHub. Tôi đã viết lại theo đúng trải nghiệm thực tế với số liệu đo lường cụ thể của nhóm mình.
- **Ý AI gợi ý bị loại bỏ:** 
  1. *"Xây dựng trợ lý ảo AI thông minh tự động trả lời mọi thắc mắc học tập 24/7"*: Bị loại ngay vì đây là giải pháp trá hình (chứa chữ AI/trợ lý ảo), phạm vi quá rộng và không chỉ ra được bottleneck cụ thể nào.
  2. *"Tự động phân chia task cho thành viên nhóm theo năng lực"*: Bị loại vì không có quy trình thực tế rõ ràng, việc phân chia task trong nhóm sinh viên phụ thuộc vào thảo luận trực tiếp và cam kết cá nhân, không thể đưa vào quy trình tự động hóa.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Đối soát rubric & checklist nộp bài lab/đồ án (#1) | Quy trình lặp lại đều đặn mỗi tuần; thời gian baseline đo được chính xác (35–45 phút/lần); rủi ro cao vì sai sót format là mất điểm ngay | Liệu có kiểm tra được chất lượng ngữ nghĩa nội dung các mục hay chỉ check được tên file và placeholder? |
| 2 | Trích xuất thông tin bài báo nghiên cứu cho Related Work (#4) | Pain point lớn của sinh viên làm đồ án; tốn nhiều thời gian đọc quét (3–5 tiếng); có thể giải quyết bằng workflow trích xuất có cấu trúc | File PDF bài báo khoa học có bố cục phức tạp (2 cột, bảng biểu, công thức) nên độ chính xác trích xuất khó đảm bảo 100% |
| 3 | Soạn Meeting Recap và phân công công việc sau họp nhóm (#3) | Diễn ra thường xuyên (2 lần/tuần); quy trình rõ ràng từ note thô sang action items; giúp nhóm vận hành trơn tru | Mức độ cam kết thực hiện task sau khi nhận recap phụ thuộc vào ý thức thành viên, khó đo lường bằng metric kỹ thuật |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị nộp bài tập lớn/lab lúc sát deadline (22h–23h), tôi muốn đối chiếu nhanh toàn bộ file sản phẩm với rubric và checklist quy định (tên file, cấu trúc thư mục, định dạng commit, tiêu chí đủ), để không bị mất điểm oan do sai quy cách format hay thiếu mục bắt buộc |
| Actor | Sinh viên nộp bài / Trưởng nhóm phụ trách đóng gói và nộp bài trên LMS và GitHub |
| Thời điểm / bối cảnh | Khoảng 1–2 tiếng trước hạn chót nộp bài (22h00 – 23h59), khi các thành viên vừa hoàn thành các phần riêng và đang chịu áp lực thời gian lớn |
| Quy trình hiện tại (3–7 bước) | 1. Mở file RUBRIC.md, CHECKPOINTS.md và SUBMISSION.md để đọc lại các yêu cầu bắt buộc (10 phút)<br>2. Mở cây thư mục dự án và kiểm tra tên từng file, thư mục theo cú pháp quy định (8 phút)<br>3. Mở từng file báo cáo cá nhân và nhóm, rà soát bằng mắt xem các tiêu đề, bảng biểu có bị để trống nội dung template không (15 phút)<br>4. Kiểm tra git status, git log xem các commit có đúng cú pháp và đẩy đủ lên origin/main chưa (7 phút)<br>5. Copy link repo nộp lên LMS và chụp màn hình xác nhận (5 phút) |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: Rà soát thủ công nội dung từng mục trong các file markdown để đảm bảo không còn template mẫu chưa điền. Tốn khoảng 15 phút, mắt thường dễ mỏi và bỏ sót lỗi do tâm lý vội vã |
| Impact (nếu không giải thì sao) | Cả nhóm mất 45 phút cho mỗi đợt nộp bài (1–2 lần/tuần); từng bị trừ 1.0 điểm do nộp thiếu 1 trường trong báo cáo cá nhân; gây căng thẳng tột độ cho người phụ trách nộp bài |
| Success metric (baseline → target) | Tổng thời gian rà soát trước nộp bài giảm từ 45 phút xuống dưới 10 phút; tỷ lệ lỗi sai quy cách format hoặc nộp sót mục sau khi nộp giảm về 0% (baseline: 1 lỗi/3 lần nộp) |
| Phương án không dùng AI | Viết 1 checklist cố định trên Google Sheets để các thành viên tự tick + 1 bash script chạy `ls` kiểm tra sự tồn tại của file: giải quyết được việc kiểm tra tên file, nhưng script không thể hiểu được liệu nội dung bên trong file markdown đã được điền nghiêm túc hay chỉ là text mẫu chưa sửa |
| Giả thuyết về AI (nếu có) | Workflow: Dùng Script regex kiểm tra tên file/folder (Rule) kết hợp LLM chạy qua nội dung markdown để phát hiện các mục còn chứa placeholder, văn bản mặc định hoặc thiếu câu trả lời theo rubric; sau đó con người nhìn bảng summary để duyệt lần cuối trước khi nộp |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 45 phút/lần nộp bài

[1. Đọc lại rubric/checklist: 10']
  │
  ▼
[2. Soát tên file/thư mục: 8']
  │
  ▼
[3. Soát nội dung markdown: 15']  ◄── BOTTLENECK (áp lực thời gian, dễ sót mục)
  │
  ▼
[4. Kiểm tra git/commit: 7']
  │
  ▼
[5. Nộp LMS & lưu minh chứng: 5']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu giai đoạn làm cơ sở lý thuyết (Related Work) cho đồ án môn học, tôi muốn trích xuất được phương pháp, tập dữ liệu và kết quả thực nghiệm từ 5–10 bài báo khoa học (paper PDF 10–15 trang), để hoàn thành bảng so sánh tài liệu tham khảo cho báo cáo |
| Actor | Sinh viên làm nghiên cứu / đồ án môn học chuyên ngành |
| Thời điểm / bối cảnh | Giai đoạn 2–3 tuần đầu của học kỳ khi vừa chốt đề tài và cần khảo cứu tài liệu liên quan |
| Quy trình hiện tại (3–7 bước) | 1. Tải 5 file PDF bài báo từ Google Scholar/arXiv về máy (10 phút)<br>2. Mở từng PDF, đọc Abstract và Introduction để nắm bài toán (30 phút / 5 paper)<br>3. Đọc lướt phần Methodology để tìm kiến trúc mô hình chính (45 phút / 5 paper)<br>4. Rà soát bảng kết quả thực nghiệm để lấy số liệu metric (Accuracy, F1, BLEU...) (60 phút / 5 paper)<br>5. Tổng hợp các thông tin vừa trích xuất vào bảng so sánh trên file Word/Overleaf (35 phút) |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4: Tìm kiếm và trích xuất đúng con số kết quả thực nghiệm và baseline so sánh trong các bảng biểu phức tạp ở phần Experiments (mất ~60 phút cho 5 bài) |
| Impact (nếu không giải thì sao) | Mất 180 phút (3 tiếng) cho mỗi đợt làm tài liệu; sinh viên dễ nản, dễ nhầm lẫn số liệu giữa các mô hình baseline của tác giả khác nhau |
| Success metric (baseline → target) | Thời gian trích xuất thông tin cho 5 paper giảm từ 180 phút xuống 40 phút; độ chính xác trích xuất đúng tên phương pháp và chỉ số đo lường đạt ≥ 90% (có người kiểm tra lại) |
| Phương án không dùng AI | Lập bảng Notion cố định sẵn các cột: [Tên bài] [Bài toán] [Mô hình] [Dataset] [Metric chính] [Hạn chế] và dùng tính năng tìm kiếm từ khóa (Ctrl+F "dataset", "accuracy") trong file PDF. Giúp tập trung hơn nhưng vẫn phải đọc quét mắt thủ công |
| Giả thuyết về AI (nếu có) | Workflow: Trích xuất text từ PDF, gửi qua LLM kèm schema JSON định nghĩa sẵn các trường cần trích xuất; sinh viên chỉ cần đối chiếu lại với file gốc |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 180 phút (cho 5 paper)

[1. Tải PDF về máy: 10']
  │
  ▼
[2. Đọc Abstract & Intro: 30']
  │
  ▼
[3. Đọc Methodology: 45']
  │
  ▼
[4. Rà soát bảng số liệu: 60']  ◄── BOTTLENECK (bảng số liệu phức tạp, đọc quét lâu)
  │
  ▼
[5. Điền bảng so sánh Overleaf: 35']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi vừa kết thúc cuộc họp nhóm đồ án kéo dài 1–2 tiếng, tôi muốn có bản tóm tắt các quyết định đã chốt, đầu việc và hạn chót của từng thành viên, để gửi vào nhóm chat Zalo trong vòng 15 phút mà không cần nghe lại file ghi âm |
| Actor | Nhóm trưởng đồ án sinh viên |
| Thời điểm / bối cảnh | Ngay sau khi kết thúc buổi họp online qua Google Meet hoặc offline tại thư viện trường |
| Quy trình hiện tại (3–7 bước) | 1. Vừa họp vừa ghi chú nhanh vào Google Docs hoặc sổ tay (trong suốt buổi họp)<br>2. Đọc lại toàn bộ ghi chú thô và nghe lại các đoạn thảo luận tranh cãi để xác định quyết định cuối cùng (15 phút)<br>3. Tổng hợp danh sách việc cần làm theo định dạng: [Ai làm] [Làm gì] [Hạn chót] (12 phút)<br>4. Đọc rà soát lại và bấm gửi vào nhóm Zalo (5 phút) |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2: Lọc từ ghi chú lộn xộn để tìm ra quyết định cuối cùng và phân công rõ ràng cho từng người (mất 15 phút) |
| Impact (nếu không giải thì sao) | Tốn khoảng 32–35 phút/cuộc họp (2 cuộc họp/tuần = hơn 1 tiếng/tuần); nếu ghi sót thì buổi sau các bạn sẽ quên làm task |
| Success metric (baseline → target) | Thời gian ra được bản recap giảm từ 32 phút xuống dưới 10 phút; 100% đầu việc trong tuần được gán đúng người và hạn chót |
| Phương án không dùng AI | Mở sẵn 1 bảng Kanban trên Trello hoặc Notion ngay trong lúc họp, chốt việc nào thì người nói tự gõ vào bảng đó. Nhược điểm: làm gián đoạn dòng suy nghĩ và nhịp độ tranh luận của buổi họp |
| Giả thuyết về AI (nếu có) | Workflow: AI nhận transcript hoặc text ghi chú thô, tự động phân loại thành [Quyết định đã chốt] và [Action Items kèm người + deadline]; nhóm trưởng chỉ cần 3 phút đọc lướt và nhấn gửi |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 32 phút/lần họp

[1. Ghi chép thô trong lúc họp]
  │
  ▼
[2. Đọc lại note thô & lọc quyết định: 15']  ◄── BOTTLENECK (note lộn xộn, mất thời gian nhớ lại)
  │
  ▼
[3. Soạn Action Items chi tiết: 12']
  │
  ▼
[4. Đọc soát & gửi Zalo: 5']
```

### Card muốn pitch nhất

- Card số: #1
- Vì sao: Bài toán có tần suất lặp lại hàng tuần rất đều đặn, quy trình các bước rất rõ ràng, có baseline đo lường được bằng phút cụ thể, và là nỗi lo sợ chung của hầu hết sinh viên trong các môn học có quy định nộp bài khắt khe.
- Câu hỏi muốn nhóm phản biện: "Liệu một script kiểm tra tự động (Rule) như bash/python regex tên file đã đủ để giải quyết 80% vấn đề chưa, hay bắt buộc phải cần đến một quy trình có AI để kiểm tra chất lượng nội dung văn bản bên trong?"

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Actor "sinh viên" còn chung chung, ai là người trực tiếp chịu trách nhiệm nộp bài cuối cùng? | Đồng ý | Đã sửa: Nêu đích danh actor là Nhóm trưởng hoặc thành viên được phân công phụ trách đóng gói nộp bài đại diện nhóm |
| Bước bottleneck "kiểm tra bài" dễ bị lẫn lộn giữa kiểm tra hình thức (tên file) và kiểm tra chuyên môn (nội dung đúng/sai) | Đồng ý | Đã sửa: Tách bạch rõ ranh giới: Công cụ chỉ kiểm tra xem các trường bắt buộc đã được điền đầy đủ và có ý nghĩa hay không (tránh nộp file trống/placeholder), không cố gắng chấm điểm hay đánh giá đúng/sai về mặt học thuật |
| Phương án không dùng AI (Script regex + Checklist Sheets) có khi đã đủ tốt và rẻ hơn rất nhiều so với dùng AI | Đồng ý một phần | Đã sửa: Bổ sung rõ trong phần so sánh: Script Rule xử lý 100% phần tên file và đường dẫn, AI chỉ được gọi vào để kiểm tra ngữ nghĩa ở các file markdown dài, và luôn có con người (Human-in-the-loop) duyệt kết quả trước khi submit |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch Card #1 (Rà soát checklist & rubric nộp bài) trước nhóm trong 2 phút | Nhóm nhận thấy đây là pain point sát sườn của cả nhóm; được đưa vào shortlist candidate ở CP3 |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: "Bài toán 'Phân loại email môn học' của Hoàng: một ngày bạn nhận bao nhiêu email thông báo, và tính năng Filter có sẵn của Gmail có giải quyết được 90% không mà cần đến AI?" | Hoàng thừa nhận rule của Gmail đã giải quyết được phần lớn, nhóm quyết định loại candidate này để tập trung vào bài toán có độ mơ hồ cao hơn |
| Nhận phản biện | Câu hỏi tôi nhận được: "Nếu dùng script regex viết bằng Python kiểm tra tên file thì mất 3 giây, tại sao phải cần AI?" (từ bạn Hoàng) | Tôi đã sửa: Làm rõ rằng script chỉ check được tên file, còn bước tốn thời gian nhất (bottleneck 15') là đọc lướt các file báo cáo xem có mục nào để trống hoặc ghi sơ sài không. AI chỉ can thiệp vào bước đọc ngữ nghĩa này |
| Gom cluster / cây OST | Đề xuất gom 3 candidate về giấy tờ, quy trình nộp bài và format báo cáo vào một cụm chung | Tạo thành Cluster A: "Kiểm soát chất lượng và tính đầy đủ của sản phẩm bàn giao trước deadline" trong cây OST |
| Chọn candidate problem | Cùng nhóm chấm điểm theo 7 tiêu chí trong bảng ma trận hội tụ | Thống nhất chọn candidate về "Rà soát đối chiếu rubric và checklist nộp bài" làm bài toán trọng tâm của nhóm |
| Kiểm chứng / research | Phỏng vấn nhanh 2 bạn sinh viên khác nhóm (dùng kỹ thuật The Mom Test: hỏi về hành vi lần nộp bài gần nhất, không hỏi 'bạn có thích tool này không') và tìm kiếm 3 công cụ linter hiện có trên GitHub | Cung cấp dữ liệu thực tế cho bảng Assumption Map và bảng Research giải pháp có sẵn (Markdownlint, Action PR linter) |
| Quy trình nhóm | Tham gia phác thảo quy trình Trước/Sau (Before/After) và chỉ ra các điểm rủi ro | Bổ sung bước "Human Review" bắt buộc vào sơ đồ quy trình tương lai trước khi đẩy bài lên LMS |
| Problem Statement | Đóng góp xây dựng định lượng cho Success Metric (từ 45 phút xuống dưới 10 phút, tỷ lệ lỗi format về 0%) | Hoàn thiện Problem Statement v0 và sau đó nâng cấp lên v1 có boundary rõ ràng |
| Mức can thiệp AI | Phân tích và bảo vệ quan điểm chọn mức **Workflow** thay vì **Agent** | Giúp nhóm không bị sa đà vào việc xây dựng Agent tự động hóa hoàn toàn — điều quá rủi ro và không khả thi trong thời gian ngắn |
| Quyết định | Tham gia đánh giá 4 rủi ro Marty Cagan và cùng nhóm đưa ra quyết định cuối cùng | Chốt quyết định: **Go, phạm vi nhỏ** kèm theo ngưỡng dừng đo lường cụ thể sau 2 tuần thử nghiệm |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Prompt AI gợi ý thêm các vấn đề thường gặp theo 4 lăng kính dựa trên bối cảnh sinh viên CNTT | Mở rộng góc nhìn về lăng kính "Pain từ người khác" (gợi ý về Code Review và Pull Request) | Đưa ra các ý tưởng rất viển vông, giải pháp trá hình như "Chatbot giải đáp thắc mắc toàn năng" | Loại bỏ các giải pháp trá hình; chỉ giữ lại 2 ý về Git/PR và viết lại hoàn toàn bằng số liệu thực tế của nhóm |
| CP2 Problem Card | Đóng vai Product Manager khó tính để phản biện điểm yếu của Problem Card #1 | Bóc trần được việc script regex có thể giải quyết được bước check tên file mà không cần đến AI | Không hiểu được bối cảnh áp lực tâm lý lúc 23h30 sát deadline khiến con người dễ sót lỗi thế nào | Bổ sung rõ ranh giới: Rule làm phần hình thức, AI chỉ hỗ trợ đọc lướt phát hiện placeholder ở nội dung |
| CP4 Research | Tra cứu các giải pháp mã nguồn mở và công cụ linter tự động trên GitHub | Liệt kê nhanh các công cụ như `markdownlint`, `action-check-format` | Ảo tưởng (hallucination) rằng một số công cụ linter đã tích hợp sẵn AI tự sửa nội dung theo rubric | Tự truy cập trực tiếp repo GitHub của từng công cụ để đọc README và xác nhận tính năng thực tế |
| CP5 Quy trình | Sinh mã Mermaid cho sơ đồ quy trình Before/After | Dựng khung sơ đồ luồng nhanh, tiết kiệm thời gian căn chỉnh cú pháp | Vẽ luồng tự động hóa hoàn toàn từ đầu đến cuối mà không có bước con người kiểm tra (HITL) | Thêm khối kiểm tra thủ công của nhóm trưởng và nhánh rẽ quay về (fallback) khi AI phân tích sai |
| CP5–6 Problem Statement | Gợi ý các chỉ số đo lường thành công (Success Metric) cho bài toán | Đưa ra gợi ý về việc đo thời gian tiết kiệm và tỷ lệ phát hiện lỗi | Đưa ra các metric định tính mơ hồ như "tăng độ hài lòng", "giảm stress cho sinh viên" | Thay thế bằng metric định lượng đo bằng phút cụ thể và tỷ lệ lỗi sai format phát hiện được |
| CP6 Mức can thiệp / quyết định | Tham khảo cấu trúc phân tích 4 rủi ro sản phẩm của Marty Cagan | Giúp cấu trúc hóa các câu hỏi phản biện về rủi ro Usability và Feasibility | Đánh giá rủi ro Value quá dễ dãi ("sinh viên chắc chắn sẽ thích dùng công cụ này") | Nhìn nhận thực tế: Nếu công cụ chạy chậm quá 3 phút sát giờ nộp, sinh viên sẽ bỏ qua ngay để nộp tay |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi lắng nghe phần pitch của các thành viên trong nhóm 7.1, tôi nhận ra một bài học rất lớn về góc nhìn: mỗi người thường có xu hướng xem vấn đề cá nhân của mình là quan trọng nhất và mặc định ai cũng cần giải quyết nó. Chẳng hạn, khi nghe bạn đề xuất bài toán phân loại email thông báo học tập, ban đầu bạn cảm thấy rất bức xúc vì hộp thư luôn đầy. Nhưng khi cả nhóm cùng đào sâu bóc tách, chúng tôi mới thấy rằng tần suất thực tế bạn mở email chỉ là 1 lần/ngày và phần lớn thông báo quan trọng đều đã có thông báo đẩy qua Zalo hoặc LMS. Nhờ nghe bài của các bạn, tôi học được cách tách bạch giữa "sự khó chịu mang tính cảm xúc" và một "bottleneck thực tế có thể đo lường định lượng được". Một bài toán tốt để đưa vào giải pháp không phải là bài toán nghe có vẻ to tát, mà là bài toán có quy trình các bước rõ ràng, có điểm nghẽn đo được bằng phút và người trong cuộc đã từng phải trả giá (bị trừ điểm, mất thời gian) vì nó.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Nhóm tôi đã bị bẫy "solution-first" rất nặng ngay từ những phút đầu tiên khi thảo luận nhóm ở CP3. Khi vừa chốt ý tưởng về việc rà soát bài nộp, phản xạ đầu tiên của cả nhóm là lập tức nói về công nghệ: *"Hay là mình build một con Agent dùng LangChain đọc toàn bộ repo rồi tự động commit sửa lỗi luôn?"*. Mọi người bắt đầu hào hứng bàn về việc dùng mô hình gì, prompt ra sao, giao diện web thế nào. May mắn là chúng tôi nhớ lại nguyên tắc của mô hình Double Diamond và câu hỏi phản biện trong đề bài: *"Nếu không có AI, cách đơn giản nhất để giảm một nửa thời gian là gì?"*. Nhóm đã dừng lại khoảng 5 phút để vẽ quy trình hiện tại ra giấy nháp. Khi nhìn vào quy trình 5 bước, chúng tôi giật mình nhận ra: việc kiểm tra tên file hay cấu trúc thư mục thì chỉ cần một dòng lệnh script Bash hoặc Python regex chạy mất 2 giây là xong, hoàn toàn không cần AI. Việc "nghĩ giải pháp trước" suýt nữa đã khiến chúng tôi đưa một con AI đắt đỏ, chậm chạp vào làm một việc mà một dòng lệnh `ls` làm tốt hơn gấp trăm lần. Từ đó, nhóm thống nhất chỉ tập trung vào đúng bước nghẽn thực sự (đọc rà soát nội dung markdown) thay vì cố biến toàn bộ quy trình thành AI.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Tôi đã đổi ý hoàn toàn ở bước xác định mức can thiệp AI giữa CP2 và CP6. Ban đầu trong Problem Card cá nhân, tôi tự tin tích vào ô "Agent" vì nghĩ rằng một hệ thống tự động quét lỗi, tự sửa nội dung markdown và tự động chạy lệnh git push lên GitHub sẽ là phương án ngầu nhất và giải phóng hoàn toàn sức lao động. Tuy nhiên, khi pitch trước nhóm và nhận phản biện từ bạn Hoàng: *"Cận giờ nộp lúc 23h30, nếu Agent tự động sửa file markdown rồi lỡ làm biến dạng nội dung phân tích của bạn thì bạn có dám nộp bài đó lên LMS không, hay bạn lại phải mất thêm 30 phút ngồi diff git để kiểm tra lại con AI?"*. Câu hỏi này đánh trúng tim đen của tôi. Tôi nhận ra mức độ chấp nhận rủi ro (risk tolerance) ở thời điểm sát deadline bằng 0. Nếu để AI tự động hành động (Agent), rủi ro sai sót là không thể cứu vãn. Tôi đã đổi ý ngay lập tức: từ bỏ ý định làm Agent, chuyển hẳn sang mức **Workflow có con người kiểm tra (Human-in-the-loop)**. AI chỉ được phép đưa ra bảng báo cáo cảnh báo (lint report) chỉ ra các mục nghi vấn, còn quyền quyết định sửa và nộp bài bắt buộc phải thuộc về con người.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Điều làm tôi bất ngờ nhất khi thực hiện phỏng vấn kiểm chứng (áp dụng nguyên tắc The Mom Test) với 2 bạn sinh viên cùng khóa là: sinh viên không hề thiếu công cụ hay checklist, mà cái họ thiếu là **sự an tâm trước khi bấm nộp bài**. Khi tôi hỏi về lần nộp bài gần nhất: *"Lần gần nhất nộp bài lab, bạn mất bao lâu để kiểm tra lại và điều gì làm bạn lo nhất?"*, bạn sinh viên trả lời rằng bạn đã in sẵn rubric ra bàn, nhưng đến 23h45 khi mắt đã mờ sau cả ngày code, bạn đọc rubric mà chữ không vào đầu và cứ bấm mở đi mở lại từng file để xem tên file có gõ nhầm chữ hoa chữ thường không. Bất ngờ thứ hai đến từ phần research: trên thị trường đã có rất nhiều công cụ linter markdown xuất sắc (như markdownlint, action-validator), nhưng chúng hoàn toàn bị bỏ xơ xác trong các đồ án sinh viên vì cấu hình quá phức tạp và không gắn liền với rubric cụ thể của từng môn học. Điều này chứng minh rằng giá trị cốt lõi không nằm ở một thuật toán AI siêu việt, mà nằm ở việc đóng gói một quy trình cực kỳ nhẹ nhàng, hiển thị đúng những gì giảng viên sẽ trừ điểm để người nộp bài yên tâm đi ngủ.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Điều khó nhất đối với tôi và cả nhóm khi hoàn thiện Problem Statement là viết phần **Boundary (Ranh giới - AI không được làm gì)** và xác định **Success Metric đo được**. Thông thường chúng ta rất dễ viết những câu mơ hồ như "hệ thống giúp sinh viên nộp bài chuẩn chỉnh hơn" hay "giảm thiểu tối đa sai sót". Nhưng khi bị ép phải đưa ra con số baseline cụ thể (45 phút giảm xuống dưới 10 phút, tỷ lệ lỗi format về 0%) và cách đo thực tế, nhóm đã phải tranh luận rất gay gắt. Khó khăn lớn thứ hai là phần Boundary: việc định nghĩa xem hệ thống *không được phép* làm gì đòi hỏi sự tỉnh táo rất lớn. Nhóm phải quy định rất khắt khe: AI tuyệt đối không được tự ý sửa nội dung file của sinh viên, không được tự động push code hay nộp bài thay người dùng, và không được đưa ra nhận định đúng/sai về mặt kiến thức chuyên môn. Viết được một Boundary chặt chẽ khó hơn nhiều so với việc liệt kê các tính năng mong muốn, vì nó đòi hỏi người làm sản phẩm phải lường trước tất cả các điểm gãy và hậu quả tiêu cực tiềm ẩn.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu có cơ hội làm lại buổi lab này từ đầu, tôi sẽ thay đổi cách tiếp cận ở giai đoạn CP1: tôi sẽ đi khảo sát thực tế và hỏi 3 người thật ngay từ bước scan problem, thay vì ngồi tự suy ngẫm một mình bên máy tính. Việc tự scan khiến góc nhìn ban đầu của tôi bị thu hẹp trong trải nghiệm cá nhân và dễ mang thiên kiến chủ quan. Điểm thứ hai, tôi sẽ phản biện nhóm mạnh mẽ hơn ở CP3 về việc **loại bỏ các ý tưởng quá phức tạp sớm hơn**. Trong buổi thảo luận, nhóm tôi đã mất gần 20 phút tranh luận về một candidate liên quan đến "tự động hóa phân tích dữ liệu log đồ án" - một bài toán mà dữ liệu đầu vào quá hỗn loạn và không ai trong nhóm thực sự hiểu rõ định dạng log. Nếu tôi quyết liệt chỉ ra rằng bài toán đó vi phạm tiêu chí Feasibility (tính khả thi về dữ liệu) ngay từ đầu, nhóm đã có thể dành 20 phút quý báu đó để đào sâu hơn vào việc phỏng vấn thêm người dùng cho candidate được chọn.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Bài toán của nhóm xuất phát từ nỗi đau thực tế: sinh viên thường mất từ 35–45 phút rà soát thủ công trong trạng thái căng thẳng sát deadline và vẫn thường xuyên bị trừ điểm do sai sót format hoặc nộp thiếu mục quy định. Khi phân tích quy trình 5 bước hiện tại, nhóm phát hiện bước nghẽn lớn nhất không nằm ở việc kiểm tra tên file mà nằm ở việc đọc rà soát nội dung từng file markdown để phát hiện các mục còn để trống hoặc chứa template chưa điền. Để giải quyết, Success Metric được xác định rõ ràng là cắt giảm tổng thời gian rà soát từ 45 phút xuống dưới 10 phút và đưa tỷ lệ lỗi sai quy cách sau nộp về mức 0%. Boundary được thiết lập nghiêm ngặt: hệ thống chỉ đóng vai trò rà soát đưa ra báo cáo cảnh báo, tuyệt đối không được tự động sửa đổi nội dung và không được tự ý nộp bài thay sinh viên. Từ ranh giới đó, nhóm xác định mức can thiệp tối ưu là **Workflow** kết hợp: Rule (script regex) xử lý kiểm tra tên file/thư mục, và AI (LLM) hỗ trợ đọc lướt nội dung để phát hiện các trường thiếu sót, với con người là mắt xích duyệt cuối cùng (Human-in-the-loop). Đánh giá qua 4 rủi ro sản phẩm cho thấy giải pháp khả thi về kỹ thuật, chi phí thấp và giá trị sử dụng cao, do đó nhóm đi đến quyết định **Go, phạm vi nhỏ** với cam kết ngưỡng dừng rõ ràng sau 2 tuần thử nghiệm.

---

## 7. Tài liệu tham khảo

- Teresa Torres (2021), *Continuous Discovery Habits: Discover Products that Create Customer Value and Business Value* (Kỹ thuật Opportunity Solution Tree).
- Rob Fitzpatrick (2013), *The Mom Test: How to talk to customers & learn if your business is a good idea when everyone is lying to you* (Phương pháp phỏng vấn kiểm chứng dựa trên hành vi quá khứ).
- Google PAIR (People + AI Research), *People + AI Guidebook* (Nguyên tắc thiết kế Augment vs. Automate và phân tích dạng lỗi sai).
- Anthropic (2024), *Building Effective Agents* (Khung phân định No AI vs. Rule vs. Workflow vs. Agent).
- Marty Cagan (2017), *Inspired: How to Create Tech Products Customers Love*, Silicon Valley Product Group (Khung đánh giá 4 rủi ro sản phẩm: Value, Usability, Feasibility, Viability).
