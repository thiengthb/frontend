# M0-01 — Chẩn đoán điểm xuất phát (baseline)

- **Ngày:** 2026-10-30
- **Trạng thái:** xong phần chẩn đoán. Chờ người dùng phản biện lại (bước 3 của Lesson Loop)
- **Người chấm:** Claude, đóng vai người phê bình khắt khe. Không chấm theo cảm xúc của người được chấm.
- **Bằng chứng đã đọc:**
  - `prm323-lab2-SE190533`: toàn bộ `design/`, `process/retro-v1.md`, 53 ảnh trong `assets/figma/` (bản teal 22/10), cùng **ảnh chụp trực tiếp từ file Figma hiện tại** (bản cam, Nunito, "Nổi khối"): GV-001, GV-102 .D2, GV-103 .D
  - `sakubun`: `app/globals.css`, `docs/ui-standard.md`, `lib/design/*`, ảnh trong `public/screens/` và `docs/plans/2026-10-28-ui-kaiwa-library/`
  - `thienui`: README, `packages/ui-patterns/src/ui-patterns.json` (37 luật), `registry/lib/motion*.ts`
- **Giới hạn:** mình không chạy được app, nên mọi nhận xét về tương tác và chuyển động dựa trên code và ảnh tĩnh, không phải cảm nhận khi dùng thật.

---

## 0. Kết luận một câu

> **Bạn là một kỹ sư hệ thống rất giỏi đang đóng vai nhà thiết kế.** Bạn tối ưu cho việc *không có lỗi*
> (kiểm contrast, kiểm token, danh sách nợ, guard, checklist 90/100), nhưng chưa tối ưu cho việc *có chất lượng*
> (điểm nhấn, nhịp điệu, tương phản tỉ lệ, cá tính, cảm xúc). Mọi công cụ bạn dựng đều đo được cái **sai**,
> nhưng không cái nào đo được cái **hay**. Vì vậy sản phẩm của bạn **đúng, sạch, nhất quán, và nhạt**.

Thầy nói "đơn điệu" là đúng. Nhưng đơn thuốc 70-20-10 chỉ chữa được khoảng 30% căn bệnh. Phần còn lại nằm ở bố cục và tỉ lệ.

---

## 1. Điểm mạnh thật (giữ lại, đừng đánh mất)

Phần này không phải để an ủi. Đây là những thứ hiếm có, và chúng sẽ là nền móng:

| # | Điểm mạnh | Bằng chứng |
|---|---|---|
| S1 | **Tư duy hệ thống**: token ba tầng, sinh theme bằng thay ramp, ranh giới vendor | thienui README; theme `slate` sinh từ `claude` không sửa tay dòng nào |
| S2 | **Phủ trạng thái**: loading, empty, error, offline, lần đầu (E2) | Figma GV-001 có .D .D1 .L .E .X .E2; luật `every-state-designed` |
| S3 | **Kỷ luật trợ năng**: tự tính contrast WCAG, vùng chạm 44/48, focus ring | DESIGN.md mục 3; guards contrast 296 cặp |
| S4 | **Biết tự sửa quy trình**: retro v1 thẳng thắn (phỏng vấn giả bằng AI, viết để chứng minh) | `process/retro-v1.md` |
| S5 | **Luật được ép bằng máy**, không bằng lời nhắc | `lib/design/*.test.ts`, debt list chỉ giảm |

Sinh viên năm 2–3 có S2, S3 và S5 là cực hiếm. **Nhưng chính S5 là nơi sinh ra điểm yếu lớn nhất** (xem W1).

---

## 2. Điểm yếu, xếp theo mức độ nghiêm trọng

### W1 — Đo cái sai thay vì tạo cái hay *(gốc rễ)*
- Bản thân bạn đã ghi trong DESIGN.md v3.0: *"bản Xanh đại dương **đúng luật nhưng vẫn nhạt**"*. Đây là câu quan trọng nhất trong cả ba repo. Bạn đã thấy bệnh.
- **Nhưng cách chữa của bạn là đổi màu nhấn** (teal → cam) và thêm viền 2px. Bố cục, tỉ lệ và nhịp điệu gần như giữ nguyên. So ảnh `412-GV-001.D` (teal) với Figma GV-001 .D (cam): vẫn là cùng một chồng thẻ trắng xếp dọc, chỉ khác màu nhấn.
- Checklist "UI Simplicity" chấm 90/100, nhưng toàn bộ tiêu chí trong đó đều là **tiêu chí loại trừ**: không lặp, không chữ dài, không nhiều màu. Không có tiêu chí nào hỏi *"màn này có một khoảnh khắc nào đáng nhớ không?"*. Một màn trắng trống trơn cũng đạt gần 100 điểm trên bảng đó.
- 37 luật thienui cùng ui-standard của sakubun **gần như toàn bộ là luật cấp control**: icon 16px, nút 28/36px, bo 8, đậm 500. **Không có một luật nào ở cấp trang**: điểm nhấn của trang là gì, nhịp giữa các section, tỉ lệ giữa khối lớn và khối nhỏ.

> **Chân lý cần thấm:** *Checklist đảm bảo sàn, không tạo trần.* "Không sai" là điều kiện cần, không phải đủ.

### W2 — "Nhất quán" bị hiểu thành "đồng phục" → triệt tiêu tương phản
Từng quyết định dưới đây đều có lý khi đứng riêng. Cộng lại, chúng xoá sạch mọi đòn bẩy phân cấp:

| Đòn bẩy | Bạn đã khoá thành | Hệ quả |
|---|---|---|
| Bo góc | sakubun: `radius-sm = md = lg = xl = 2xl = 0.5rem` (6 token, 1 giá trị) | Thẻ, nút, dialog, chip trông như cùng một loại vật |
| Cỡ icon | thienui `icon-size-scale`: **chỉ một cỡ** 16px | Icon không bao giờ làm điểm nhấn được |
| Độ đậm | sakubun: `--font-weight-bold: 600` và control luôn 500 | Dải đậm thực tế chỉ còn 500–700, gần như không phân biệt được |
| Cỡ chữ | sakubun: **tiêu đề phần 14px = nội dung 14px**, chỉ khác độ đậm | Mắt không thấy ranh giới section |
| Cỡ chữ (lab2) | 9 kiểu, nhưng trên màn chủ yếu 13–17px; title 22 → section 16 → body 15 | Tỉ lệ bước chỉ ~1.07 → cảm giác "phẳng" |
| Độ nổi | lab2 và sakubun: **mọi thẻ, nút, chip đều có gờ đáy 2px** | *Mọi thứ đều nổi = không gì nổi* (Von Restorff bị vô hiệu) |
| Khoảng cách | lab2: thẻ cách thẻ 8–12, nhóm cách nhóm 16–24 | Khoảng cách trong nhóm và giữa nhóm quá gần nhau → nhịp đều đều |

> **Chân lý cần thấm:** *Nhất quán là dùng cùng một thang. Đồng phục là chỉ dùng một bậc của thang.*
> Hệ tốt có ít bậc, nhưng các bậc phải **cách xa nhau** (ví dụ chữ 14 / 20 / 32, chứ không phải 14 / 15 / 16 / 17).

### W3 — Phản xạ "lưới thẻ KPI" và thiếu hành động chính
- **lab2 GV-001 (bản cam):** bốn ô số bằng nhau (4 lớp · 131 sinh viên · 94% · 2 yêu cầu) chiếm **màn hình đầu tiên** của giảng viên lúc 7:05 sáng. Trong khi đó, việc duy nhất họ cần làm lúc ấy là *mở điểm danh slot đang diễn ra*. "131 sinh viên" không giúp được quyết định nào. Đây là **vanity metric**, và nó đẩy thẻ slot quan trọng nhất xuống dưới. Bản teal trước đó **đúng hơn** (slot đang diễn ra nằm trên cùng). Bạn đã đi lùi về UX khi đi tới về "đỡ nhạt".
- **sakubun Phân tích:** lại là bốn ô KPI bằng nhau, rồi một banner dài, rồi tiến độ, rồi heatmap. Trong viewport đầu tiên **không có nút "Ôn ngay"**, dù "26 đến hạn bây giờ" là con số quan trọng nhất. Người học mở app để học, không phải để đọc báo cáo.
- Cả hai project, cùng một phản xạ. Đây là **mặc định của AI và của shadcn dashboard template**, không phải một quyết định thiết kế.

> **Chân lý cần thấm:** *Màn hình bắt đầu từ hành động, không bắt đầu từ dữ liệu.* Câu hỏi đầu tiên luôn là "người này mở màn này để LÀM gì?"

### W4 — Mượn bề mặt của tham chiếu, bỏ lại hệ thống phía sau
- **"Nổi khối kiểu Duolingo"**: Duolingo là gờ dày **đi cùng** minh hoạ nhân vật, nhiều màu bão hoà, chữ rất to và rất đậm, chuyển động nảy, âm thanh. Bạn lấy đúng cái gờ 2px rồi cấm minh hoạ, cấm nhiều màu và dùng chữ 15px. Kết quả là đồ chơi không có niềm vui: nặng nề nhưng không vui.
- **Thang chữ sakubun** dùng tên của Apple HIG (`caption2`, `footnote`, `subhead`, `title3`, `large-title`) nhưng luật trang chỉ dùng 12 / 14 / 18–24. Bạn chép **tên** của thang, không chép **cách dùng** của nó.
- **Màu**: theme mặc định của thienui tên là `claude` ("Claude Clay"), và sakubun dùng nó. Cam đất trên nền kem ấm chính là nhận diện của Claude.ai. Lab2 dùng cam FPT thì có lý do (nhận diện), nhưng sakubun và thienui thì **"gu thường xuyên" của bạn đang là gu của sản phẩm bạn dùng nhiều nhất**. Đó là sao chép, chưa phải gu.

> **Chân lý cần thấm:** *Hiểu một phong cách là hiểu vì sao các phần của nó đi cùng nhau.* Lấy một chi tiết ra khỏi hệ của nó thì nó mất nghĩa.

### W5 — Lấy giải thích để bù cho thiết kế chưa tự nói được
- Lab2 có luật T1 "không có câu giải thích", rất tốt. Nhưng sakubun và thienui lại đi ngược:
  - banner Phân tích dài khoảng 30 chữ có gạch ngang giải thích
  - section "OpenJLPT theo cấp" có dòng phụ hướng dẫn "Bấm một ô để xem…"
  - thienui luật `every-control-explains-itself`: **mọi** nút icon, badge, số liệu đều phải có tooltip
- Tooltip là **nạng chống**. Nếu nhiều thứ cần giải thích đến mức phải thành luật, câu hỏi đúng là *vì sao chúng không tự hiển nhiên* (dùng icon không nhãn, viết tắt, số không có đơn vị).
- sakubun luật nút: *"laptop chỉ hiện icon, rê chuột thì giãn ra hiện chữ"*. Đây là hy sinh **recognition** để đổi lấy **gọn mắt** (vi phạm Nielsen #6: *recognition rather than recall*), rồi lại phải dùng tooltip để vá.

### W6 — Đúng ngữ pháp component, sai ngữ nghĩa
- **lab2 GV-102 .D2 (bản cam):** dùng **switch** để điểm danh có mặt/vắng cho 35 em. Switch theo quy ước nghĩa là *bật/tắt một cài đặt, có hiệu lực ngay*, không phải "đánh dấu có mặt". Hơn nữa, 32 switch xanh lá trên màn tạo ra **mảng màu lớn nhất màn hình**, cho một thứ *không phải hành động chính* → mâu thuẫn trực tiếp với kỷ luật "cam chỉ cho hành động" của chính bạn. Bản teal dùng nút ✓/✕ chỉ cho 3 em chưa quét và gộp 32 em đã quét thành một hàng thì **đúng hơn nhiều**. Lần thứ hai bạn đi lùi.
- **sakubun Hội thoại:** dùng ẩn dụ chat (trái/phải) cho kịch bản **ba người**. Hai nhân vật cùng nằm bên phải, khác nhau chỉ bằng màu nền (xám và xanh nhạt). Mắt phải zíc zắc qua khoảng trống lớn ở giữa. Với việc *luyện đọc kịch bản*, một cột thẳng có tên vai, giống kịch bản sân khấu, sẽ dễ đọc hơn.
- **Chip "Tôi là 店員 / グエン / 田中"** (chọn một trong nhiều) và **chip "Ẩn nghĩa", "Che câu của tôi"** (bật/tắt) có cùng hình dạng, nằm cùng một hàng. Gestalt similarity nói với người dùng rằng chúng cùng loại, nhưng thực ra không phải.

### W7 — Quản trị nhiều hơn thiết kế
- Ba repo có lượng **văn bản về luật** rất lớn: 37 luật thienui, ui-standard sakubun, DESIGN.md 125 dòng, screen-spec cho 61 khung. Trong khi đó số **phương án bố cục được thử** cho mỗi màn là 1–3.
- Nhiều luật được chốt theo cảm giác vi chỉnh, không theo nguyên lý: *"thien chọn 7px… rồi nâng lên 8px sau khi xem trên trang thật"*. Chỉnh 1px bo góc không làm thay đổi trải nghiệm. Thời gian đó nên dành cho việc thử ba bố cục khác hẳn nhau.
- Luật `capability-over-rearrangement` ("không sắp xếp lại màn đã quen") **chặn đúng loại thay đổi chữa được bệnh đơn điệu**.
- Đây là dấu hiệu của **W1 ở cấp quy trình**: bạn thấy an toàn khi có luật. Nhưng thiết kế giỏi cần nhiều phương án bị vứt đi hơn là nhiều luật được giữ lại.

### W8 — Chuyển động: hạ tầng đầy đủ, cảm giác chưa từng được kiểm *(có bằng chứng lỗi)*
- thienui có thang duration, năm easing, **bốn "tính cách" spring × bốn vai trò**: trên giấy thì rất kỹ.
- Nhưng `registry/lib/motion-tokens.ts` (file sinh tự động) có giá trị spring là chuỗi **`"[object Object]"`**. `motion.ts` dùng `...(primitive[...] as unknown as {stiffness, damping, mass})` để spread chuỗi đó, nên lớp ép kiểu `as unknown as` **che mất lỗi**. Hệ quả: spring không nhận được stiffness, damping hay mass nào, motion/react rơi về spring mặc định, và **bốn tính cách chuyển động hiện đang giống hệt nhau**.
- Lỗi này qua được typecheck, lint, test và build. Nó chỉ lộ ra nếu có người **nhìn và cảm** chuyển động. Không ai đã làm vậy.
- Trong sakubun, chuyển động thực tế chủ yếu là `transition-colors` (29 lần) và `animate-spin` (16 lần). Hầu như không có chuyển động mang ý nghĩa: chuyển cảnh, phản hồi thành công, nối giữa hai trạng thái.

> **Chân lý cần thấm:** *Chuyển động phải được cảm bằng mắt, ở tốc độ thật, nhiều lần.* Test chứng minh code chạy, không chứng minh cảm giác đúng.

### W9 — Gu hình thành qua việc duyệt, không qua việc làm
- Bạn kể: tự tay làm Figma một lần, sau đó làm qua AI, rồi duyệt và yêu cầu sửa. Đọc nhật ký AI của lab2 cũng thấy đúng như vậy: 15 mục AI, 4 vòng "thien duyệt từng màn".
- Người chỉ duyệt sẽ phát triển **khả năng nhận ra cái sai** (W1), nhưng rất chậm phát triển **khả năng tưởng tượng ra cái hay**. Lý do là bạn luôn chọn trong những gì AI đưa ra, và AI đưa ra **mức trung bình** của các mẫu nó từng thấy.
- Vì vậy lộ trình sẽ có luật **"tay trước, AI sau"** cho mỗi bài tập (xem `docs/02-roadmap.md`).

---

## 3. Phản biện luật 70-20-10 của thầy, áp vào chính lab2

Đo trên Figma GV-001 .D (bản cam), ước lượng theo diện tích:
- **~85–88% trắng và xám nhạt** (nền, thẻ, viền)
- **~0–3% "màu phụ"**: thực tế không có tầng này. Avatar nền cam nhạt rất nhỏ.
- **~10–12% cam** (thẻ slot đang diễn ra cùng icon tab)

→ Thầy đúng ở chỗ **tầng 20% không tồn tại**. Giao diện chỉ có hai tầng là trung tính và nhấn, nên mắt nhảy thẳng từ "không có gì" sang "cam", không có mặt bằng trung gian.

Nhưng nếu chỉ thêm tầng 20% bằng cách tô màu nền vài thẻ, bạn sẽ **phá kỷ luật "không tô màu để trang trí"** mà không chữa được W2 hay W3. Cách áp dụng đúng:
1. **Tầng 20% nên là một mặt phẳng có ý nghĩa**, ví dụ một vùng header màu ấm nhạt bao lấy *ngữ cảnh hôm nay* (ngày, tiến độ chốt), hoặc nền section khác nhau giữa "việc cần làm" và "thông tin tham khảo". Nó tạo ra **figure–ground** (hình–nền), không phải trang trí.
2. **Sửa W2 trước**: một con số thật to (display 40–48px) làm điểm nhấn, tiêu đề và nội dung cách xa nhau về cỡ, bỏ gờ đáy ở những thẻ không bấm được.
3. Sau đó mới tinh chỉnh tỉ lệ màu.

→ COL-001 giữ ở trạng thái `draft`. Bổ sung ghi chú: *"tầng phụ là mặt phẳng tổ chức nội dung, không phải màu tô thẻ."*

---

## 4. Ảnh chân dung kỹ năng (tự đánh giá của Claude, thang 1–5)

| Trục | Điểm | Ghi chú |
|---|---|---|
| Hệ thống / token / tooling | **5** | Cao hơn nhiều so với mức sinh viên |
| Trạng thái & trợ năng | **4** | Rất kỹ; còn thiếu nhịp chuyển giữa các trạng thái |
| Nghiên cứu & lập luận UX | **3.5** | Retro tốt, có phỏng vấn thật (n=2 sinh viên, ít). Lập luận "vì sao" mạnh |
| Kiến trúc thông tin & ưu tiên | **2.5** | Có hiểu biết lý thuyết, nhưng hai lần đi lùi (W3, W6) |
| Phân cấp thị giác / tỉ lệ / bố cục | **2** | Điểm yếu chính (W1, W2) |
| Typography | **2** | Có thang chữ, chưa dùng chữ làm chất liệu biểu cảm |
| Màu | **3** | Kỷ luật tốt, chưa có tầng phụ, chưa có màu của riêng mình |
| Cá tính / thương hiệu / cảm xúc | **1.5** | Mượn bề mặt (W4) |
| Chuyển động | **1.5** | Hạ tầng có, cảm giác chưa có, có lỗi (W8) |
| Gu / tưởng tượng phương án | **2** | Gu đang hình thành qua việc duyệt (W9) |

---

## 5. Ưu tiên học (dẫn tới lộ trình)

1. **Bố cục và phân cấp ở cấp trang** (M1): chữa W1, W2, W3. Đây là thứ thầy đang nhìn thấy.
2. **Typography như chất liệu** (M2): tăng tương phản cỡ chữ và độ đậm.
3. **Tâm lý hành vi và kiến trúc thông tin** (M5, M6): chữa W3, W5, W6. Học bắt đầu thiết kế từ hành động.
4. **Animation** (M9): chữa W8. Học cảm chuyển động bằng mắt.
5. **Cá tính và hệ thống** (M10): chữa W4. Tìm gu riêng thay vì mượn.

---

## 6. Bài tập đầu tiên (giao cho bạn)

**BT-M0-01 · "Ba bố cục, không đổi màu"** *(khoảng 2 giờ, làm bằng tay trên Figma, KHÔNG dùng AI)*
Lấy màn GV-001 Tổng quan (lab2), giữ nguyên dữ liệu và bảng màu cam hiện có. Vẽ **3 bố cục khác hẳn nhau**:
- A: một con số hoặc một hành động chiếm ≥ 30% màn đầu tiên
- B: dùng một mặt nền màu (tầng 20%) để chia "việc của hôm nay" và "thông tin tham khảo"
- C: tự do, nhưng phải khác A và B về cấu trúc, không chỉ về chi tiết

Điều kiện: không thêm màu mới, không thêm font mới. Mỗi phương án ghi **một câu**: điểm nhấn là gì, và vì sao người dùng cần thấy nó đầu tiên lúc 7:05 sáng.
Mang cả ba vào buổi sau, ta sẽ critique theo `templates/review-checklist.md`.

---

## 7. Luật rút ra (draft, chờ bạn duyệt)

- `VIS-001` (heuristic, draft) — Mỗi màn có **đúng một điểm nhấn chính**, lớn hơn rõ rệt phần còn lại (gợi ý: ≥ 2 bậc trên thang chữ, hoặc là mảng màu nhấn duy nhất).
- `VIS-002` (heuristic, draft) — **Nhất quán ≠ đồng phục**: thang bo, chữ, icon và nổi phải có ít nhất 3 bậc **cách xa nhau**. Cấm gộp mọi token về một giá trị.
- `VIS-003` (heuristic, draft) — **Chỉ thứ bấm được mới nổi**. Thẻ thông tin không có gờ hay bóng.
- `UX-001` (heuristic, draft) — **Màn hình bắt đầu từ hành động**: hành động chính nằm trong viewport đầu tiên. Số liệu chỉ được lên đầu nếu nó dẫn tới một quyết định.
- `CMP-001` (standard, draft) — Dùng control đúng ngữ nghĩa nền tảng: switch = cài đặt có hiệu lực ngay; checkbox hoặc nút = đánh dấu mục; radio hoặc segmented = chọn một; toggle chip = bật/tắt. Hai loại khác nghĩa thì không được trông giống nhau.
- `PRC-001` (heuristic, draft) — **Mỗi màn quan trọng thử ≥ 3 bố cục khác cấu trúc** trước khi tinh chỉnh chi tiết.
- `PRC-002` (heuristic, draft) — **Chuyển động phải được xem ở tốc độ thật** (và ở 0.25×) trước khi coi là xong. Test không thay được mắt.

## Ghi chú / câu hỏi mở cho bạn
1. Bạn **không đồng ý** điểm nào ở trên? Hãy phản biện. Đó là bước 3 của Lesson Loop, và mình cũng có thể sai.
2. Thầy nhận xét "đơn điệu" trên **bản cam hiện tại** hay trên bản teal? (Ảnh trong repo là bản teal ngày 22/10.)
3. Lỗi spring `[object Object]` trong thienui: bạn muốn tự sửa, coi như bài tập mở màn cho M9, hay để mình mở PR?
