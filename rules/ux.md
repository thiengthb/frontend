# Luật UX (UX)

---
### UX-001 — Màn hình bắt đầu từ hành động
- **Loại:** heuristic
- **Trạng thái:** draft
- **Luật:** Hành động chính của màn phải nằm trong viewport đầu tiên. Số liệu chỉ được lên đầu nếu nó dẫn tới một quyết định ngay lúc đó.
- **Lý do:** Người dùng mở màn để làm một việc (JTBD). Dữ liệu không dẫn tới hành động là *vanity metric*: nó chiếm chỗ của việc chính và tăng tải nhận thức.
- **Ví dụ:** ❌ lab2 GV-001 (cam): "131 sinh viên" đứng trên thẻ "Điểm danh". ❌ sakubun Phân tích: không có nút "Ôn ngay" trong màn đầu. ✅ GV-001 bản teal.
- **Nguồn:** JTBD (Christensen); Nielsen heuristic #8 (aesthetic & minimalist design).
- **Bài học gốc:** M0-01 (W3) → kiểm chứng ở M1-05

---
### UX-002 — Mỗi tab trả lời một câu hỏi khác nhau
- **Loại:** heuristic
- **Trạng thái:** draft
- **Luật:** Trước khi thiết kế một tab, viết câu hỏi nó trả lời (Tổng quan: "Bây giờ tôi cần làm gì, có gì bất thường?"; Lịch: "Hôm nay/tuần này tôi dạy gì, ở đâu?"). Nếu bố cục của tab A trả lời câu hỏi của tab B, nó đang trùng lặp.
- **Lý do:** Hai tab trả lời cùng một câu hỏi thì một tab thừa, và người dùng không biết nên mở tab nào (information architecture).
- **Ví dụ:** ❌ CC-01 phương án C: trục giờ trong ngày là câu trả lời của tab Lịch, đặt vào Tổng quan. **Người dùng phát hiện**, Claude bỏ sót trong phê bình tham chiếu.
- **Nguồn:** nguyên lý IA chung (Rosenfeld & Morville, *Information Architecture*); cách diễn đạt "một câu hỏi" là tổng hợp, không phải trích dẫn.
- **Bài học gốc:** CC-01
