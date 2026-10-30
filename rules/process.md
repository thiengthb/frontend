# Luật quy trình (PRC)

---
### PRC-001 — Ba bố cục trước khi tinh chỉnh
- **Loại:** heuristic
- **Trạng thái:** draft
- **Luật:** Mỗi màn quan trọng phải thử ≥ 3 bố cục khác nhau **về cấu trúc** (không chỉ khác màu hay chi tiết) trước khi tinh chỉnh pixel.
- **Lý do:** Phương án đầu tiên thường là mặc định (của mình hoặc của AI). Chỉnh 1px bo góc không thay đổi trải nghiệm; đổi cấu trúc thì có.
- **Bài học gốc:** M0-01 (W1, W7)

---
### PRC-002 — Chuyển động được duyệt bằng mắt
- **Loại:** heuristic
- **Trạng thái:** draft
- **Luật:** Mọi chuyển động được xem ở tốc độ thật và ở 0.25× trước khi coi là xong. Typecheck hay test không thay được bước này.
- **Lý do:** Lỗi spring `[object Object]` trong thienui đã qua được mọi cổng máy móc, và bốn "tính cách" chuyển động hoá ra giống hệt nhau.
- **Bài học gốc:** M0-01 (W8) → M9

---
### PRC-003 — Tay trước, AI sau (khi học)
- **Loại:** preference (quy ước học tập)
- **Trạng thái:** draft
- **Luật:** Trong lộ trình học, mỗi bài tập phác bằng tay trước, rồi mới nhờ AI tạo biến thể, rồi so sánh và ghi lại khác biệt.
- **Lý do:** Chỉ duyệt phương án của AI thì luyện được mắt bắt lỗi, không luyện được khả năng tưởng tượng phương án (W9).
- **Bài học gốc:** M0-01 (W9)
