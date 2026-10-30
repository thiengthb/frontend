# PROGRESS — Nguồn sự thật về tiến độ

> Cập nhật cuối mỗi phiên. Phiên Claude mới đọc file này đầu tiên.

## Trạng thái hiện tại
- **Ngày cập nhật:** 2026-10-30
- **Chế độ:** **Crash course 3 ngày + Critique Loop** (`docs/05-crash-course.md`). Lộ trình dài là deep track, làm sau lab2
- **M0-01:** xong, đã hiệu chỉnh theo phản biện của người dùng (§8: W10 ảo giác năng lực; thầy chê bản cam)
- **Crash course:** chưa bắt đầu. Khối tiếp theo là **CC-01** (phân cấp, tương phản, điểm nhấn)
- **Luật:** adopted: PRC-004 (Critique Loop), PRC-006 (mỗi Mốc một chat). Draft: VIS-001..003, UX-001, CMP-001, COL-001, PRC-001, 002, 005. Deprecated: PRC-003

## Bước tiếp theo
**Mở chat mới = Mốc 1 (Ngày 1: CC-01..04).** Trình tự trong chat mới:
1. Gắn và clone `thiengthb/frontend`, đọc PROGRESS và DECISIONS, tóm tắt 3 dòng.
2. **Giao ngay `docs/briefs/CC-01.md` cho subagent chạy nền.**
3. Giảng CC-01 (phân cấp, tương phản, điểm nhấn, squint test; nhất quán ≠ đồng phục), có demo.
4. Người dùng xem video Steve Schoger *Practical Solutions to Common UI Design Problems*.
5. Dự đoán 2 phút → mở bài subagent → người dùng phê bình → Claude chấm cả hai.
6. Trước CC-02: viết sẵn `docs/briefs/CC-02.md` (và lần lượt cho các khối sau) để giao subagent sớm.

## Câu hỏi còn mở
- Lỗi spring `[object Object]` trong thienui: sẽ làm ở CC-11 (người dùng đã biết spring là gì sau phiên này).

## Bối cảnh người dùng
- Thiết kế chủ yếu qua AI; tự nhận phần lớn artefact (WCAG, vùng chạm, focus ring) là AI đề xuất, chưa hiểu nền tảng
- Stack: React, Vite, Next.js. Học dồn 2–3 ngày, sau đó 4 giờ/tuần
- Mục tiêu gần: làm lại lab2 (thầy chê bản cam là đơn điệu)
