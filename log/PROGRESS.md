# PROGRESS — Nguồn sự thật về tiến độ

> Cập nhật cuối mỗi phiên. Phiên Claude mới đọc file này đầu tiên.

## Trạng thái hiện tại
- **Ngày cập nhật:** 2026-10-31
- **Chế độ:** **Crash course TRỰC QUAN v2** (`docs/05-crash-course.md`, D-018, PRC-007): mỗi khối V-xx là một artifact tương tác Claude dựng sẵn; người dùng chỉ đọc và nghịch. **Không bài tập, không chấm, không quiz đầu khối.**
- **Đã học theo cách cũ (v1):** CC-01 phân cấp (xong), nửa đầu CC-02 typography (bài giảng + demo inline). Tài liệu tái dùng cho V-01, V-02.
- **Đã xong (v2):** **V-01 Phân cấp & điểm nhấn** (2026-10-31): `demos/V-01/hierarchy.html`, artifact "V-01 Phân cấp" (https://claude.ai/artifact/UUdsaDzKfNx3L3FchPDvf6).
- **Khối tiếp theo:** **V-02 Typography** (brief: `docs/briefs/V-02.md`), làm tiếp trong cùng chat nếu còn ngắn.
- **Luật:** adopted: PRC-004 (tạm ngưng), PRC-006 (sửa D-019), PRC-007, VIS-004, VIS-005, UX-002. Draft: VIS-001..003, UX-001, CMP-001, COL-001, PRC-001, 002, 005. Deprecated: PRC-003
- **Từ điển ra lệnh AI:** `docs/06-ai-prompt-dictionary.md` (đã có V-01 (thêm dòng "cam ở khắp nơi"), V-02)

## Bước tiếp theo
**Dựng V-02** theo `docs/briefs/V-02.md` (load `artifact-design`, tái dùng CSS/khung của `demos/V-01/hierarchy.html`, publish "V-02 Typography") → giải thích ≤ 10 dòng nên bấm gì → viết brief V-03 → hỏi "Sang V-03?".
Cuối mỗi khối: `demos/V-xx/`, từ điển, glossary, brief khối kế, PROGRESS, push.

## Câu hỏi còn mở
- Lỗi spring `[object Object]` trong thienui: minh hoạ ở V-13.
- Bài subagent CC-02 (`demos/CC-02/`) chưa publish cho người dùng; phê bình tham chiếu trong `lessons/CC-02-typography.md` dùng làm chú thích ví dụ ở V-02.

## Bối cảnh người dùng
- Thiết kế chủ yếu qua AI; chưa hiểu nền tảng sau các artefact AI làm hộ (W10)
- Giai đoạn hiện tại: **học vẹt, biết và hiểu sơ** để nhận diện pattern, thuật ngữ, và ra lệnh cho AI; muốn học trực quan, đọc nhanh, liên tục, ít tốn năng lượng
- Stack: React, Vite, Next.js. Học dồn 2–3 ngày, sau đó 4 giờ/tuần
- Mục tiêu gần: làm lại lab2 (thầy chê bản cam là đơn điệu)
