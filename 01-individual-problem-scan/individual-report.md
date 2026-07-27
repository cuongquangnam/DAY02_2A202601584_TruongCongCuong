# Case: Nhà đầu tư cá nhân nghiên cứu cổ phiếu Việt Nam trước khi quyết định mua/bán

**Nhân vật ví dụ:** An, 28 tuổi, nhân viên văn phòng, đầu tư chứng khoán Việt Nam khoảng 1–2 năm. Mỗi tuần An dành vài buổi tối để theo dõi thị trường: mở CafeF / Vietstock / TCBS / Facebook nhóm cổ phiếu, đọc tin, lướt báo cáo tài chính (BCTC), xem biểu đồ, rồi mới quyết định mua/bán hoặc giữ. An không phải chuyên gia phân tích; thường bị ngợp thông tin, dễ bỏ sót tin quan trọng, và hay mất nhiều thời gian trước khi “cảm thấy đủ chắc” để hành động.

## Vì sao đây là case tốt?

- Có actor cụ thể (An — nhà đầu tư cá nhân, không phải quỹ/analyst chuyên nghiệp).
- Có workflow lặp lại thật: đọc tin → tìm số liệu → đọc BCTC → so sánh → quyết định.
- Có bottleneck rõ (tổng hợp nhiều nguồn rời rạc thành insight đủ để quyết định).
- Có metric về thời gian nghiên cứu / lần quyết định.
- Có thể so sánh Rule / Workflow / Agent.
- Có thể vẽ before/after workflow.
- Domain gần với ý tưởng **Vietnam stock AI financial advisor** nhưng vẫn bắt đầu từ pain, không bắt đầu từ chatbot.

---

# 01 — Individual Problem Scan

## Scan rộng

Từ hành trình nghiên cứu cổ phiếu của An (và các nhà đầu tư cá nhân tương tự trên HOSE/HNX), scan ra 10 problems trong cùng case.

| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Tốn thời gian | Trước mỗi lần mua/bán, phải đọc tin + số liệu từ nhiều trang (CafeF, Vietstock, FireAnt, app CTCK) rồi tự tổng hợp | Nhà đầu tư cá nhân như An | 45–90 phút/lần nghiên cứu 1 mã; 2–4 lần/tuần |
| 2 | Tốn thời gian | Đọc báo cáo tài chính quý/năm (BCTC) dài, khó hiểu, phải tự tìm chỉ số quan trọng | Nhà đầu tư mới / bán chuyên | 30–60 phút/BCTC; hay bỏ cuộc giữa chừng |
| 3 | Lặp lại | Mỗi sáng/tối mở nhiều app để check giá, tin, khuyến nghị của cùng vài mã theo dõi | Nhà đầu tư cá nhân | 15–30 phút/ngày, lặp lại gần như mỗi phiên |
| 4 | AI có thể tốt hơn | App CTCK/broker chủ yếu hiện số và chart, ít giải thích “vì sao mã X biến động hôm nay” bằng ngôn ngữ dễ hiểu | Nhà đầu tư cá nhân | Biết giá tăng/giảm nhưng không nắm catalyst |
| 5 | AI có thể tốt hơn | Khó so sánh nhanh 3–5 mã cùng ngành (VD: ngân hàng, bất động sản) theo cùng bộ tiêu chí | Nhà đầu tư đang chọn mã | So sánh thủ công trên Excel hoặc mở nhiều tab |
| 6 | Pain từ người khác | Người mới hay hỏi lại cùng câu cơ bản (P/E là gì, nên đọc gì trước khi mua) trong nhóm Facebook/Discord | Nhà đầu tư mới, admin nhóm | Câu hỏi lặp lại mỗi đợt sóng mới |
| 7 | Pain từ người khác | Tin đồn / “call stock” trên Telegram/Facebook khiến người mới mua theo mà không có checklist kiểm chứng | Nhà đầu tư mới | Quyết định dựa rumor, thiếu bước lọc |
| 8 | Lặp lại | Cuối tuần tự viết nhật ký giao dịch / review danh mục: mã nào lãi-lỗ, vì sao giữ/bán | Nhà đầu tư có kỷ luật | 30–45 phút/tuần, hay trì hoãn |
| 9 | Tốn thời gian | Tìm lại thông tin cũ (nghị quyết ĐHĐCĐ, tin tăng vốn, kết quả kinh doanh quý trước) khi cần đối chiếu | Nhà đầu tư theo dõi dài hạn | 10–20 phút/lần tìm, nhiều nguồn không đồng bộ |
| 10 | AI có thể tốt hơn | Không có cảnh báo sớm theo ngữ cảnh cá nhân (VD: mã đang giữ có tin bất thường / vượt ngưỡng rủi ro tự đặt) | Nhà đầu tư đang nắm danh mục | Chỉ biết khi đã nhìn chart hoặc đọc tin muộn |

Ghi chú: thời gian ở bảng trên là ước lượng từ trải nghiệm quan sát / tự trải nghiệm của nhà đầu tư cá nhân, chưa phải số liệu khảo sát chính thức — sẽ validate thêm ở Phase 4 nếu nhóm chọn bài này.

### Nếu dùng AI ở phase này

Tôi tự đưa ra problem #1 (tổng hợp tin + số liệu trước khi quyết định) và #2 (đọc BCTC) từ trải nghiệm theo dõi chứng khoán VN trước. Sau đó dùng AI để mở rộng thêm các góc pain khác trong cùng case (so sánh mã, nhật ký giao dịch, tin đồn), rồi tự lọc bỏ ý quá rộng kiểu “AI tự trade thay người”. Số phút giữ dạng ước lượng, ghi rõ chưa khảo sát.

## Top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Tổng hợp tin + số liệu từ nhiều nguồn trước khi quyết định mua/bán | Workflow rõ, tốn nhiều thời gian, khớp trực tiếp với AI financial advisor, metric thời gian tốt | “Insight đủ tốt” đo thế nào ngoài thời gian? |
| 2 | Đọc và hiểu BCTC tiếng Việt trước khi đầu tư | Bottleneck cụ thể, AI mạnh ở tóm tắt/giải thích số liệu | Chất lượng tóm tắt tài chính sai thì rủi ro cao |
| 3 | So sánh nhanh nhiều mã cùng ngành theo cùng tiêu chí | Pain thật khi chọn mã, dễ vẽ before/after | Bộ tiêu chí chuẩn cho từng ngành chưa thống nhất |

## Problem Card #1 — Tổng hợp tin + số liệu trước khi quyết định

**Problem 1 câu:**  
Trước mỗi lần quyết định mua/bán một mã cổ phiếu Việt Nam, nhà đầu tư cá nhân như An mất khoảng 45–90 phút tự đọc và tổng hợp tin tức, giá, chỉ số từ nhiều nguồn rời rạc, trong đó bước “biến raw info thành insight đủ để quyết định” tốn nhất và dễ bỏ sót tin quan trọng.

**Actor:**  
Nhà đầu tư cá nhân (retail) trên thị trường chứng khoán Việt Nam, theo dõi vài mã, không phải analyst chuyên nghiệp.

**Thời điểm / bối cảnh:**  
Trước phiên giao dịch, hoặc khi có tin bất thường về mã đang quan tâm / đang nắm giữ.

**Current workflow:**

```text
1. Mở app CTCK xem giá / biến động trong ngày
2. Đọc tin trên CafeF / Vietstock / báo điện tử
3. Lướt nhóm Facebook / Telegram xem mọi người nói gì
4. Mở FireAnt / báo cáo để xem vài chỉ số cơ bản
5. Tự ghi chú / nhớ insight: catalyst, rủi ro, có mua/bán/giữ không
6. Quyết định hoặc trì hoãn vì chưa chắc
```

**Bottleneck:**  
Bước 5 — tổng hợp nhiều nguồn thành insight ngắn đủ để quyết định, mất khoảng 20–30 phút và dễ bỏ sót hoặc bị nhiễu bởi tin đồn.

**Impact:**  
45–90 phút/lần nghiên cứu × 2–4 lần/tuần ≈ 2–6 giờ/tuần cho 1 nhà đầu tư. Quyết định chậm hoặc dựa tin chưa kiểm chứng làm tăng rủi ro mua/bán sai thời điểm.

**Success metric:**  
Giảm thời gian nghiên cứu 1 mã từ 45–90 phút xuống dưới 20 phút; người dùng vẫn tự xác nhận trước khi đặt lệnh; không tăng tỷ lệ quyết định dựa tin đồn chưa kiểm nguồn.

**Non-AI alternative:**  
Watchlist cố định + checklist 5 câu hỏi (catalyst? định giá? rủi ro? thanh khoản? tin nguồn nào?) + bookmark 2–3 trang chính. Giảm loạn tab nhưng vẫn phải tự đọc và tự viết insight.

**AI hypothesis:**  
AI gom tin + số liệu đã chọn, draft bản tóm tắt có cấu trúc (catalyst, số liệu chính, rủi ro, câu hỏi còn mở). Nhà đầu tư review, kiểm nguồn, rồi mới quyết định — AI không đặt lệnh.

**Quick gut:**  
Workflow.

### Draft current workflow

```text
CURRENT STATE — 45–90 phút / mã

[1 Xem giá app CTCK: 5']
→ [2 Đọc tin CafeF/Vietstock: 15–25']
→ [3 Lướt nhóm MXH: 10']
→ [4 Xem chỉ số / chart: 10']
→ [5 Tự tổng hợp insight: 20–30']  <-- bottleneck
→ [6 Quyết định hoặc trì hoãn: 5']
```

### Draft future workflow

```text
FUTURE STATE — 15–20 phút / mã

[1 Chọn mã + khoảng thời gian quan tâm: 1']
→ [2 Auto-pull tin/số liệu từ nguồn đã chọn: 1']  -- Rule/script
→ [3 AI draft brief: catalyst, số liệu, rủi ro, nguồn: 1']  -- Workflow
→ [4 Nhà đầu tư review + mở link nguồn kiểm: 10–15']  <-- human boundary
→ [5 Quyết định mua/bán/giữ: 2']

Fallback:
AI tóm tắt thiếu/sai hoặc không cite nguồn
→ bỏ draft, quay lại đọc tay theo checklist.
```

---

## Problem Card #2 — Đọc và hiểu BCTC trước khi đầu tư

**Problem 1 câu:**  
Nhà đầu tư cá nhân muốn kiểm tra sức khỏe tài chính của doanh nghiệp niêm yết nhưng báo cáo tài chính quý/năm dài và khó hiểu, nên mất 30–60 phút/lần hoặc bỏ cuộc và quyết định mà thiếu bước đọc BCTC.

**Actor:**  
Nhà đầu tư cá nhân mới/trung bình, muốn phân tích cơ bản nhưng không quen đọc BCTC.

**Thời điểm / bối cảnh:**  
Khi sắp mua mã mới, hoặc sau khi doanh nghiệp công bố BCTC quý.

**Current workflow:**

```text
1. Tìm file/BCTC trên website công ty hoặc CafeF/Vietstock
2. Mở báo cáo (PDF/HTML), đọc lướt bảng cân đối / KQKD / lưu chuyển tiền tệ
3. Tự tính hoặc tìm vài chỉ số (doanh thu, lợi nhuận, nợ vay…)
4. Cố hiểu ý nghĩa (“lợi nhuận tăng nhưng dòng tiền sao?”)
5. Ghi chú ngắn hoặc bỏ cuộc vì quá dài
6. Quyết định mua/không mua (đôi khi thiếu bước này)
```

**Bottleneck:**  
Bước 2–4 — đọc và diễn giải BCTC bằng ngôn ngữ dễ hiểu, mất nhiều thời gian và dễ hiểu sai.

**Impact:**  
30–60 phút/BCTC; nhiều nhà đầu tư bỏ qua bước này → quyết định thiếu lớp kiểm tra cơ bản.

**Success metric:**  
Giảm thời gian nắm ý chính BCTC từ 30–60 phút xuống dưới 10 phút; người dùng vẫn mở được nguồn gốc số liệu; không dùng tóm tắt AI như lời khuyên mua/bán tuyệt đối.

**Non-AI alternative:**  
Template checklist chỉ số cố định (doanh thu YoY, biên LN, nợ/VCSH, dòng tiền HĐKD) + bookmark trang tóm tắt sẵn trên CafeF. Hữu ích nhưng ít giải thích “ý nghĩa trong ngữ cảnh ngành”.

**AI hypothesis:**  
AI tóm tắt BCTC theo checklist, giải thích thay đổi lớn bằng ngôn ngữ đơn giản, kèm câu hỏi cần kiểm thêm. Người dùng đối chiếu số liệu gốc trước khi dùng cho quyết định.

**Quick gut:**  
Workflow (cần Rule/checklist chặt vì domain tài chính nhạy cảm).

### Draft current workflow

```text
CURRENT STATE — 30–60 phút / BCTC

[1 Tìm BCTC: 5']
→ [2 Đọc lướt nhiều trang: 15–25']  <-- bottleneck
→ [3 Tự lọc chỉ số: 10']
→ [4 Cố hiểu ý nghĩa: 10–15']  <-- bottleneck
→ [5 Ghi chú / bỏ cuộc]
→ [6 Quyết định (đôi khi thiếu BCTC)]
```

### Draft future workflow

```text
FUTURE STATE — ~10 phút / BCTC

[1 Chọn mã + kỳ báo cáo: 1']
→ [2 AI tóm tắt theo checklist + highlight bất thường: 1']
→ [3 Nhà đầu tư đối chiếu 3–5 số liệu gốc: 7']  <-- human boundary
→ [4 Quyết định có cần đào sâu thêm không: 1']

Fallback:
Số liệu AI lệch hoặc không cite trang nguồn
→ không dùng tóm tắt; đọc tay theo checklist.
```

---

## Problem Card #3 — So sánh nhanh nhiều mã cùng ngành

**Problem 1 câu:**  
Khi cần chọn 1 trong 3–5 mã cùng ngành, nhà đầu tư cá nhân phải mở nhiều tab/Excel để tự xếp cùng bộ tiêu chí, mất 30–45 phút và dễ so sánh không nhất quán.

**Actor:**  
Nhà đầu tư cá nhân đang trong giai đoạn chọn mã / tái cơ cấu danh mục.

**Thời điểm / bối cảnh:**  
Khi muốn xoay vòng vốn trong cùng ngành (VD: chọn 1 ngân hàng, 1 cổ phiếu BĐS).

**Current workflow:**

```text
1. Liệt kê 3–5 mã ứng viên
2. Mở từng mã trên CafeF/FireAnt lấy P/E, ROE, biến động, tin gần đây
3. Tự ghi vào Excel/ghi chú
4. Cố chuẩn hóa tiêu chí (đôi khi đổi tiêu chí giữa chừng)
5. Chọn 1 mã “cảm thấy ổn nhất”
```

**Bottleneck:**  
Bước 2–4 — thu thập và chuẩn hóa dữ liệu so sánh thủ công.

**Impact:**  
30–45 phút/lần so sánh; quyết định dễ bị thiên lệch vì thiếu bảng so sánh thống nhất.

**Success metric:**  
Giảm thời gian so sánh 3–5 mã xuống dưới 10 phút; cùng một bộ tiêu chí cố định mỗi lần.

**Non-AI alternative:**  
Excel template cột cố định + copy số liệu tay. Đủ dùng nhưng vẫn tốn công nhập liệu.

**AI hypothesis:**  
AI (hoặc script + AI giải thích) tạo bảng so sánh theo checklist ngành, kèm 3–5 bullet “khác biệt đáng chú ý”. Người dùng chọn, không để AI xếp hạng “mua mã này”.

**Quick gut:**  
Rule + Workflow.

### Draft current workflow

```text
CURRENT STATE — 30–45 phút

[1 Liệt kê mã: 2']
→ [2 Mở từng mã lấy số liệu: 15–20']  <-- bottleneck
→ [3 Ghi Excel/ghi chú: 10']
→ [4 Tự chuẩn hóa tiêu chí: 5–10']
→ [5 Chọn mã]
```

### Draft future workflow

```text
FUTURE STATE — ~8–10 phút

[1 Nhập list mã + chọn bộ tiêu chí ngành: 1']
→ [2 Auto-pull số liệu vào bảng so sánh: 1']  -- Rule
→ [3 AI giải thích khác biệt đáng chú ý: 1']  -- Workflow
→ [4 Nhà đầu tư review bảng + quyết định: 5–7']  <-- human boundary

Fallback:
Thiếu dữ liệu hoặc chỉ số không đồng bộ nguồn
→ quay lại Excel template thủ công.
```

---

## Card muốn pitch nhất

```text
Problem Card #1 — Tổng hợp tin + số liệu từ nhiều nguồn trước khi quyết định mua/bán
```

Vì sao:

```text
Đây là pain gần nhất với ý tưởng Vietnam stock AI financial advisor, nhưng vẫn bắt đầu từ
workflow thật của nhà đầu tư cá nhân chứ không nhảy thẳng sang “làm chatbot khuyên mua/bán”.
Bottleneck rõ (bước tự tổng hợp insight), có metric thời gian, dễ vẽ before/after, và boundary
rất quan trọng trong tài chính: AI chỉ draft brief + cite nguồn, người thật quyết định và đặt lệnh.
```

Câu hỏi muốn nhóm challenge:

```text
1. Domain chứng khoán có rủi ro pháp lý / mis-selling — nhóm có nên siết boundary mạnh hơn
   (ví dụ: AI không được dùng động từ “nên mua/nên bán”) ngay từ Problem Statement không?
2. Thời gian 45–90 phút/lần là ước lượng của tôi — nếu chưa survey được, có đủ để pitch không,
   hay nên đổi metric sang “số nguồn phải mở” / “số lần bỏ sót tin quan trọng”?
3. Quick gut của tôi là Workflow; có ai nghĩ cần Agent (theo dõi liên tục + cảnh báo chủ động)
   ngay từ pilot không, hay Agent để giai đoạn sau?
```
