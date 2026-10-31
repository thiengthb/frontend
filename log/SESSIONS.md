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
- (chat mới) Dựng và publish V-06 Bố cục mobile (`demos/V-06/layouts.html`) theo cách viết D-020: năm pattern (overview, list, detail, form, master–detail) khung xương xám, vùng ngón cái có lớp phủ ba vùng và nút gạt top/đáy + tay trái/phải, F-pattern (triệu chứng, NN/g) có/không điểm bám, Z-pattern (kinh nghiệm), viewport đầu tiên với hai thanh trượt chiều cao + cỡ chữ (bản cam rơi dưới fold ở 600dp/125%), mỗi tab một câu hỏi (UX-002, CC-01 phương án C), 5 cặp, 4 màn lab2 xếp theo pattern.
- Glossary ✅ F/Z-pattern, above the fold; thêm list/detail, overview, master–detail, thumb zone, top/bottom bar, multi-step form. Từ điển thêm V-06. Viết `docs/briefs/V-07.md`.
- (tiếp) Dựng và publish V-07 Nút & điều khiển (`demos/V-07/controls.html`): phân cấp nút có nút gạt "nheo mắt" (làm mờ), nhãn nút OK / Xác nhận / Chốt điểm danh trên hộp thoại, năm cách chọn bấm được thật (checkbox, radio, switch có thông báo đã lưu, segmented, filter chip lọc danh sách), máy đếm GV-102 (bản cam 33 lời mời mạnh, 35 hàng; bản tách 1 và 4), chip sakubun cùng hình và khác hình, icon quy ước và icon tự đặt nghĩa, 5 cặp, lab2 GV-102 và GV-001 trước/sau.
- Glossary ✅ phân cấp nút, Jakob's law; thêm destructive, checkbox/radio/switch, segmented, chip, icon button, nhãn động từ. Từ điển thêm V-07. Viết `docs/briefs/V-08.md`.
- (chat mới, 2026-11-01) Dựng và publish V-08 Điều hướng (`demos/V-08/navigation.html`): ba câu hỏi định hướng có nút gạt tiêu đề / tab đang chọn / ‹; máy đo back stack bấm được thật (4 cột ngăn xếp, chế độ giữ / xoá về gốc, nút quay lại hệ thống, deep link từ thông báo); sơ đồ đi ngang và đi dọc với ‹ sai cha, breadcrumb; thanh trượt 2–6 tab (Material: 3–5, đã kiểm developer.android.com); tab trên và tab dưới; 5 cặp; cây lab2 với 3 chỗ IA mập mờ.
- Glossary ✅ IA; thêm navigation bar, top tabs, back stack, up/back, hierarchy, breadcrumb, navigation drawer, deep link. Từ điển thêm V-08. Viết `docs/briefs/V-09.md`.
- (tiếp, 2026-11-01) Dựng và publish V-09 Trạng thái (`demos/V-09/states.html`), đọc spec thật của lab2 (screen-spec, user-flow, ảnh GV-001 .E và .X): sáu khuôn mặt GV-001 có nhận xét (khen .D1, .E giữ Cần chú ý, .E2; chê .X thay cả màn); spinner và skeleton tải lại song song; máy đo thời gian chờ thang log 0,1/1/10 giây (NN/g) với chế độ im lặng đếm số lần bấm trùng; empty state ba kiểu; lỗi ba cách viết; mất mạng thay hết và giữ dữ liệu; Duyệt yêu cầu ba cách báo có đếm chạm và Hoàn tác; 5 cặp; luồng chốt khi mất mạng có hàng chờ tự gửi.
- Glossary ✅ state, spinner/skeleton, empty/error state, offline, toast/snackbar, undo, optimistic UI, mốc thời gian phản hồi. Từ điển thêm V-09. Viết `docs/briefs/V-10.md`.
- (tiếp, 2026-11-01) Dựng và publish V-10 Định luật UX (`demos/V-10/laws.html`), kiểm nguồn Miller 1956 / Cowan 2001, Kahneman 1993, Kurosu & Kashimura 1995: đồng hồ bấm Fitts thật (nhỏ xa và to gần, 5 lần, tính độ khó từ kích thước thật), Hick với menu 2–16 lớp có chế độ "lớp hôm nay lên đầu", chunking mã 8 số và bác "menu tối đa 7 mục", biểu đồ peak-end một buổi điểm danh có hai nút sửa, aesthetic-usability bản thô và bản chăm chút, 5 cặp, nhãn định luật trên GV-001 và GV-102. Hết Ngày 2.
- Glossary ✅ Fitts, Hick, Miller/chunking, peak-end, aesthetic-usability; thêm serial position. Từ điển thêm V-10. Viết `docs/briefs/V-11.md`.
- (tiếp, 2026-11-01) Chat mới. Dựng và publish V-11 Trợ năng (`demos/V-11/a11y.html`), tính lại contrast lab2 bằng công thức WCAG (khớp DESIGN.md; cam FPT gốc 2,97:1): ba tầng chuẩn/quy ước/heuristic, máy đo contrast 8 cặp có sẵn, khu bấm thử vùng chạm 24/32/44/48 với ngón tay giả, lọc mù lục/mù đỏ/xám (gần đúng), vòng focus có nút Tab giả, giảm chuyển động theo cài đặt máy, 5 cặp, bảng mặc định, chú thích DESIGN.md lab2 và câu trả lời mẫu cho thầy.
- Glossary ✅ a11y, WCAG, relative luminance, target size, dp, focus ring, screen reader, reduced motion. Từ điển thêm V-11. Viết `docs/briefs/V-12.md`.
