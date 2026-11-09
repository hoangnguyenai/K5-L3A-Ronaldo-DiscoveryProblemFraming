# Báo cáo cá nhân — 2A202603448_NguyenLamHoang

> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm.

## 1. Thông tin học viên

- Họ tên: Nguyễn Lâm Hoàng
- MSSV: 2A202603448
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Ronaldo
- Link repo nhóm: https://github.com/hoangnguyenai/K5-L3A-Day02-NguyenLamhHoang-2A202603448-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Pain từ người khác | Khi ăn uống xong cùng nhóm 9 người tại quán bia đông khách tối thứ Bảy, tôi muốn yêu cầu tính tiền được tiếp nhận và nhận bill sớm, để chủ động kết thúc buổi gặp | Khách ăn theo nhóm đông; nhân viên phục vụ và thu ngân phối hợp | Chờ mang bill: ~7 phút trong vùng chờ ~10–15 phút từ lần gọi đầu (mô phỏng; trải nghiệm thật chỉ xác định vùng chờ) |
| 2 | Tốn thời gian | Khi đặt đồ ăn giờ trưa trong ngày bận học/làm việc, tôi muốn biết đơn đang ở bước nào và có chậm không, để sắp xếp giờ ăn mà không kiểm tra liên tục | Người đặt đồ ăn; nhà hàng và shipper phối hợp | Chờ thụ động ~30 phút; phần có thể cải thiện trực tiếp là ~5 phút kiểm tra/liên hệ mỗi đơn |
| 3 | Pain từ người khác | Khi đến làm giấy tờ hoặc xin xác nhận, tôi muốn biết hồ sơ cần gì và còn phải chờ những bước nào, để hạn chế bổ sung giấy tờ và chủ động thời gian | Người làm thủ tục; nhân viên tiếp nhận phối hợp | Chờ lượt ~38 phút trong tổng ~60 phút (mô phỏng); nhánh bổ sung giấy tờ ~5 phút |
| 4 | Lặp lại | Khi nhận email thông báo của trường (deadline, học bổng, sự kiện) xen lẫn spam, tôi muốn phân biệt cái nào liên quan đến mình, để không bỏ lỡ deadline quan trọng | Sinh viên nhận thông báo | ~10–15 email/tuần; đã từng suýt bỏ lỡ 1 deadline trong học kỳ (số liệu cần kiểm lại theo trải nghiệm thật) |
| 5 | Tốn thời gian | Khi chuẩn bị nộp bài lab sát deadline, tôi muốn đối chiếu nhanh file sản phẩm với rubric, để không bị mất điểm oan do sai quy cách | Người phụ trách nộp bài của nhóm | ~45 phút/lần nộp, 1–2 lần/tuần; nhóm từng bị trừ 1.0 điểm ở Day 01 vì quên đổi tên file |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Bỏ ý "chatbot trả lời thắc mắc học tập 24/7"**: pain có thật nhưng là solution trá hình (chatbot), không phải pain cụ thể có thể đo được; nhóm đã loại ở CP1.
- **Bỏ ý "tự động phân chia task theo năng lực"**: solution trá hình, không có quy trình thật đằng sau, không đo được.
- **Bỏ ý "app theo dõi chi tiêu đa nền tảng"**: pain có thật nhưng đã có nhiều công cụ giải gần hết (Momo, Spendee), không còn bottleneck đáng đào sâu trong phạm vi lab.
- **Giữ ý "quán bia đông khách"**: pain có thật, trải nghiệm cụ thể với 9 người, bottleneck là khâu lập bill nằm ở phía nhà hàng — phù hợp để phản biện về scope kiểm soát.
- **Giữ ý "đặt đồ ăn giờ trưa"**: pain phổ biến, bottleneck là chờ thụ động và thiếu thông tin trạng thái đơn.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Chờ tính tiền quán bia đông khách | Pain có thật, trải nghiệm cụ thể với 9 người, bottleneck là khâu lập bill | Tần suất thấp, phần bottleneck nằm ở phía nhà hàng — ngoài tầm kiểm soát của nhóm |
| 2 | Chờ đồ ăn giờ trưa, không biết trạng thái đơn | Pain phổ biến, bottleneck rõ (5 phút kiểm tra/liên hệ), có thể so sánh No AI/Rule/AI | Phần lớn là chờ thụ động nằm ở phía nhà hàng/shipper |
| 3 | Làm giấy tờ/xác nhận, không biết còn thiếu gì | Pain phổ biến với sinh viên, bottleneck ~38 phút chờ lượt, có nhánh bổ sung giấy tờ | Số liệu là mô phỏng, chưa đo thực tế |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi ăn uống xong cùng nhóm 9 người tại quán bia đông khách tối thứ Bảy, tôi muốn yêu cầu tính tiền được tiếp nhận và nhận bill sớm, để chủ động kết thúc buổi gặp |
| Actor | Khách ăn theo nhóm đông; nhân viên phục vụ và thu ngân phối hợp |
| Thời điểm / bối cảnh | Buổi tối thứ Bảy, quán bia đông khách, nhóm ~9 người |
| Quy trình hiện tại (3–7 bước) | 1. Gọi nhân viên yêu cầu tính tiền → 2. Nhân viên tiếp nhận, đi vào quầy → 3. Thu ngân lập bill → 4. Nhân viên mang bill ra bàn → 5. Khách kiểm tra và thanh toán |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–4 — chờ mang bill: ~7 phút trong vùng chờ ~10–15 phút từ lần gọi đầu |
| Impact (nếu không giải thì sao) | Buổi gặp kéo dài thêm 10–15 phút không cần thiết; khách khó chủ động kết thúc |
| Success metric (baseline → target) | Thời gian từ gọi tính tiền đến nhận bill: baseline ~10–15 phút → target ≤ 3 phút |
| Phương án không dùng AI | Phân công một người theo dõi yêu cầu theo bàn / dùng nút gọi phục vụ có sẵn |
| Giả thuyết về AI (nếu có) | Không cần AI — pain nghiêng No AI/Rule |
| Cảm nhận nhanh | No AI / Rule |

Quy trình nháp hiện tại:

```text
[1] Gọi nhân viên yêu cầu tính tiền
      |
[2] Nhân viên tiếp nhận, đi vào quầy
      |
[3] Thu ngân lập bill
      |
[4] Nhân viên mang bill ra bàn  <<<< BOTTLENECK ~7' (vùng chờ 10-15')
      |
[5] Khách kiểm tra và thanh toán
Tổng phần chờ: ~10-15'/lần, tần suất thấp
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi đặt đồ ăn giờ trưa trong ngày bận học/làm việc, tôi muốn biết đơn đang ở bước nào và có chậm không, để sắp xếp giờ ăn mà không kiểm tra liên tục |
| Actor | Người đặt đồ ăn; nhà hàng và shipper phối hợp |
| Thời điểm / bối cảnh | Giờ trưa, ngày bận học/làm việc |
| Quy trình hiện tại (3–7 bước) | 1. Đặt đơn → 2. Chờ nhà hàng xác nhận → 3. Chờ chế biến → 4. Chờ shipper lấy đơn → 5. Chờ giao → 6. Kiểm tra liên tục xem đơn tới chưa |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 6 — kiểm tra/liên hệ mỗi đơn: ~5 phút trên tổng ~30 phút chờ thụ động |
| Impact (nếu không giải thì sao) | Mất thời gian kiểm tra liên tục; khó sắp xếp giờ ăn; đôi khi bỏ lỡ bữa |
| Success metric (baseline → target) | Thời gian kiểm tra/liên hệ mỗi đơn: baseline ~5 phút → target 0 phút (có thông báo tự động) |
| Phương án không dùng AI | App giao đồ ăn có sẵn đã có trạng thái đơn — chỉ cần bật thông báo |
| Giả thuyết về AI (nếu có) | Không cần AI — pain nghiêng No AI/Rule |
| Cảm nhận nhanh | No AI / Rule |

Quy trình nháp hiện tại:

```text
[1] Đặt đơn
      |
[2] Chờ nhà hàng xác nhận
      |
[3] Chờ chế biến
      |
[4] Chờ shipper lấy đơn
      |
[5] Chờ giao
      |
[6] KIỂM TRA LIÊN TỤC  <<<< BOTTLENECK ~5'/đơn
Tổng chờ thụ động: ~30'/đơn
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến làm giấy tờ hoặc xin xác nhận, tôi muốn biết hồ sơ cần gì và còn phải chờ những bước nào, để hạn chế bổ sung giấy tờ và chủ động thời gian |
| Actor | Người làm thủ tục; nhân viên tiếp nhận phối hợp |
| Thời điểm / bối cảnh | Đến cơ quan làm thủ tục hành chính |
| Quy trình hiện tại (3–7 bước) | 1. Hỏi nhân viên cần giấy tờ gì → 2. Chuẩn bị hồ sơ → 3. Nộp hồ sơ → 4. Chờ lượt xử lý → 5. Bổ sung giấy tờ nếu thiếu → 6. Nhận kết quả |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4 — chờ lượt: ~38 phút trong tổng ~60 phút; nhánh bổ sung giấy tờ ~5 phút |
| Impact (nếu không giải thì sao) | Mất ~60 phút/lần; bổ sung giấy tờ làm kéo dài thêm |
| Success metric (baseline → target) | Thời gian chờ + bổ sung: baseline ~60 phút → target ≤ 30 phút |
| Phương án không dùng AI | Checklist giấy tờ công khai trên website cơ quan; đặt lịch hẹn trước |
| Giả thuyết về AI (nếu có) | Không cần AI — pain nghiêng No AI/Rule |
| Cảm nhận nhanh | No AI / Rule |

Quy trình nháp hiện tại:

```text
[1] Hỏi nhân viên cần giấy tờ gì
      |
[2] Chuẩn bị hồ sơ
      |
[3] Nộp hồ sơ
      |
[4] CHỜ LƯỢT  <<<< BOTTLENECK ~38' (tổng ~60')
      |
[5] Bổ sung giấy tờ nếu thiếu (~5')
      |
[6] Nhận kết quả
```

### Card muốn pitch nhất

- Card số: **Card #1 (chờ tính tiền quán bia)**
- Vì sao: pain có thật, trải nghiệm cụ thể với 9 người, bottleneck là một bước rõ (khâu lập bill), phù hợp để phản biện về scope kiểm soát (phần bottleneck nằm ở phía nhà hàng).
- Câu hỏi muốn nhóm phản biện: "Nếu chỉ phân công một người theo dõi yêu cầu theo bàn thì đã đủ chưa, hay bottleneck thật nằm ở khâu lập bill của thu ngân?"

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1: pain có thật nhưng tần suất thấp và phần bottleneck nằm ở phía nhà hàng — nhóm không kiểm soát được; nghiêng No AI/Rule | Đồng ý | Giữ card ở mức No AI/Rule; dùng để phản biện về scope kiểm soát |
| Card #2: app giao đồ ăn đã có trạng thái đơn — pain đã được công cụ giải gần hết | Đồng ý | Giữ card ở mức No AI/Rule; nhấn mạnh phần cải thiện trực tiếp chỉ ~5 phút |
| Card #3: checklist giấy tờ công khai đã giải phần lớn — bottleneck chờ lượt nằm ở phía cơ quan | Đồng ý | Giữ card ở mức No AI/Rule; nhấn mạnh nhánh bổ sung giấy tờ ~5 phút |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch 3 card (quán bia, đồ ăn, thủ tục) — nội dung đã ghi ở dòng 4–6 bảng pitch mục 2.1 `group_report.md` | Đóng góp 3/12 candidate cho nhóm hội tụ; cả 3 candidate nghiêng No AI/Rule |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: "Nếu dùng script regex viết bằng Python kiểm tra tên file thì mất 3 giây, tại sao phải cần AI?" (tới Khoa, card #10) | Đẩy nhóm tách rõ Rule (tên file) vs AI (nội dung) — ảnh hưởng trực tiếp tới Problem Statement v1 |
| Nhận phản biện | Câu hỏi tôi nhận được: *(điền câu hỏi thật nhận được trong buổi pitch, ví dụ về tần suất pain quán bia và scope kiểm soát)* | Tôi đã sửa gì: chấp nhận rằng cả 3 candidate nghiêng No AI/Rule, nên ủng hộ chọn candidate #10 của Khoa |
| Gom cluster / cây OST | Tham gia gom cluster A (chuẩn trước deadline) và cây OST | Candidate #10 vào cluster A |
| Chọn candidate problem | Ủng hộ chọn #10 — rà soát rubric/checklist nộp bài | Candidate #10 được chọn (35 điểm) |
| Kiểm chứng / research | Tham gia research giải pháp đã có (mục 3.3 `group_report.md`): markdownlint, script bash `ls`, GitHub Actions | Kết luận: Rule xử lý hình thức, AI chỉ xử lý ngữ nghĩa |
| Quy trình nhóm | Tham gia viết quy trình trước/sau (mục 4 `group_report.md`) | Quy trình tương lai với Rule + Workflow + HITL |
| Problem Statement | Tham gia viết Problem Statement v0 (mục 5) và v1 (mục 7) | Boundary và AI intervention point rõ ràng |
| Mức can thiệp AI | Tham gia ma trận, so sánh 4 mức, AI Canvas (mục 6) | Chọn Workflow (Rule + AI + HITL) |
| Quyết định | Tham gia 4 rủi ro và quyết định Go (mục 8) | Go, phạm vi nhỏ |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tự scan trước (vài ý riêng), sau đó nhờ AI gợi ý thêm problems theo 4 lăng kính để đối chiếu góc nhìn | AI nêu được các góc pain mà mình chưa nghĩ tới (pain từ người khác: quán bia, thủ tục hành chính) và viết đúng format Job Story | Một số ý AI đưa ra là solution trá hình (chatbot, tự phân chia task) hoặc pain chung chung, không có con số đo được | Tự chọn giữ 5 ý mình thật sự gặp, bỏ các ý solution trá hình; tự điền dấu hiệu thật và kiểm tra không dòng nào có chữ "AI/chatbot/agent" trong cột Job Story |
| CP2 Problem Card | Tự viết 3 Problem Card và 3 quy trình nháp trước, rồi nhờ AI đóng vai "PM hoài nghi" phản biện từng card | AI chỉ ra được rằng app giao đồ ăn đã có trạng thái đơn (pain #2 gần như đã được công cụ giải) và checklist giấy tờ công khai đã giải phần lớn pain #3 | AI chưa đánh giá được tần suất pain trong bối cảnh cụ thể (quán bia chỉ xảy ra vài lần/năm); phần phản biện có chỗ hời hợt về scope kiểm soát | Tự chốt mức cảm nhận nhanh cho từng card (cả 3 ở mức No AI/Rule); viết sẵn câu hỏi phản biện để mang vào buổi pitch với nhóm |
| CP4 Research | Nhờ AI gợi ý các công cụ linter/markdown và case giải pháp đã có | AI nêu được markdownlint, GitHub Actions, script bash — giúp nhóm không nghĩ trong chân không | AI từng hallucination về tính năng của các công cụ linter — phải tự mở lại từng link GitHub để kiểm | Tự mở từng link kiểm chứng; kết luận Rule giải được phần hình thức, không giải được phần ngữ nghĩa |
| CP5 Quy trình | Nhờ AI chuyển mô tả quy trình sang Mermaid/ASCII | AI giúp vẽ nhanh sơ đồ trước/sau | AI hay gộp hai bước khác nhau thành một, làm mất bottleneck | Kiểm từng bước, giữ nguyên bottleneck rõ ràng (bước 3 rà soát nội dung) |
| CP5–6 Problem Statement | Nhờ AI phản biện Problem Statement v0 | AI chỉ ra trường nào còn mơ hồ, metric chưa đo được | AI có xu hướng viết lại thay nhóm thay vì chỉ đặt câu hỏi | Chỉ dùng AI để đặt câu hỏi và chỉ ra lỗ hổng, tự viết lại |
| CP6 Mức can thiệp / quyết định | Nhờ AI gợi ý các tiêu chí đánh giá đầu ra của AI | AI gợi ý được 5 tiêu chí (phát hiện mục trống, tỷ lệ báo nhầm, tôn trọng boundary, tốc độ, không chấm điểm chuyên môn) | AI có xu hướng đề xuất mức Agent — không phù hợp với bài này | Tự chốt mức Workflow (Rule + AI + HITL), không chọn Agent vì sát deadline rủi ro bằng 0 |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Tôi học được rằng cùng một nhóm nhưng mỗi người nhìn thấy pain ở những chỗ rất khác nhau: Trường nhìn thấy pain trong việc học (slide, citation, email), Trung nhìn thấy pain trong tự học (flashcard, tìm code, CV), Khoa nhìn thấy pain trong việc nộp bài và nghiên cứu. Điều đáng chú ý là candidate của Khoa (#10 rà soát rubric/checklist) dù không "hoành tráng" nhưng có bằng chứng thật (nhóm từng bị trừ 1.0 điểm) và quy trình rõ, nên dễ đo được. Tôi cũng nhận ra pain của mình (quán bia, đồ ăn, thủ tục) phần lớn nghiêng No AI/Rule vì bottleneck nằm ở phía bên ngoài (nhà hàng, cơ quan) mà nhóm không kiểm soát được. Đây là bài học quan trọng: pain có thật chưa đủ, phải xem nhóm có thể can thiệp vào bottleneck không.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có. Ở CP1, chính tôi đã có xu hướng nghĩ ngay đến "app theo dõi đơn đồ ăn" hay "chatbot lọc email" trước khi vẽ rõ quy trình. Nhóm nhận ra khi pitch: câu hỏi phản biện "Nếu chỉ phân công một người theo dõi yêu cầu theo bàn thì đã đủ chưa?" buộc phải thừa nhận rằng solution có sẵn (phân công, checklist) đã giải được phần lớn. Nhóm xử lý bằng cách ép mỗi candidate phải có "phương án không dùng AI" trong Problem Card, và chỉ chọn candidate nào mà Rule/No AI không đủ. Nhờ đó candidate #10 của Khoa được chọn vì bottleneck thật là rà soát nội dung markdown — bước mà mắt thường làm chậm và dễ sót, AI mới can thiệp được.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có. Ban đầu tôi pitch card #1 (quán bia) với ý rằng AI có thể giúp theo dõi yêu cầu tính tiền. Sau phản biện, tôi chấp nhận rằng tần suất pain thấp (không phải việc lặp lại hằng tuần) và phần bottleneck nằm ở phía nhà hàng — nhóm không kiểm soát được. Tôi đổi ý: không theo đuổi candidate này cho bài lab, thay vào đó ủng hộ candidate #10 của Khoa. Tôi cũng sửa câu hỏi phản biện của mình từ "AI có giúp không" sang "nếu script regex kiểm tra tên file mất 3 giây thì tại sao cần AI" — câu hỏi này sau đó được ghi nhận trong group_report và ảnh hưởng trực tiếp tới Problem Statement v1 (tách rõ Rule xử lý hình thức, AI chỉ xử lý ngữ nghĩa).

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Có bất ngờ. Phỏng vấn 2 sinh viên nhóm khác theo The Mom Test cho thấy họ đã có checklist in sẵn (in rubric ra giấy) — chứng tỏ công cụ không thiếu, giá trị phải nằm ở chỗ khác: sự an tâm trước khi bấm nộp. Điều này làm nhóm thu hẹp problem: phần kiểm tra tên file giao cho script Rule, chỉ tập trung đào sâu vào bước rà soát nội dung markdown tìm mục trống/placeholder. Research giải pháp đã có (markdownlint, script bash `ls`) cũng xác nhận: Rule giải được phần hình thức, không giải được phần ngữ nghĩa — đúng với giả định #2 (bottleneck là soát nội dung).

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Điều khó nhất là tách problem ra khỏi solution. Ban đầu tôi (và cả nhóm) có xu hướng viết "cần AI rà soát rubric" vào problem — nhưng Problem Statement phải mô tả đủ rõ để nhiều giải pháp khác nhau có thể được thử. Khó thứ hai là Success Metric: phải có baseline (đo được), target (muốn đạt) và cách đo (bấm giờ). Nếu không viết được metric đo được, bài toán chưa rõ ràng. Khó thứ ba là Boundary: phải nói rõ AI không được làm gì (không tự sửa file, không tự commit/push, không tự nộp bài) và khi nào cần con người kiểm tra (HITL bắt buộc).

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, tôi sẽ phản biện mạnh hơn ở hai điểm. Thứ nhất: ép mỗi candidate phải có số liệu thật (không phải ước lượng) ngay từ CP1 — nhiều card của tôi (quán bia, đồ ăn, thủ tục) chỉ là mô phỏng, chưa đo thực tế, nên dễ bị loại vì tần suất/thời gian không chắc. Thứ hai: tôi sẽ đặt câu hỏi phản biện sớm hơn về "ai kiểm soát bottleneck" — nếu bottleneck nằm ở phía bên ngoài (nhà hàng, cơ quan), thì pain khó can thiệp trong phạm vi lab và nên loại sớm. Tôi cũng sẽ tự phỏng vấn ít nhất 1 người ngoài nhóm cho candidate của mình thay vì chỉ dựa vào trải nghiệm cá nhân.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Nhóm chọn problem: khi chuẩn bị nộp bài lab/đồ án sát deadline, người phụ trách đóng gói và nộp bài muốn đối chiếu nhanh toàn bộ sản phẩm với rubric và checklist, để không bị mất điểm oan do sai quy cách format hoặc thiếu mục bắt buộc. Quy trình hiện tại 5 bước mất ~45 phút/lần, bottleneck là bước 3 rà soát nội dung markdown tìm mục trống/placeholder bằng mắt (~15 phút). Success Metric: thời gian rà soát từ ~45 phút xuống < 10 phút; lỗi quy cách/missing sau nộp từ 1 lỗi/3 lần xuống 0%. Boundary: AI chỉ đọc và xuất báo cáo cảnh báo, không sửa file, không commit/push, không nộp bài, không chấm điểm chuyên môn; con người duyệt từng cảnh báo (HITL bắt buộc). Mức can thiệp AI chọn: Workflow (script Rule kiểm tên file + LLM đọc markdown xuất báo cáo + con người duyệt). Quyết định: Go, phạm vi nhỏ, với pilot chạy trên chính repo Day 02 ở đợt nộp tiếp theo và ngưỡng dừng: nếu sau 2 tuần phát hiện < 80% lỗi thử nghiệm hoặc mất > 3 phút/lần chạy thì quay về checklist tay + script Rule.

---

## 7. Tài liệu tham khảo

- Design Council (UK), *Framework for Innovation* — Double Diamond: https://www.designcouncil.org.uk/resources/framework-for-innovation/
- Intercom — Job Stories: https://www.intercom.com/blog/accidentally-invented-job-stories/
- Teresa Torres — Opportunity Solution Trees: https://www.producttalk.org/opportunity-solution-trees/
- Rob Fitzpatrick, *The Mom Test*: https://www.momtestbook.com/
- Google PAIR — People + AI Guidebook, User Needs: https://pair.withgoogle.com/chapter/user-needs/
- Anthropic — Building Effective Agents: https://www.anthropic.com/research/building-effective-agents
- Marty Cagan — The Four Big Risks: https://www.svpg.com/four-big-risks/
- David Anson — markdownlint: https://github.com/DavidAnson/markdownlint
