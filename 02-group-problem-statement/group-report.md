## Thành viên nhóm B5

| STT | Họ và tên | Mã học viên | Vai trò |
|-----|------------------------|---------------|---------------------|
| 1 | Đặng Nguyên Giáp | 2A202601486 | Thành viên nhóm 1 |
| 2 | Mai Tuấn Quang | 2A202601484 | Thành viên nhóm 1 |
| 3 | Nguyễn Thị Thu Trang | 2A202601172 | Thành viên nhóm 1 |
| 4 | Phạm Thanh Hưng | 2A202601468 | Thành viên nhóm 2 |
| 5 | Nguyễn Thế Khiêm | 2A202601036 | Thành viên nhóm 2 |
| 6 | Phạm Minh Hiếu | 2A202601562 | Thành viên nhóm 2 |
| 7 | Đỗ Đức Tiến | 2A202601130 | Thành viên nhóm 3 |
| 8 | Nguyễn Thế Sơn | 2A202601632 | Thành viên nhóm 3 |
| 9 | Võ Quốc Huy | 2A202601110 | Thành viên nhóm 3 |
| 10 | Trương Công Cường | 2A202601584 | Thành viên nhóm 3 |
| 11 | Hoàng Thị Thuyên | 2A202601910 | Thành viên nhóm 4 |
| 12 | Dương Tiến Dũng | 2A202602020 | Thành viên nhóm 4 |
| 13 | Đặng Quang Trung | 2A202601510 | Thành viên nhóm 4 |

Note: Bàn B5 chia thành 4 nhóm, mỗi nhóm chọn ra 3 ý tưởng chính, sau đó tổng hợp lại thành một chủ đề là *AI Art Mentor*

# 02 — Group Problem Statement

Case nhóm chọn: **Đào tạo nhân viên mới tại phòng tranh nghệ thuật — AI Art Mentor**

Nhân vật tham chiếu: **Lan**, nhân viên tư vấn mới tại một phòng tranh nghệ thuật. Lan đã đọc tài liệu sản phẩm và quy trình bán hàng, nhưng kỹ năng tư vấn khách thực tế chỉ luyện được khi có khách đến gallery. Feedback từ quản lý đến muộn, không lặp lại được đúng tình huống — đôi khi phải đợi vài ngày mới gặp ca cần học.

---

## Group convergence

Nhóm 3–4 người, mỗi người share top 3. Tổng cộng 12 candidates từ 4 case khác nhau.

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh |
|---|---|---|---|---|---|
| 1 | Nhóm 1 | Đi lại nhiều lượt do thủ tục liên phòng ban (đất đai) | Người dân, cán bộ một cửa | Dò hỏi + bị đẩy qua phòng ban khác | Có số liệu thật, nhưng domain xa với nhóm |
| 2 | Nhóm 1 | Thiếu giấy tờ bị trả hồ sơ | Người dân lần đầu làm thủ tục | Phát hiện thiếu sau khi đã đến nộp | Pain rõ, nhưng cần data quy định pháp lý |
| 3 | Nhóm 1 | Cán bộ giải thích lặp lại cùng câu hỏi | Cán bộ một cửa | Giải thích miệng lặp lại mỗi ngày | Pattern giống onboarding, nhưng bối cảnh hành chính |
| 4 | Nhóm 2 | Khách hotline lặp lại thông tin khi chuyển máy | Khách hàng, tổng đài viên | Khách phải trình bày lại mỗi lần chuyển | Workflow rõ, metric tốt |
| 5 | Nhóm 2 | Tìm tài liệu nội bộ theo mô tả tự nhiên | Nhân viên văn phòng | Search keyword không ra đúng nội dung | Impact rộng, scope data lớn |
| 6 | Nhóm 2 | CSKH tự đọc và định tuyến yêu cầu | CSKH, các phòng ban | Đọc + phân loại thủ công | AI có thể hỗ trợ, nhưng quality metric khó |
| 7 | Nhóm 3 | Nhân viên mới chỉ luyện tư vấn khi có khách thật | Nhân viên tư vấn mới, quản lý gallery | Gặp khách → tư vấn → góp ý: không lặp lại được | Workflow onboarding rõ, có thể pilot A/B |
| 8 | Nhóm 3 | Feedback quản lý đến muộn, không kiểm soát được tình huống luyện | Nhân viên mới | Chờ ca khách phù hợp để học | Pain lặp lại mỗi đợt tuyển |
| 9 | Nhóm 3 | Kiến thức nghệ thuật + kỹ năng bán chưa được chuẩn hóa giữa nhân viên | Quản lý, khách hàng | Tự học từ tài liệu, thiếu luyện tập có cấu trúc | AI có thể hỗ trợ Q&A + role-play |
| 10 | Nhóm 4 | Sinh viên mất nhiều thời gian để đọc, tóm tắt và tổng hợp tài liệu học tập trước khi học hoặc ôn thi | Sinh viên đại học | Phải đọc toàn bộ PDF/slide rồi tự chọn lọc ý chính, ghi chú thủ công, rất tốn thời gian | Workflow rõ, AI phù hợp để tóm tắt; dễ đo bằng thời gian đọc |
| 11 | Nhóm 4 | Sinh viên gặp khó khăn trong việc tìm đúng tài liệu học tập giữa rất nhiều nguồn khác nhau | Sinh viên đại học | Có quá nhiều tài liệu trên LMS, Google Drive, GitHub… nhưng không biết tài liệu nào phù hợp và cập nhật | AI có thể đề xuất tài liệu phù hợp theo môn học; workflow rõ |
| 12 | Nhóm 4 | Sinh viên mất nhiều thời gian ôn tập trước kỳ thi vì phải đọc lại toàn bộ tài liệu và ghi chú | Sinh viên đại học | Phải tổng hợp lại kiến thức từ nhiều nguồn và tự làm đề cương ôn tập | AI có thể tạo đề cương, flashcard và câu hỏi ôn; dễ đánh giá bằng thời gian chuẩn bị |

### Cluster

| Cluster | Candidate examples | Pattern chung |
|---|---|---|
| **Onboarding / đào tạo kỹ năng** | Gallery onboarding, cán bộ giải thích lặp, nhân viên mới hỏi quy trình | Người mới cần luyện tập lặp lại, nhưng phụ thuộc vào người có kinh nghiệm hoặc tình huống thật |
| **Tìm kiếm / hỏi đáp thông tin** | Tìm tài liệu nội bộ, thiếu giấy tờ thủ tục, kiến thức nghệ thuật gallery, tìm tài liệu học tập | Cần tra đúng thông tin theo ngữ cảnh, không chỉ keyword |
| **Handoff / chuyển tiếp mất context** | Hotline chuyển máy, thủ tục liên phòng ban | Thông tin không được truyền sang bước tiếp theo, người sau phải bắt đầu lại |
| **Phân loại / định tuyến** | CSKH route yêu cầu | Đọc nội dung rồi quyết định chuyển đúng chỗ |
| **Học tập / tổng hợp tài liệu** | Tóm tắt PDF/slide, ôn thi, tạo đề cương | Gom nhiều nguồn học thành insight ngắn để học/ôn nhanh hơn |

---

## Shortlist và score

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **Gallery — AI Art Mentor** | 5 | 5 | 4 | 4 | 5 | 5 | 5 | **33** |
| Hotline lặp thông tin khi chuyển máy | 5 | 5 | 4 | 4 | 4 | 4 | 4 | 30 |
| Thủ tục liên phòng ban (đất đai) | 4 | 5 | 5 | 5 | 2 | 4 | 2 | 27 |
| Tóm tắt / ôn tập tài liệu học tập | 5 | 4 | 4 | 4 | 5 | 4 | 5 | 31 |
| Tìm tài liệu nội bộ | 4 | 4 | 3 | 4 | 3 | 4 | 3 | 25 |

Nhóm chọn: **Đào tạo nhân viên mới tại phòng tranh — AI Art Mentor (luyện tư vấn trước khi gặp khách thật).**

Vì sao chọn:

- Có actor cụ thể (nhân viên tư vấn mới như Lan), workflow onboarding lặp lại mỗi đợt tuyển.
- Bottleneck rõ: **gặp khách thật → tư vấn → nhận góp ý** — không lặp lại được, không kiểm soát tình huống.
- Có metric đo được: thời gian onboarding, feedback khách, tỉ lệ chốt deal (đề xuất A/B test trong slide nhóm).
- Nhóm có case tham chiếu và slide giải pháp ([Case ví dụ: Đào tạo nhân viên mới tại phòng tranh nghệ thuật](https://docs.google.com/document/d/1hfgU-bog7hmhO_ZPbJz9GtVyTBYQj7zHVE_KkwE_9d4/edit?usp=sharing)), dễ vẽ before/after và so sánh Rule / Workflow / Agent.
- Pattern onboarding + role-play khớp với nhiều tool đã có trên thị trường, research không phải bắt đầu từ zero.

Vì sao không chọn các bài khác:

- **Hotline chuyển máy:** workflow rõ nhưng cần tích hợp hệ thống tổng đài/CRM thật, khó pilot trong lab.
- **Thủ tục đất đai:** có số liệu mạnh (Nghị định 151/2025, PAPI 2024) nhưng domain pháp lý xa, nhóm không ai am hiểu sâu workflow UBND.
- **Tóm tắt / ôn tập tài liệu học tập:** gần với sinh viên, dễ làm lab, nhưng pain thiên về “đọc-tóm tắt” hơn là luyện kỹ năng tương tác; nhóm muốn bài có role-play + human boundary rõ hơn.
- **Tìm tài liệu nội bộ:** impact rộng nhưng data access và index toàn bộ file khó làm trong thời gian lab.

Nếu có disagreement, nhóm xử lý thế nào:

- Bài hotline, học tập và gallery đều điểm cao. Nhóm vote theo tiêu chí **"làm được pilot nhỏ trong lab" + có bước luyện tương tác thật** — gallery thắng vì có thể role-play bằng prompt + checklist mà không cần hệ thống doanh nghiệp, đồng thời khác với bài tóm tắt tài liệu thuần túy.

---

## Quick validation

Nhóm hỏi nhanh 3 người có kinh nghiệm bán hàng dịch vụ / retail / gallery (quen biết + poll mini trong lớp).

| Nguồn | Số người | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Quick interview | 3 | 2/3 từng onboard nhân viên mới; đều nói phần khó nhất là **luyện tình huống thật**, không phải đọc tài liệu | 1 người nói shadow senior vài tuần là đủ | Thu hẹp: không phải "thay toàn bộ đào tạo", mà là **luyện tư vấn + role-play trước khi gặp khách** |
| Mini poll trong lớp | 6 | 4/6 từng phải học kỹ năng giao tiếp/bán hàng qua tình huống thật | 2 người chưa từng làm sales | Thêm non-AI alternative: shadow senior + tài liệu in sẵn |
| Case tham chiếu (Google Doc) | 1 case | Mô tả rõ pain "chỉ luyện được khi có khách thật", feedback muộn | Chưa có số liệu thời gian chính thức từ gallery thật | Giữ metric dạng ước lượng có ghi chú "cần đo thêm ở pilot" |

Insight sau validation:

```text
Pain thật không nằm ở việc "thiếu tài liệu". Pain nằm ở đoạn luyện tập tư vấn:
không lặp lại được đúng tình huống, không kiểm soát được ca khó, và phải chờ khách thật
hoặc quản lý rảnh mới có feedback.
```

---

## Research giải pháp

Nhóm tìm các hướng đã có sẵn, không giả định phải tự build agent từ đầu.

| Nguồn / tool / case | Link | Họ giải quyết phần nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Prestance (AI sales coach retail) | https://prestancelab.com/ | Role-play hằng ngày theo brand voice, brief trước ca VIP | Tập trung retail, luyện objection ("quá đắt") | Không chuyên gallery/nghệ thuật | Pattern: coach pocket-size, luyện nhiều lần trước ca thật |
| UMU AI Roleplay Chatbot | https://www.umu.com/product/ai-roleplay-chatbot | Simulation + scoring competency cho onboarding | On-demand, có điểm readiness | Cần customize scenario theo domain gallery | Workflow phù hợp: AI role-play → người review → field-ready |
| Emerse.ai | https://www.emerse.ai/ | Role-play video avatar, retail + objection handling | Browser-based, không cần VR | Generic sales, chưa có art analysis | AI draft scenario + feedback, manager vẫn set chuẩn |
| ARTERNAL — Sal (gallery AI agent) | https://observer.com/2026/07/arts-sean-green-arternal-ai-agents-galleries-reggie-sal/ | Brief staff, draft email, sales funnel gallery | Domain gallery thật | Tập trung CRM/sales ops hơn là onboarding kỹ năng tư vấn | Gallery đã có nhu cầu AI; onboarding vẫn là khoảng trống riêng |

Research takeaway:

```text
Không nên build một agent tự chạy toàn bộ đào tạo ngay. Hướng hợp lý hơn là Workflow:
tài liệu + checklist (Rule) → AI Q&A kiến thức → AI role-play khách → nhân viên + quản lý review.
Agent chỉ cần khi muốn tự điều chỉnh lộ trình và scenario theo điểm yếu từng người.
```

---

## Workflow before/after

```text
CURRENT STATE — 6 bước, ~3-4 tuần onboarding (ước lượng)

[1 Đọc tài liệu sản phẩm/nghệ thuật: 2-3 ngày]
→ [2 Shadow senior khi có khách: không kiểm soát ca]
→ [3 Gặp khách thật lần đầu tư vấn: 20-40'/khách]  <-- phụ thuộc foot traffic
→ [4 Quản lý quan sát + góp ý sau ca: 15-30', có thể trễ vài ngày]  <-- bottleneck
→ [5 Tự học lại từ góp ý: 30-60'/lần]
→ [6 Lặp lại đến khi đủ tự tin: 2-4 tuần]

FUTURE STATE — 6 bước, ~1-2 tuần onboarding (kỳ vọng)

[1 Đọc tài liệu + AI kiểm tra kiến thức đầu vào: 1 ngày]  -- Rule + Workflow
→ [2 AI thiết kế lộ trình cá nhân theo điểm yếu: 30']      -- Workflow
→ [3 AI Q&A kiến thức nghệ thuật/sản phẩm: on-demand]       -- Workflow
→ [4 AI role-play khách (price objection, so sánh tác phẩm): 15-20'/session]  -- Workflow
→ [5 Quản lý review điểm kỹ năng + xác nhận field-ready: 30']  -- Human boundary
→ [6 Gặp khách thật với confidence cao hơn]

Fallback:
AI role-play sai ngữ cảnh nghệ thuật hoặc đề xuất giá sai
→ nhân viên bỏ scenario, quản lý chạy role-play thủ công hoặc shadow senior như cũ.

Bottleneck mới:
Quản lý review + xác nhận field-ready. Đây là bottleneck chấp nhận được vì đó là điểm kiểm soát chất lượng trước khi chốt khách thật.
```

Before/after impact:

| Metric | Trước | Sau kỳ vọng | Ghi chú |
|---|---:|---:|---|
| Thời gian onboarding | 3-4 tuần | 1-2 tuần | Target chính (A/B với nhóm đào tạo truyền thống) |
| Số lần luyện tư vấn/tuần | Phụ thuộc khách thật (2-5 ca) | 10-15 session AI + 2-3 ca thật | AI bù phần không kiểm soát được |
| Thời gian chờ feedback | Vài giờ → vài ngày | Ngay sau mỗi session role-play | AI feedback tức thì, quản lý review định kỳ |
| Tỉ lệ chốt deal (nhân viên mới) | Baseline chưa đo | Cải thiện so với nhóm A | Cần A/B test thực tế — chưa verify |
| Risk mới | Không có AI hallucination | AI bịa thông tin nghệ thuật/giá | Cần quản lý review trước field-ready |

---

## Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | Nhân viên tư vấn mới tại phòng tranh nghệ thuật (ví dụ Lan), và quản lý gallery chịu trách nhiệm onboard. |
| **Workflow** | Nhân viên mới đọc tài liệu → shadow/gặp khách thật → tư vấn → nhận góp ý quản lý → tự học lại → lặp đến khi đủ tự tin. |
| **Bottleneck** | Bước **gặp khách thật → tư vấn → góp ý**: không lặp lại được đúng tình huống, feedback đến muộn, phụ thuộc foot traffic và lịch quản lý. |
| **Impact** | Onboarding kéo dài 3-4 tuần (ước lượng); nhân viên mới dễ lúng túng trước objection; quản lý tốn thời gian góp ý lặp lại; trải nghiệm khách có thể kém trong giai đoạn đầu. |
| **Success Metric** | Giảm thời gian onboarding từ 3-4 tuần xuống 1-2 tuần; tăng số session luyện tư vấn/tuần; không giảm feedback tích cực từ khách (A/B: nhóm B dùng AI Art Mentor vs nhóm A truyền thống). |
| **Boundary** | AI không thay nhân viên chốt deal với khách thật; không tự bịa giá/tác giả/lịch sử tác phẩm; không gửi thông tin cho khách mà chưa qua quản lý duyệt. |

---

## Rule / Workflow / Agent

| Mức | Phương án | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| **Rule** | Tài liệu in sẵn, checklist tư vấn, script objection, shadow senior cố định | Đủ nếu chỉ cần truyền kiến thức nền | Không giải quyết luyện tập lặp lại và feedback tức thì | Không chọn làm toàn bộ, nhưng dùng cho bước kiến thức nền |
| **Workflow** | AI kiểm tra kiến thức → AI Q&A → AI role-play khách → scoring → quản lý review field-ready | Hợp vì workflow tuyến tính, AI hỗ trợ các bước ngôn ngữ/tình huống | Role-play sai ngữ cảnh nghệ thuật, cần quản lý review | **Chọn** |
| **Agent** | Agent tự thiết kế lộ trình, chọn scenario, điều chỉnh độ khó, nhắc luyện tập theo điểm yếu | Cần khi muốn cá nhân hóa sâu và tự điều phối nhiều bước | Phức tạp hơn cần thiết cho pilot lab; cần data lịch sử luyện tập | Chưa chọn — có thể mở rộng sau pilot Workflow |

Mức chọn:

```text
Workflow (có thể tiến tới Agent ở giai đoạn 2 nếu pilot Workflow ổn).
```

Vì sao:

- Kiến thức nền có thể dùng Rule (checklist, tài liệu).
- Luyện tư vấn và role-play cần AI hiểu ngôn ngữ + mô phỏng khách.
- Quản lý vẫn xác nhận field-ready nên risk kiểm soát được.
- Agent chưa cần ngay vì pilot lab có thể chạy workflow cố định: Q&A → role-play → review.

---

## Problem Statement v1

| Field | Nội dung |
|---|---|
| **Actor** | Nhân viên tư vấn mới tại phòng tranh nghệ thuật; quản lý gallery xác nhận readiness trước khi nhân viên tư vấn độc lập. |
| **Workflow** | Đọc tài liệu → (hiện tại) gặp khách thật → tư vấn → góp ý quản lý → tự học; (tương lai) thêm AI kiểm tra kiến thức, Q&A, role-play, scoring trước bước gặp khách thật. |
| **Bottleneck** | Luyện tư vấn phụ thuộc khách thật và feedback quản lý muộn — không lặp lại được scenario cần học (objection giá, so sánh tác phẩm, khách first-time buyer). |
| **Impact** | Onboarding ~3-4 tuần; nhân viên mới thiếu confidence; quản lý lặp góp ý; khách có thể gặp tư vấn chưa sẵn sàng. |
| **Success Metric** | Giảm onboarding xuống 1-2 tuần; ≥10 session role-play/tuần/người; feedback khách và tỉ lệ chốt deal nhóm B ≥ nhóm A trong A/B test cùng giai đoạn. |
| **Boundary** | AI không tư vấn/giá thay nhân viên với khách thật; không bịa thông tin tác phẩm; quản lý duyệt trước khi coi nhân viên field-ready. |
| **AI intervention point** | Sau khi nhân viên đọc tài liệu nền, **trước** khi tư vấn khách thật độc lập: kiểm tra kiến thức, Q&A, role-play, tổng hợp điểm kỹ năng. |
| **Mức chọn** | Workflow: Rule cho tài liệu/checklist, AI cho Q&A + role-play + scoring, quản lý review field-ready. |
| **Rủi ro & người thật kiểm tra** | Risk: hallucination về nghệ thuật/giá, role-play quá generic, nhân viên phụ thuộc AI. Người thật kiểm tra: quản lý review điểm kỹ năng và xác nhận trước khi nhân viên tư vấn khách thật solo. |

---

## Final decision

Decision:

```text
Go với scope nhỏ — pilot AI Art Mentor cho 1 nhóm nhân viên mới.
```

Pilot nhỏ nhất:

- Chọn 4-6 nhân viên mới, chia A/B: nhóm A đào tạo truyền thống, nhóm B thêm AI Art Mentor (Q&A + role-play 3 scenario cố định: objection giá, so sánh 2 tác phẩm, khách lần đầu mua tranh).
- Chạy workflow bán thủ công: quản lý paste tài liệu gallery vào prompt chuẩn; nhân viên luyện role-play; AI chấm điểm theo rubric; quản lý review 1 lần/tuần.
- Đo: thời gian onboarding, số session/tuần, feedback khách, tỉ lệ chốt deal (nếu có đủ mẫu).

Exit / rollback:

- Nếu sau 2 tuần nhóm B vẫn cần quản lý sửa >50% nội dung role-play hoặc điểm kỹ năng không cao hơn nhóm A → hạ xuống Rule (checklist + shadow senior), bỏ role-play AI.
- Nếu AI bịa thông tin tác phẩm/giá → không cho dùng Q&A tự do; chỉ dùng scenario có script quản lý duyệt trước.

Decision rationale:

- Problem rõ, workflow rõ, metric rõ (thời gian onboarding + A/B).
- Có non-AI components (tài liệu, shadow, quản lý review).
- AI nằm ở bước luyện tập cụ thể, không thay nhân viên chốt deal.
- Research cho thấy pattern role-play + scoring đã có trên thị trường; gallery case ([Google Doc tham chiếu](https://docs.google.com/document/d/1hfgU-bog7hmhO_ZPbJz9GtVyTBYQj7zHVE_KkwE_9d4/edit?usp=sharing)) và slide AI Art Mentor khớp hướng này.

---

*Nhóm Day 02 — Case: Đào tạo nhân viên mới tại phòng tranh nghệ thuật / AI Art Mentor*
