# PROGRESS — Nguồn sự thật về tiến độ

> Cập nhật cuối mỗi phiên. Phiên Claude mới đọc file này đầu tiên.

## Trạng thái hiện tại
- **Ngày cập nhật:** 2026-10-31
- **Chế độ:** **Crash course 3 ngày + Critique Loop** (`docs/05-crash-course.md`). Lộ trình dài là deep track, làm sau lab2
- **M0-01:** xong
- **Crash course:** **CC-01 xong** (`lessons/CC-01-hierarchy.md`; subagent 7/10, người dùng 3/10). Khối tiếp theo là **CC-02** (typography)
- **Luật:** adopted: PRC-004, PRC-006, **VIS-004, VIS-005, UX-002**. Draft: VIS-001..003, UX-001, CMP-001, COL-001, PRC-001, 002, 005. Deprecated: PRC-003
- Artifact CC-01: "GV-001 ba bố cục" (bài subagent, publish từ `demos/CC-01/`)

## Bước tiếp theo
**Chat mới = khối CC-02.** Trình tự:
1. Gắn và clone `thiengthb/frontend`, đọc PROGRESS và DECISIONS, tóm tắt 3 dòng.
2. **Giao ngay `docs/briefs/CC-02.md` cho subagent chạy nền.**
3. **Quiz nhớ lại** 3 câu ở cuối `lessons/CC-01-hierarchy.md`.
4. **5 phút phê bình lại phương án B của CC-01** (D-016): mỗi ý phải có thuật ngữ + mức + hướng sửa. Ghi dòng "CC-01b" vào `critique-scores.md`. Người dùng có thể bác bước này.
5. Giảng CC-02 (thang tỉ lệ, đậm/nghiêng/gạch chân khi nào, chữ số tabular, tiếng Việt dấu chồng và line-height). Nối từ CC-01: thang lab2 có bậc ×1.06–1.07.
6. Video Elliot Jay Stocks, Config 2025 *Typography is the foundation of any design system* — nếu người dùng thiếu thời gian thì Claude tóm tắt thay (D-017). Kiểm tra link trước khi đưa.
7. Dự đoán 2 phút (bỏ được nếu gấp) → publish bài subagent thành artifact → người dùng phê bình → Claude viết phê bình tham chiếu **trước khi đọc**, rồi chấm cả hai.
8. Kết thúc khối theo PRC-006: lesson `lessons/CC-02-typography.md` (tóm tắt + quiz), điểm, **viết `docs/briefs/CC-03.md`**, PROGRESS, push, đưa câu mở chat CC-03.

## Câu hỏi còn mở
- Lỗi spring `[object Object]` trong thienui: sẽ làm ở CC-11.
- Quy tắc "khối < 4/10 thì làm lại" mâu thuẫn với mục tiêu "khối 1 khoảng 3–4/10" trong `docs/05-crash-course.md`. Tạm xử lý bằng D-016; nên sửa câu chữ trong doc khi người dùng đồng ý.

## Bối cảnh người dùng
- Thiết kế chủ yếu qua AI; tự nhận phần lớn artefact (WCAG, vùng chạm, focus ring) là AI đề xuất, chưa hiểu nền tảng
- Stack: React, Vite, Next.js. Học dồn 2–3 ngày, sau đó 4 giờ/tuần
- Thời gian eo hẹp: ở CC-01 bỏ video, nhờ tóm tắt và làm bài luôn
- Mục tiêu gần: làm lại lab2 (thầy chê bản cam là đơn điệu)
