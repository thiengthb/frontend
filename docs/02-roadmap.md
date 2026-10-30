# 02 — Lộ trình học (Roadmap) · v2 · *deep track*

> **Từ 2026-10-30:** học trước bằng **crash course 3 ngày** (`docs/05-crash-course.md`), làm lại lab2, rồi mới quay lại lộ trình này như deep track 4 giờ/tuần (D-008).

> **v2 · 2026-10-30.** Viết lại sau chẩn đoán `lessons/M0-01-baseline.md`.
> - Thêm: tâm lý học hành vi (M5), nghiên cứu người dùng (M6), quy chuẩn & tỉ lệ (M7), **chuyên mục Animation riêng (M9)**.
> - Sắp lại thứ tự theo điểm yếu W1–W9.
> - Nhịp đã chỉnh cho **4 giờ/tuần**.

## Nhịp một tuần (4 giờ)
| Khối | Thời lượng | Nội dung |
|---|---|---|
| Buổi học với Claude | 90' | Bước 1–3 của Lesson Loop: khái niệm, ví dụ (demo), phản biện |
| Bài tập | 120' | Bước 4. **Luật "tay trước, AI sau"**: phác bằng tay (Figma hoặc code) trước, rồi mới nhờ AI làm biến thể, rồi so sánh |
| Nhật ký & đọc | 30' | Design diary (2 giao diện/tuần) cùng 1 bài đọc ngắn trong `docs/03-reading-list.md` |

Review (bước 5) và chắt luật (bước 6) diễn ra đầu buổi học tuần sau, khoảng 20 phút.
**1 bài ≈ 1 tuần.** Toàn bộ lộ trình khoảng 50 bài, tức **khoảng 12 tháng**. Đây là con số thật, không làm đẹp.

**Mốc kiểm tra:** cuối M4 (khoảng tháng 4) bạn làm lại lab2 GV-001 và GV-102 và mang cho thầy xem. Nếu thầy không còn nói "đơn điệu", thì giai đoạn thị giác đã qua.

```
Giai đoạn A · NHÌN (thị giác)        M1 Bố cục & phân cấp → M2 Chữ → M3 Màu → M4 Lưới & nhịp
Giai đoạn B · HIỂU NGƯỜI (UX sâu)    M5 Tâm lý hành vi → M6 Nghiên cứu người dùng → M7 Quy chuẩn & tỉ lệ
Giai đoạn C · LÀM VẬT (tương tác)    M8 Component & pattern → M9 ANIMATION
Giai đoạn D · THÀNH HỆ               M10 Cá tính & design system → M11 Art-direct AI → M12 Capstone
```

---

## M0 — Chẩn đoán (2 bài) ✅ bài 1 xong
- M0-01 Baseline: đọc 3 project, chấm 10 trục → `lessons/M0-01-baseline.md`
- M0-02 Moodboard gu: 10 giao diện thích, 5 ghét. **Mỗi cái gọi tên ≥ 2 thuật ngữ**. Mục tiêu là tìm gu *của bạn*, tách khỏi gu Claude.ai và shadcn (W4)

## Giai đoạn A · NHÌN

### M1 — Bố cục & phân cấp ở cấp trang (6 bài) ← *chữa W1, W2, W3*
- M1-01 Visual hierarchy: 6 đòn bẩy (cỡ, đậm, màu, vị trí, khoảng trắng, hình dạng); bài test nheo mắt (squint test)
- M1-02 Tương phản & tỉ lệ: vì sao bước 14→15→16 vô nghĩa còn 14→20→32 có nghĩa; **nhất quán ≠ đồng phục**
- M1-03 Gestalt nâng cao: figure–ground, common region, similarity bị dùng sai (W6)
- M1-04 Điểm nhấn & Von Restorff: một focal point mỗi màn; "mọi thứ nổi = không gì nổi"
- M1-05 Bố cục khởi đầu từ hành động: thứ tự ưu tiên nội dung, viewport đầu tiên, phá phản xạ lưới KPI
- M1-06 Nhịp điệu & khoảng trắng: khoảng trong nhóm < khoảng giữa nhóm < khoảng giữa section; lặp có biến tấu
- **Bài tập lớn:** làm lại GV-001 lab2 bằng 3 bố cục (BT-M0-01 nối tiếp)
- **Đầu ra:** `rules/visual.md`, `rules/layout.md` (phần cấp trang)

### M2 — Typography như chất liệu (5 bài)
- M2-01 Giải phẫu chữ; "giọng" của font; font hỗ trợ tiếng Việt tốt (dấu chồng, độ cao dấu)
- M2-02 Type scale: tỉ lệ modular (1.2 / 1.25 / 1.333 / 1.5), chọn tỉ lệ theo mật độ sản phẩm, `clamp()` co giãn
- M2-03 Độ đậm, nghiêng, gạch chân, in hoa, tracking: **ma trận khi nào dùng / cấm dùng**
- M2-04 Đọc dễ: measure 45–75ch, line-height theo cỡ chữ, chữ số tabular cho dữ liệu, chữ CJK cạnh chữ Latin (sakubun)
- M2-05 Chữ làm điểm nhấn: display type, số lớn, font pairing tạo cá tính
- **Đầu ra:** `rules/typography.md` cùng token thang chữ

### M3 — Màu (5 bài)
- M3-01 OKLCH: trục L-C-H, vì sao dải màu tạo bằng OKLCH đều mắt hơn HSL
- M3-02 Hệ màu: neutral có pha sắc, primary, semantic, thang 50–950
- M3-03 **60-30-10 / 70-20-10**: tính theo diện tích; tầng phụ là *mặt phẳng tổ chức*, không phải màu tô (bài thầy giao)
- M3-04 WCAG 2.2, APCA (thế hệ mới, ⚠ chưa thành chuẩn), mù màu, dark mode đúng cách
- M3-05 Màu & cảm xúc, văn hoá (Việt Nam / Nhật / phương Tây). Tìm màu *của riêng bạn*
- **Đầu ra:** `rules/color.md` cùng token màu

### M4 — Lưới, spacing & responsive (4 bài)
- M4-01 Thang spacing & 4/8pt, khoảng cách theo quan hệ (proximity) chứ không theo thói quen
- M4-02 Lưới cột, container, lưới bất đối xứng, bento, split; bố cục kinh điển (F/Z, hero, sidebar, master–detail)
- M4-03 Responsive & container query; mật độ: landing ≠ app ≠ dashboard
- M4-04 **Mốc kiểm tra:** làm lại 2 màn lab2, so trước/sau, xin thầy nhận xét

## Giai đoạn B · HIỂU NGƯỜI

### M5 — Tâm lý học nhận thức & hành vi người dùng (7 bài) ← *chữa W3, W5*
- M5-01 Hai hệ tư duy (Kahneman System 1/2): người dùng **không đọc**, họ lướt (NN/g eyetracking, F-pattern, banner blindness)
- M5-02 Trí nhớ & tải nhận thức: Miller (đúng nghĩa), chunking, Cognitive Load Theory (Sweller), recognition > recall
- M5-03 Các định luật vận động & quyết định: Fitts, Hick–Hyman, Steering law, keystroke-level model; **thời gian phản hồi** 0.1 / 1 / 10 giây (Miller 1968, Nielsen), Doherty threshold
- M5-04 Thiên kiến nhận thức trong UI: anchoring, default effect, loss aversion, framing, peak-end, Zeigarnik, aesthetic-usability, ấn tượng 50ms (Lindgaard 2006)
- M5-05 Mô hình hành vi: Fogg B=MAP, vòng thói quen (Hooked, đọc có phê phán), Self-Determination Theory (tự chủ, năng lực, kết nối). Áp vào sakubun (SRS, streak)
- M5-06 Thuyết phục & đạo đức: Cialdini, nudge (Thaler–Sunstein), **dark patterns** (Brignull). Lằn ranh giữa giúp và thao túng
- M5-07 10 heuristic Nielsen và 7 nguyên tắc Norman (affordance, signifier, mapping, feedback, constraint, conceptual model). Bài tập là heuristic evaluation sakubun
- **Đầu ra:** `rules/ux.md` (UX-xxx), `rules/content.md` (CNT-xxx)

### M6 — Nghiên cứu người dùng (5 bài)
- M6-01 Bản đồ phương pháp: định tính ↔ định lượng, thái độ ↔ hành vi (NN/g "landscape of UX research methods")
- M6-02 Phỏng vấn: The Mom Test, câu hỏi về quá khứ chứ không về tương lai; tránh dẫn dắt (bạn đã rút bài học phỏng vấn giả bằng AI ở lab2)
- M6-03 JTBD, persona dựa trên bằng chứng, journey map, affinity mapping
- M6-04 Usability testing: think-aloud, 5 người (Nielsen–Landauer, và giới hạn của con số 5), task success, SUS
- M6-05 Đo sau phát hành: analytics, A/B test (cạm bẫy thống kê), HEART framework (Google)
- **Đầu ra:** `templates/interview-guide.md`, `templates/usability-test.md`, luật PRC

### M7 — Quy chuẩn & tỉ lệ: sổ tay số liệu (3 bài)
- M7-01 Chuẩn bắt buộc: WCAG 2.2 AA (contrast, target size 24px tối thiểu / 44px khuyến nghị, focus appearance, reflow 320px), ARIA APG
- M7-02 Quy ước nền tảng: Apple HIG, Material 3, Fluent. So **cùng một component** trên ba hệ để hiểu vì sao chúng khác nhau
- M7-03 Tỉ lệ & con số trong thiết kế: modular scale, tỉ lệ vàng (và vì sao nó bị thần thánh hoá), tỉ lệ khung hình, 8pt, measure, density, duration chuyển động. Kèm **phản biện từng con số**
- **Đầu ra:** `docs/04-numbers-cheatsheet.md` (mỗi con số có nguồn và loại: standard / heuristic)

## Giai đoạn C · LÀM VẬT

### M8 — Component & UI pattern (6 bài) ← *chữa W6*
Mỗi component học theo 5 câu hỏi: **giải quyết vấn đề gì → giải phẫu → biến thể → trạng thái → khi nào KHÔNG dùng**.
- M8-01 Nút: phân cấp hành động, nhãn động từ, icon-only khi nào được phép (phản biện luật sakubun)
- M8-02 Chọn & bật/tắt: checkbox, radio, switch, segmented, toggle chip. **Ngữ nghĩa trước hình dạng** (W6)
- M8-03 Form & input: label, validation inline, thông báo lỗi
- M8-04 Điều hướng & IA: sidebar, tabs, bottom nav, breadcrumb, command palette
- M8-05 Hiển thị dữ liệu: card vs list vs table; dashboard *dẫn tới hành động*
- M8-06 Overlay & phản hồi: modal, sheet, popover, tooltip (khi nào là nạng chống, W5), toast, empty/loading/error
- **Tham chiếu:** GOV.UK Design System (rất giỏi về lý do), Material 3, Apple HIG, Radix/Base UI, Mobbin
- **Đầu ra:** `rules/components.md`

### M9 — ANIMATION & MOTION · chuyên mục riêng (9 bài) ← *chữa W8*
> Mục tiêu: hiểu chuyển động như **ngôn ngữ** (nó nói gì với người dùng), không như trang trí; và **cảm** được nó bằng mắt.

| Bài | Nội dung |
|---|---|
| M9-01 | **Vì sao UI chuyển động**: 5 mục đích (định hướng không gian, nối nhân–quả/phản hồi, hướng sự chú ý, thể hiện trạng thái hệ thống, cá tính). Khi nào KHÔNG nên animate (tần suất cao, luật đã có trong thienui) |
| M9-02 | **12 nguyên lý hoạt hình Disney** (Thomas & Johnston), lọc ra các nguyên lý áp được cho UI: timing, easing (slow in/out), anticipation, follow-through, staging, squash & stretch, arc |
| M9-03 | **Timing**: thang thời lượng (100–150ms phản hồi nhỏ, 200–300ms chuyển trạng thái, 300–500ms chuyển cảnh lớn); vì sao chuyển động dài hơn khi quãng đường xa hơn; vào nhanh hơn ra hay ngược lại |
| M9-04 | **Easing**: cubic-bezier đọc thế nào, ease-out cho vào, ease-in cho ra; vì sao `linear` trông máy móc. Bài tập là tự vẽ đường cong trên cubic-bezier.com |
| M9-05 | **Spring physics**: stiffness, damping, mass; vì sao spring tự nhiên hơn tween; bounce khi nào thì sang, khi nào thì rẻ. **Bài tập là sửa lỗi `[object Object]` trong thienui** rồi so 4 tính cách bằng mắt |
| M9-06 | **Biên đạo (choreography)**: stagger, thứ tự xuất hiện, shared element / layout animation, chuyển cảnh giữa trang (View Transitions API) |
| M9-07 | **Micro-interaction** (Dan Saffer: trigger → rules → feedback → loops): nút nhấn, toggle, thành công, lỗi (shake), kéo thả, gesture và quán tính |
| M9-08 | **Hiệu năng & trợ năng**: chỉ animate `transform`/`opacity`, compositor, 60/120fps, `will-change`; `prefers-reduced-motion` (chính sách "không bao giờ chết" của thienui là đúng hướng); tiền đình (vestibular) |
| M9-09 | **Công cụ & thực hành**: CSS transitions/keyframes, Motion (framer), Figma Smart Animate; quy trình **xem ở 1× và 0.25×**, quay màn hình so sánh từng khung. Dựng `demos/motion-lab/` |

- **Tham chiếu:** Material motion, Apple HIG Motion, *UX in Motion* (Issara Willenskomer), Val Head *Designing Interface Animation*, animations.dev (Emil Kowalski), Rauno Freiberg *Invisible Details of Interaction Design*, Josh Comeau (spring)
- **Đầu ra:** `rules/interaction.md` (INT-xxx), token motion **đã được cảm**, `demos/motion-lab/`

## Giai đoạn D · THÀNH HỆ

### M10 — Cá tính & design system (3 bài) ← *chữa W4*
- M10-01 Cá tính thương hiệu: tính từ kèm phản đề, rồi dịch thành token (chữ, màu, bo, chuyển động, giọng văn)
- M10-02 Rà lại thienui bằng con mắt mới: luật nào giữ, luật nào là "đồng phục" (W2, W7), thêm luật **cấp trang**
- M10-03 Kiểm thử thẩm mỹ: những thứ máy không đo được thì đo bằng người (preference test, 5-second test)
- **Đầu ra:** `rules/tokens.md`, đề xuất PR cho thienui

### M11 — Art-direct AI (3 bài)
- M11-01 Design brief tốt (`templates/design-brief.md`); dịch cảm giác ra thuật ngữ
- M11-02 Nhận diện "AI slop" (mặc định của AI và shadcn: lưới KPI, gradient, card-everything) và cách ép ra phương án khác
- M11-03 Quy trình: brief → 3 phương án bố cục → chọn → chi tiết → review checklist → motion pass
- **Đầu ra:** `rules/process.md`

### M12 — Capstone (4 bài)
- Một sản phẩm thật (đề xuất: làm lại **một luồng của sakubun**, vì bạn là người dùng thật và có dữ liệu thật): nghiên cứu → IA → 3 bố cục → UI → motion → usability test với 3–5 người → sửa → case study
- Rà toàn bộ `rules/`, chuyển những luật đã kiểm chứng sang `adopted`

---

## Thói quen song song
- **Design diary** (`log/diary/YYYY-MM.md`): mỗi tuần 2 giao diện, mỗi cái có 1 điều hay và 1 điều dở, gọi bằng thuật ngữ.
- **Motion snack**: mỗi tuần quay một chuyển động hay ở app nào đó (5 giây), xem ở 0.25× và mô tả timing/easing. Nhờ vậy bạn luyện mắt cho M9 từ sớm.
- **Clone có phân tích**: mỗi tháng dựng lại một section của sản phẩm bạn ngưỡng mộ, đo bằng DevTools.
