# SESSIONS — Nhật ký phiên

## 2026-10-30 · Phiên khởi tạo
- Người dùng nêu mục tiêu: học UI/UX có chiều sâu để làm việc với AI như một art director.
- Thầy góp ý: thiết kế đơn điệu, nên áp dụng 70-20-10. Đã ghi thành COL-001 (draft) kèm phản biện.
- Dựng khung repo: CLAUDE.md, docs (perspective, glossary, roadmap), templates, log.
- Tiếp theo: M0 (chẩn đoán thiết kế hiện tại).

## 2026-10-30 · Phiên 2 · Chẩn đoán & lộ trình v2
- Đọc lab2 (repo cùng Figma hiện tại qua MCP), sakubun, thienui. Viết `lessons/M0-01-baseline.md` (W1–W9, chấm 10 trục).
- Phát hiện lỗi spring `[object Object]` trong thienui motion-tokens.
- Viết lại roadmap v2 (thêm M5–M7, M9 Animation; nhịp 4 giờ/tuần), thêm `docs/03-reading-list.md`.
- 8 luật draft mới. Giao BT-M0-01. Đẩy lên repo `thiengthb/frontend`.

## 2026-10-30 · Phiên 3 · Chuyển sang crash course
- Người dùng thú thực điểm mạnh chủ yếu do AI làm; đồng ý W1–W9; thầy chê bản cam. Hiệu chỉnh M0-01 (§8, thêm W10).
- Chốt crash course 3 ngày + Critique Loop (subagent làm, người dùng phê bình, Claude chấm cả hai).
- Thêm `docs/05-crash-course.md` (13 khối, mindmap), `templates/critique.md`, `log/critique-scores.md`, danh sách video đã kiểm link.
- Giải thích spring bằng demo tương tác.
- (Phiên 3, tiếp) Duyệt PRC-004; thêm PRC-005 (Figma chỉ đọc) và PRC-006 (mỗi Mốc một chat); thêm bước quiz nhớ lại đầu khối; viết sẵn `docs/briefs/CC-01.md`. Kết thúc chat, Mốc 1 mở ở chat mới.

## 2026-10-30/31 · Phiên 4 · Khối CC-01
- Subagent làm 3 bố cục GV-001 (`demos/CC-01/`, publish artifact). Giảng phân cấp, demo squint test; video thay bằng tóm tắt 9 ý Schoger (D-017).
- Người dùng phê bình 3/10 (mắt đúng, thiếu thuật ngữ và hướng sửa); subagent 7/10. Người dùng tìm ra C trùng tab Lịch, Claude bỏ sót.
- Adopted VIS-004, VIS-005, UX-002 (D-015). D-016: không làm lại CC-01, phê bình lại phương án B ở đầu CC-02.
- Viết `docs/briefs/CC-02.md` (thang chữ mới + GV-103). Tiếp theo: CC-02 ở chat mới.

## 2026-10-31 · Phiên 5 · Nửa CC-02 → thiết kế lại crash course
- Quiz CC-01 1.5/3; 0b bỏ qua (Claude làm mẫu). Subagent làm thang chữ + GV-103 (`demos/CC-02/`), phê bình tham chiếu đã khoá trong lesson (6/10).
- Giảng typography (modular scale, đậm/nghiêng/gạch chân, tabular, dấu chồng) kèm demo inline.
- Người dùng yêu cầu đổi sang học trực quan, chỉ đọc: viết `docs/05-crash-course.md` v2 (V-01..V-15), PRC-007, D-018, D-019, `docs/06-ai-prompt-dictionary.md`, brief V-01.

## 2026-10-31 · Phiên 6 · V-01
- Dựng và publish artifact V-01 Phân cấp (`demos/V-01/hierarchy.html`): 7 đòn bẩy bật tắt, squint test, thanh tỉ lệ bước, 5 cặp tệ/tốt, công thức mặc định, 3 phương án CC-01 có chú thích, 6 câu lệnh AI, tự kiểm tra.
- Glossary đánh ✅ 5 thuật ngữ, thêm de-emphasize, consistency ≠ uniformity, concentric radius. Từ điển thêm dòng "cam ở khắp nơi".
- Viết `docs/briefs/V-02.md`. Tiếp theo: V-02 Typography.
- (tiếp) Người dùng đọc xong V-01. Dựng và publish V-02 Typography (`demos/V-02/typography.html`): thang chữ sống (gốc + tỉ lệ, so thang cũ), độ đậm có vai, ma trận nhấn mạnh, tabular, line-height/measure tiếng Việt, 5 cặp, bài AI GV-103 có chú thích + bản sửa.
- Glossary ✅ thêm 8, từ điển thêm dòng "số to mà chẳng để làm gì". Viết `docs/briefs/V-03.md`. Tiếp theo: V-03 Màu ở chat mới.

## 2026-10-31 · Phiên 7 · V-03
- Chat mới. Dựng và publish V-03 Màu (`demos/V-03/color.html`): OKLCH vs HSL (xem bằng xám, thang theo hue), neutral thuần/ấm/lạnh, máy đo 70-20-10 tự đo diện tích trên GV-001 (2 thanh trượt, 4 phương án, đếm số chỗ dùng cam), tầng 20% đúng/sai, semantic + mô phỏng mù màu, 5 cặp, công cụ contrast WCAG, lab2 cam → B → sửa có đo.
- Phát hiện: warning lab2 `#A15C00` gần cam nhấn (hue 62° vs 45°, cùng L ≈ 0.55), phải kèm icon/chữ.
- Glossary ✅ 8 + thêm OKLCH, chroma, accent dilution, color-not-alone. Từ điển thêm mục V-03. Viết `docs/briefs/V-04.md`.
- (tiếp) Dựng và publish V-04 Khoảng cách (`demos/V-04/spacing.html`): thang 4/8 vs số tuỳ hứng, proximity 2 thanh trượt (mốc lab2 12/16 → "đều đều"), ba tầng 8/24/40, nhịp, lưới 4 cột bật tắt lệch/theo lưới, mật độ 48/60/76, 5 cặp, GV-102 trước/sau. Mọi khoảng cách là phần tử thật nên có lớp phủ đo như DevTools.
- Glossary ✅ grid, spacing scale, rhythm, proximity, alignment, density; thêm gutter/margin, whitespace micro/macro, padding vs gap. Từ điển thêm V-04. Viết `docs/briefs/V-05.md`.
- (tiếp) Dựng và publish V-05 Chiều sâu (`demos/V-05/depth.html`): năm cách tách khối, elevation một lớp vs hai lớp, máy đếm nổi/bấm được trên GV-001 (bản cam: 11 nổi, 7 nói dối), bo đồng tâm có thanh trượt, thang bo sakubun vs 3 bậc, gờ dày đúng/sai (W4), dark mode surface tint, 5 cặp, GV-001 trước/sau. Hết Ngày 1.
- Glossary ✅ affordance/signifier; thêm elevation, shadow hai lớp, ledge, surface tint. Từ điển thêm V-05. Viết `docs/briefs/V-06.md`.
- (tiếp) Người dùng góp ý cách viết khó hiểu, thiếu chuyển tiếp. Tra nguồn (ISO 24495, CPSC, known-new contract, curse of knowledge, Briswell) → viết `docs/07-communication-style.md` (10 quy tắc + ví dụ sửa câu của chính Claude), D-020, CLAUDE.md §2 và §4 trỏ tới, brief V-06 cập nhật.
