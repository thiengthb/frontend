# Luật thị giác (VIS)

---
### VIS-001 — Mỗi màn một điểm nhấn chính
- **Loại:** heuristic
- **Trạng thái:** draft
- **Luật:** Mỗi màn có đúng một điểm nhấn chính, lớn hơn rõ rệt phần còn lại (≥ 2 bậc trên thang chữ, hoặc là mảng màu nhấn duy nhất).
- **Lý do:** Không có điểm nhấn thì mắt không biết bắt đầu từ đâu và màn trông "đơn điệu". Có nhiều điểm nhấn thì chúng triệt tiêu nhau (Von Restorff).
- **Áp dụng khi:** mọi màn có hành động hoặc thông tin ưu tiên.
- **Không áp dụng khi / lưu ý:** màn đọc dài (bài viết) thì điểm nhấn là tiêu đề, và không cần mạnh.
- **Ví dụ:** ❌ lab2 GV-001 (cam): 4 ô KPI bằng nhau cùng thẻ slot, không có gì thắng. ✅ Bản teal: thẻ slot đang diễn ra là khối màu duy nhất, nằm trên cùng.
- **Nguồn:** Von Restorff (1933); *Refactoring UI*, chương Hierarchy.
- **Bài học gốc:** M0-01 (W2, W3) → kiểm chứng ở M1-04

---
### VIS-002 — Nhất quán ≠ đồng phục
- **Loại:** heuristic
- **Trạng thái:** draft
- **Luật:** Mỗi thang (chữ, bo góc, icon, độ nổi, khoảng cách) có ít nhất 3 bậc, và các bậc phải **cách xa nhau đủ để mắt phân biệt**. Không gộp mọi token về một giá trị.
- **Lý do:** Phân cấp cần tương phản. Một thang chỉ có một bậc thì nhất quán tuyệt đối nhưng không còn công cụ nào để nhấn.
- **Ví dụ:** ❌ sakubun `radius-sm = md = lg = xl = 2xl`; thienui icon chỉ 16px; tiêu đề phần 14px bằng nội dung 14px. ✅ chữ 14 / 20 / 32; bo 4 / 8 / 16.
- **Nguồn:** không có nguồn duy nhất; tổng hợp từ nguyên lý contrast.
- **Bài học gốc:** M0-01 (W2) → kiểm chứng ở M1-02

---
### VIS-003 — Chỉ thứ bấm được mới nổi
- **Loại:** heuristic
- **Trạng thái:** draft
- **Luật:** Gờ, bóng hay độ nổi chỉ dành cho phần tử bấm được. Thẻ chỉ chứa thông tin thì phẳng (dùng nền hoặc khoảng cách để tách).
- **Lý do:** Độ nổi là *signifier* (Norman) của khả năng bấm. Nếu cái gì cũng nổi thì tín hiệu mất nghĩa, và màn hình nặng nề.
- **Ví dụ:** ❌ lab2 bản cam: mọi thẻ đều có gờ đáy 2px, kể cả ô số không bấm được.
- **Nguồn:** Norman, *The Design of Everyday Things* (signifiers).
- **Bài học gốc:** M0-01 (W2, W4)

---
### VIS-004 — Tiêu đề màn không phải điểm nhấn mặc định
- **Loại:** heuristic
- **Trạng thái:** draft
- **Luật:** Trong app có tab, tiêu đề màn hoặc ngày hôm nay đứng ở cấp nhãn (13–16px, không nhất thiết đậm). Bậc chữ lớn nhất dành cho thứ người dùng mở màn để xem hoặc làm.
- **Lý do:** Người dùng đã biết mình đang ở tab nào, hôm nay là thứ mấy. Đặt bậc chữ lớn nhất cho thông tin đã biết là phí điểm nhấn (Von Restorff), và nó tranh với điểm nhấn thật.
- **Áp dụng khi:** màn trong app có thanh tab/điều hướng cố định.
- **Không áp dụng khi / lưu ý:** trang đọc dài, màn chi tiết của một đối tượng (tên đối tượng chính là nội dung), web nơi tiêu đề giúp định hướng.
- **Ví dụ:** ❌ CC-01 cả 3 phương án đặt "Thứ Ba, 20/10" 22px đậm ở góc trên trái. Người dùng phê bình ngược ("tiêu đề card to hơn tiêu đề ngày") → đây là hiểu lầm cần sửa.
- **Nguồn:** *Refactoring UI* (de-emphasize; labels are a last resort).
- **Bài học gốc:** CC-01

---
### VIS-005 — Bo góc lồng nhau phải đồng tâm
- **Loại:** heuristic (gần chuẩn hình học)
- **Trạng thái:** draft
- **Luật:** Khi một khối bo góc nằm trong khối bo góc khác: bo trong = bo ngoài − khoảng đệm (tối thiểu 0–4px).
- **Lý do:** Hai đường cong không đồng tâm làm khe hở ở góc rộng hẹp không đều, mắt thấy "lệch" dù không gọi được tên.
- **Ví dụ:** ❌ CC-01 phương án A: khối cam bo 24, đệm 20, nút trắng bên trong bo 16 (đúng ra ≈ 4). Người dùng cảm thấy "bo góc rất xấu" mà chưa có từ để gọi.
- **Nguồn:** quy ước hình học; phổ biến trong cộng đồng thiết kế (Apple dùng bo liên tục "squircle", nguyên lý tương tự). Không có một nguồn gốc duy nhất.
- **Bài học gốc:** CC-01
