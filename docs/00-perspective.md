# 00 — Phản biện & góc nhìn nền tảng

## 1. "AI thiết kế đẹp nhưng thiếu chiều sâu": đúng, nhưng nguyên nhân chính không nằm ở AI
AI tạo ra giao diện "trung bình đẹp" vì khi thiếu ràng buộc, nó chọn **mặc định an toàn nhất**: gradient tím, card bo góc,
font Inter, hero ở giữa. Thiếu chiều sâu thường là do **đề bài thiếu**, không chỉ do năng lực AI. Cụ thể là thiếu:
- **Người dùng là ai**, đang ở bối cảnh nào, muốn hoàn thành việc gì (job-to-be-done).
- **Nội dung thật** (AI hay thiết kế quanh lorem ipsum).
- **Cá tính thương hiệu** (3–5 tính từ kèm phản đề: "nghiêm túc, KHÔNG lạnh lùng").
- **Hệ thống**: token màu, thang chữ, thang spacing. Không có hệ thống thì không thể nhất quán.
- **Lý do**: không ai yêu cầu AI giải thích vì sao chọn như vậy.

→ Kỹ năng quan trọng nhất của bạn khi làm việc với AI là **viết được đề bài và bộ luật**, rồi **phê bình (critique) được kết quả bằng ngôn ngữ chuyên môn**.
Repo này chính là để luyện hai việc đó.

## 2. "Gu" không phải năng khiếu bẩm sinh
Gu hình thành qua: **tiếp xúc nhiều** → **phân tích** vì sao cái này tốt → **gọi tên được** (từ vựng) → **tự làm và nhận phê bình**.
Bạn chỉ điều khiển được AI ở mức chi tiết mà bạn gọi tên được. "Bớt đơn điệu" là chỉ dẫn mơ hồ.
"Tăng tương phản về kích thước giữa heading và body, thêm một màu nhấn cho CTA" là chỉ dẫn mà AI làm đúng được.

## 3. Không có "UX chuẩn" tuyệt đối, chỉ có ba tầng
| Tầng | Ví dụ | Mức bắt buộc |
|---|---|---|
| **Chuẩn (standards)** | WCAG (trợ năng), quy ước nền tảng (Apple HIG, Material), quy ước web (link có gạch chân hoặc phân biệt rõ) | Gần như bắt buộc |
| **Heuristic & nguyên lý** | 10 heuristic của Nielsen, Gestalt, Fitts, Hick, Jakob | Nên theo, có ngoại lệ |
| **Quy tắc kinh nghiệm (rule of thumb)** | 60-30-10 / 70-20-10, thang 8pt, tỉ lệ vàng | Công cụ khởi đầu, không phải luật |

Rất nhiều "luật UX" trên mạng bị **trích sai**. Ví dụ, "con số 7±2" của Miller nói về bộ nhớ ngắn hạn trong thí nghiệm,
không có nghĩa là "menu tối đa 7 mục". Mỗi luật trong repo phải ghi rõ **thuộc tầng nào**.

## 4. Về luật 70-20-10 mà thầy bạn gợi ý
- Đây là quy tắc **tỉ lệ phân bổ màu** (bản phổ biến hơn là **60-30-10**, xuất phát từ thiết kế nội thất):
  ~70% màu nền/trung tính, ~20% màu phụ (mảng, thẻ, section), ~10% màu nhấn (CTA, trạng thái, điểm nhấn).
- **Điểm mạnh:** chống được hai lỗi phổ biến là "toàn xám trắng, không có điểm nhấn" (đơn điệu) và "màu nào cũng mạnh" (rối).
- **Giới hạn:** tỉ lệ tính theo **diện tích thị giác**, không phải theo số lượng element. Màu nhấn phải gắn với **ý nghĩa**
  (hành động chính) chứ không rải để trang trí.
- **Phản biện quan trọng:** "đơn điệu" chưa chắc chỉ do màu. Thường nó đến từ thiếu **tương phản** (kích thước, độ đậm, khoảng trắng),
  thiếu **nhịp điệu** (rhythm, mọi section giống hệt nhau) hoặc thiếu **phân cấp** (hierarchy, mọi thứ quan trọng ngang nhau).
  Mình sẽ cùng bạn chẩn đoán thiết kế thật để biết nguyên nhân thực sự.

## 5. UI ≠ UX
- **UI** trả lời câu hỏi: *trông thế nào, cảm giác ra sao* (thị giác, chữ, màu, component).
- **UX** trả lời câu hỏi: *có giải quyết đúng vấn đề, dễ dùng, không gây bối rối không* (luồng, cấu trúc thông tin, phản hồi, lỗi, trợ năng).
Một giao diện rất đẹp vẫn có thể có UX tệ. Chiều sâu thật sự nằm ở UX, nên lộ trình dành nhiều thời gian cho phần này.

## 6. Rủi ro của chính kế hoạch này (để mình tự canh)
- **Học lý thuyết vô tận mà không làm.** Cách khắc phục: mỗi bài phải có bài tập và sinh ra luật.
- **Bộ luật phình to và mâu thuẫn.** Cách khắc phục: mỗi luật có ID, loại, lý do và trạng thái; luật mới phải được duyệt.
- **Luật hoá quá mức làm mất sáng tạo.** Cách khắc phục: phân biệt luật cứng với heuristic, và cho phép phá luật nếu có lý do ghi rõ.
- **Lệch ý giữa các phiên AI.** Cách khắc phục: `PROGRESS.md`, `DECISIONS.md` và nghi thức đầu/cuối phiên trong `CLAUDE.md`.
