# CC-02 — Typography: thang tỉ lệ, độ đậm, chữ số, tiếng Việt
- **Ngày:** 2026-10-31
- **Trạng thái:** dừng giữa khối (2026-10-31): người dùng đổi sang crash course trực quan (D-018). Nội dung chuyển vào V-02.
- **Bài subagent:** `demos/CC-02/type-scale-gv103.html` (thang chữ mới + GV-103 Chi tiết lớp)

## 0. Quiz nhớ lại CC-01 — 1.5/3
- C1 ½: chẩn đoán đúng (bước sát nhau), nhưng trả lời bằng cỡ chữ (đề hỏi đòn bẩy khác cỡ) và đề xuất 16→12→8 (8px dưới ngưỡng đọc). Muốn bước lớn thì đi **lên** (display), đừng đi xuống.
- C2 0: trả lời 16px; đúng là ≈4px (24 − 20), bo góc không đồng tâm (VIS-005). Đã giải thích lại bằng tâm cung chung.
- C3 1: đúng lý do; ví dụ "trang giới thiệu" chấp nhận được.
- 0b: người dùng bỏ qua; Claude làm mẫu (common region nhóm sai · vanity metric chỉ bị hạ · ngày 22 vs PRM393 24 · cam pha loãng).

## 1. Khái niệm (bài giảng đã trình bày trong chat)
- **Modular scale:** gốc + tỉ lệ (1.2 quãng ba thứ, 1.25 quãng ba trưởng, 1.333 quãng bốn, 1.5 quãng năm). Mắt so theo tỉ lệ: ×1.07 vô hình, ×1.6 ra tầng. App dày/màn nhỏ 1.2–1.25; landing 1.333–1.5. Dùng 4–6 bậc, được bỏ bậc. Có **sàn** ~12–13px: tương phản đi lên, không đi xuống. Phản biện: heuristic; giá trị thật là ít bậc và cách xa.
- **Đậm / nghiêng / gạch chân / in hoa:** đậm tách tầng khi cùng cỡ (đừng 600 khắp nơi); nghiêng nhấn trong câu, không cho nhãn; gạch chân chỉ cho link; in hoa chỉ nhãn 1–2 từ + tracking, cẩn thận dấu chồng.
- **Chữ số:** proportional cho văn; **tabular** cho bảng, cột x/4, giờ, số đếm.
- **Tiếng Việt:** dấu chồng (ễ, ữ, ẫ) cao hơn Latin; line-height đoạn 1.4–1.6, dưới ~1.25 dấu chạm dòng trên; display một dòng được thấp hơn; chọn font vẽ dấu tốt.
- Demo inline: thang cũ ×1.07 vs ×1.25 cùng Nunito; proportional vs tabular; thanh trượt line-height với chữ hoa có dấu.
- Video Elliot Jay Stocks: trang phiên Config tồn tại, không tìm được bản ghi (⚠); đề xuất bỏ (D-017).

## 4. Bài tập (Critique Loop)
- Dự đoán của người dùng: (chờ)
- Phê bình của người dùng: (chờ)

<details>
<summary>⛔ Phê bình tham chiếu của Claude — viết TRƯỚC khi người dùng xem bài và phê bình. Người dùng: đừng mở trước.</summary>

**Viết lúc:** 2026-10-31 ~20:40, ngay sau khi subagent xong, trước khi bài được publish cho người dùng.

### Nhận định chung
**Thang chữ (Việc 1) tốt**: 5 cỡ 13 / 15 / 18 / 24 / 36, bước ×1.2–1.5, ba độ đậm có vai rõ (400 đọc, 600 gọi tên/chạm, 700 chỉ cho hai cỡ lớn), sàn 13 giữ đúng, chữ số tabular. Đây là chữa đúng W2 ở tầng công cụ.
**Màn GV-103 (Việc 2) dùng thang đúng kỹ thuật nhưng đặt điểm nhấn sai chỗ**: cỡ 36, bậc mạnh nhất, dành cho "35 sinh viên" và "6/20 buổi", hai con số không dẫn tới quyết định nào. Con số trả lời câu hỏi "lớp này khỏe không" (1 cấm thi, 1 sát ngưỡng) nằm trong pill 13px. Lặp lại đúng lỗi #1 của CC-01 (vanity metric chiếm vị trí đầu, W3). Bài học trung tâm: **thang chữ là công cụ, còn quyết định cái gì to là chuyện của nội dung**.
**Điểm bài subagent: 6/10.**

### Vấn đề, xếp từ nặng nhất
| # | Chỗ nào | Vấn đề (thuật ngữ) | Vì sao | Mức | Hướng sửa |
|---|---|---|---|---|---|
| 1 | Khối "sức khỏe", hai số 36px | **Điểm nhấn đặt sai** (focal point dành cho vanity metric) | Mục đích màn là sức khỏe chuyên cần. 35 và 6/20 không đổi quyết định nào; số rủi ro chỉ có 13px. Squint: hai số đen 36 thắng | cao | Display cho "2 em cần chú ý" (hoặc "1 cấm thi · 1 sát ngưỡng"); 35 SV và 6/20 thành một dòng meta |
| 2 | Dòng cuối danh sách | **Bịa dữ liệu**: "Còn 27 sinh viên khác, đều 0/4" | Brief chỉ nói "còn 27 em khác". Thông tin sai trên màn chuyên cần làm mất lòng tin; và chữ thay cho danh sách thật làm mất khả năng cuộn tìm | cao | Hiện các hàng thật (cuộn), không viết câu tổng kết tự đặt |
| 3 | Ba pill trạng thái | **Signifier mơ hồ + màu dàn trải** | Pill trông như chip lọc (bấm được?) nhưng không phải. "33 an toàn" xanh lá thêm một màu cho thứ không cần hành động (Von Restorff yếu đi) | vừa | Nếu là bộ lọc thì làm thật (chip có trạng thái chọn, CMP-001); nếu chỉ là số thì bỏ "an toàn", gộp vào câu |
| 4 | Thanh tiến độ, tab active, focus ô tìm | **Cam dùng để trang trí** | Màn không có hành động chính nào cam; cam xuất hiện ở progress bar (thông tin, không phải hành động) → mất nghĩa "cam = hành động" (COL-001) | vừa | Progress và tab active về trung tính đậm `#1F1F1F` |
| 5 | Font | **Đổi hai biến cùng lúc** (thang + font Nunito → Be Vietnam Pro) | Khi so trước/sau, không biết cải thiện đến từ thang hay từ font; đổi cá tính thương hiệu (tròn, thân thiện) mà không được yêu cầu. Lý do kỹ thuật thật (dấu chồng, tabular) nhưng Nunito cũng hỗ trợ tiếng Việt | vừa | Làm thang mới trên Nunito trước; đổi font là quyết định riêng, có A/B |
| 6 | Khối sức khỏe | **Lồng khung**: card có viền, trong có viền dọc, viền ngang, rồi pill nền màu | Nhiều ranh giới cho một nhóm nhỏ (Schoger: bớt viền) | thấp | Bỏ viền card, tách bằng nền muted hoặc khoảng trắng |
| 7 | Mỗi hàng | **SemiBold dày đặc**: tên 600, số 18/600, nhãn trạng thái 600 | 600 xuất hiện mọi nơi thì độ đậm mất sức tách tầng (đồng phục ở trục đậm) | thấp | Tên giữ 600, số 0/1 về 400 xám (đã làm với 0, nên mở rộng) |
| 8 | Header | SE1801 24/700 + hai số 36 + số đỏ: 4 mảng đậm ở 1/3 trên | Đây là màn chi tiết nên tên lớp làm tiêu đề lớn được phép (đáp án quiz 3), nhưng cạnh tranh với số | thấp | Khi đã sửa #1, giảm còn một số display |

### Điểm tốt thật
1. **Thang ít bậc, bước rõ**: 5 cỡ, ×1.2–1.5; bỏ hẳn 14/16/17 sát nhau. Lý do bỏ bậc n=3 (≈29) để số tách khỏi tiêu đề là lập luận có nguyên lý.
2. **Độ đậm có ngữ nghĩa**: 400 / 600 / 700 với vai rõ; Bold chỉ cho cỡ lớn. Thang cũ gần như kiểu nào cũng Bold/SemiBold.
3. **Chữ số tabular + căn phải** cho cột x/4: số thẳng cột, so nhanh. "/4" hạ xám, số 0 hạ xám: hạ cấp đúng cách.
4. **Không dùng màu một mình**: hàng đỏ có thêm chữ "Đã bị cấm thi" (WCAG 1.4.1).
5. Dòng "Vắng nhiều nhất trước · ngưỡng 4 buổi" giải thích thứ tự sắp xếp mà không thành nạng chống; chú thích đánh đổi trung thực.

### Nếu chỉ sửa MỘT thứ
#1: chuyển bậc display từ "35 / 6" sang số em có rủi ro. Thang đã đúng; chỉ cần đặt cỡ to vào đúng câu trả lời.

### Checklist chấm người dùng (Recall)
Để Recall 2/2: tìm được #1 và ít nhất 2 trong {#2, #3, #4, #5, #6}. Bắt được #2 (dữ liệu bịa) là điểm cộng lớn vì không phải lỗi thị giác.
</details>
