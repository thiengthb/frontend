# CC-01 — Phân cấp, tương phản, điểm nhấn
- **Ngày:** 2026-10-30
- **Trạng thái:** đang học (đã giảng, chờ dự đoán và phê bình của người dùng)
- **Thuật ngữ mới:** visual hierarchy, focal point, Von Restorff (isolation) effect, squint test, de-emphasize, consistency vs uniformity
- **Bài subagent:** `demos/CC-01/gv001-3-layouts.html` (3 phương án GV-001)

## 1. Khái niệm (tóm tắt bài giảng)
- Người dùng quét, không đọc. Màn nào cũng có thứ tự đọc; phân cấp là **nhà thiết kế quyết định thứ tự đó**. Câu hỏi gốc đến từ UX: họ mở màn để làm gì.
- 6 đòn bẩy: cỡ, độ đậm, màu/độ sáng tối, vị trí, khoảng trắng, hình dạng/khung. Nhấn một thứ = **hạ cấp những thứ khác** (Schoger). Nhãn thường là phụ, con số là chính.
- Tương phản theo **tỉ lệ**: 14→15→16 (×1.07) trông phẳng; 14→20→32 (×1.4–1.6) ra ba tầng. lab2: 22→16→15.
- Von Restorff (1933): thứ khác biệt được chú ý. Một điểm nhấn mỗi màn; mọi thứ nổi = không gì nổi. Điểm nhấn là thứ **khác biệt nhất**, không nhất thiết to nhất.
- Squint test: làm mờ, hỏi mảng nào thắng, bao nhiêu mảng tranh nhau, có thấy nhóm không.
- Nhất quán = cùng một thang; đồng phục = chỉ một bậc của thang.

## 1b. Video (người dùng bỏ qua do thiếu thời gian, 2026-10-31) — tóm tắt thay thế
Schoger, *Practical Solutions to Common UI Design Problems*. Tóm tắt dựa trên nội dung talk và sách *Refactoring UI* cùng tác giả; Claude không xem lại được video nên thứ tự/ví dụ có thể lệch.
1. Phân cấp không chỉ bằng cỡ: dùng độ đậm và màu (đen / xám đậm / xám nhạt) cho 3 tầng.
2. Nhấn bằng cách hạ cấp thứ xung quanh (vd tab không active nhạt đi, thay vì tô màu tab active).
3. Nhãn là phương án cuối: gộp nhãn vào giá trị ("còn được vắng 1" thay vì "Số buổi còn lại: 1").
4. Không đặt chữ xám trên nền màu; dùng sắc độ cùng hue với nền.
5. Bớt viền: tách bằng nền khác màu, bóng, hoặc khoảng cách.
6. Khoảng cách không mơ hồ: trong nhóm < giữa nhóm.
7. Bắt đầu với dư khoảng trắng rồi bớt dần.
8. Nút theo phân cấp, không theo ngữ nghĩa: primary đặc, secondary viền, tertiary dạng link.
9. Cân trọng lượng–tương phản: icon đặc/nặng thì hạ tương phản để không lấn chữ.
- Dự đoán trước khi xem bài: **bỏ qua** khối này (người dùng thiếu thời gian).

## 2. Ví dụ
- Demo inline (trong chat): màn ôn tập "đồng phục" (4 ô KPI + nút cùng viền) vs "có phân cấp" (số 56px, nút đặc, chỉ số phụ thành 1 dòng xám), kèm thanh làm mờ.

## 3. Phản biện
- Bảng dữ liệu cần so sánh: đồng phục là đúng; phân cấp ở cấp bảng và hàng bất thường.
- Màn nhiều việc ngang hàng (launcher, cài đặt): đừng ép điểm nhấn giả, phân cấp bằng nhóm.
- Hiểu lầm: "phân cấp = tiêu đề to hơn"; "điểm nhấn = thứ to nhất".
- Ý kiến của người dùng: (chờ)

## 4. Bài tập (Critique Loop)
- Dự đoán của người dùng: (chờ)
- Phê bình của người dùng: (chờ, chép theo `templates/critique.md`)

<details>
<summary>⛔ Phê bình tham chiếu của Claude — viết TRƯỚC khi đọc bài của người dùng. Người dùng: đừng mở trước khi tự phê bình.</summary>

**Viết lúc:** 2026-10-30, ngay sau khi subagent xong, trước khi người dùng gửi dự đoán.

### Nhận định chung
Bài tốt hơn mức mặc định mình kỳ vọng. Cả ba phương án đều **bỏ lưới 4 ô KPI khỏi vị trí đầu** và đưa hành động "Điểm danh" lên làm điểm nhấn (đúng UX-001, chữa đúng W3). Lý do: brief có persona, nỗi sợ, giờ cụ thể. Đây chính là luận điểm `docs/00-perspective.md` §1: đề bài đủ thì AI làm khá. Lỗi còn lại tinh vi hơn, nằm ở thứ tự đọc, thang chữ, màu nhấn bị pha loãng và cách nhóm thông tin.
**Điểm bài subagent: 7/10.**

### Vấn đề, xếp từ nặng nhất
| # | Chỗ nào | Vấn đề (thuật ngữ) | Vì sao | Mức | Hướng sửa |
|---|---|---|---|---|---|
| 1 | C, góc phải trên | Giữ và **nâng cấp vanity metric** "94%" lên cỡ tiêu đề, ngang với ngày | Mâu thuẫn chính lý do của C (bỏ 4 lớp/131 vì không giúp quyết định). Squint: ngày, 94%, PRM393, nút = 4 mảng đậm tranh nhau ở 1/3 trên | cao | Hạ 94% xuống dòng phụ xám hoặc bỏ; để nút là mảng duy nhất thắng |
| 2 | C, nhóm Chú ý | Chỉ hiện sinh viên thuộc lớp có lịch hôm nay | Đánh mất nỗi sợ số 2 (phát hiện muộn). Em quá ngưỡng ở lớp không dạy hôm nay biến mất khỏi Tổng quan. Đánh đổi IA lớn mà phần ghi chú nói nhẹ | cao | Giữ nhóm gắn slot, nhưng thêm một dòng "+n em ở lớp khác" dẫn tới Xem tất cả |
| 3 | A, thứ tự khối | **Thứ tự thời gian đảo ngược**: "Tiếp theo 12:30" nằm TRÊN slot đang diễn ra 07:00 | Vi phạm mapping (Norman) giữa vị trí và thời gian; mắt đọc từ trên đọc tương lai trước hiện tại | cao | Đưa 12:30 xuống dưới khối cam, hoặc gộp vào dòng phụ trong khối |
| 4 | A, khối cam | **Vùng chạm lồng nhau**: cả khối bấm được, bên trong lại có nút trắng; thêm câu giải thích "Chạm để mở mã QR…" | Signifier mơ hồ (bấm đâu?). Câu hướng dẫn là nạng chống (W5), phạm luật T1 của lab2 | vừa | Một vùng chạm duy nhất (nút), bỏ câu giải thích, nhãn nút tự nói "Mở QR điểm danh" |
| 5 | Cả ba, header | Ngày "Thứ Ba, 20/10" làm tiêu đề 22px đậm, góc trên trái | Lãng phí vị trí đọc đầu tiên cho thông tin ít giá trị quyết định nhất (GV biết hôm nay thứ mấy). Phản xạ mặc định | vừa | Hạ ngày thành nhãn 13–14px xám; vị trí đầu cho trạng thái slot |
| 6 | B, C | **Thang chữ vẫn phẳng**: ngày 22 ≈ PRM393 24, body 15–16. Chỉ A dùng display (~40px) | W2 lặp lại ở mức nhẹ hơn: hai tiêu đề gần bằng nhau triệt tiêu nhau | vừa | Một bậc display (32–40) cho mã môn hoặc giờ, các tiêu đề khác ≤ 16 |
| 7 | Cả ba, đặc biệt B | **Màu nhấn bị pha loãng**: cam cho nút, link "Xem tất cả", chấm trạng thái, chữ cảnh báo, pill tab active, nền mặt phẳng | Cam không còn nghĩa "hành động chính" (COL-001, Von Restorff). B có ~6 vai trò cam | vừa | Link và tab active về trung tính đậm; cam đặc chỉ cho nút |
| 8 | B, ranh giới mặt phẳng | **Common region nhóm sai**: Trang và Long học SE1801 đang diễn ra, nhưng nằm ngoài mặt phẳng "hôm nay"; hàng số liệu 94/4/131 vẫn còn | Chia theo "hôm nay / tham khảo" cắt đứt quan hệ giữa slot và sinh viên của nó; vanity metric chỉ bị hạ chứ không bị hỏi lại | vừa | Đưa sinh viên của lớp đang dạy vào mặt phẳng; hàng số liệu thành 1 dòng xám hoặc bỏ |
| 9 | C, trục thời gian | Lề trục giờ ăn ~70px trên khung 360; lồng 4 tầng (trục > slot > hộp > hàng có pill) | Mật độ chật, nhiều ranh giới lồng nhau | thấp | Bỏ hộp nền, dùng thụt lề và khoảng cách |
| 10 | A vs B/C | Microcopy không nhất quán: "còn được vắng 1" vs "sắp chạm" | A tốt hơn (nói thẳng hệ quả, hành động được) | thấp | Dùng cách nói của A cho cả ba |
| 11 | Cả ba | Không nghĩ tới **trạng thái sau khi điểm danh xong** (chỉ A nhắc trong chú thích) | Điểm nhấn hợp lý lúc 07:05 sẽ vô nghĩa lúc 07:20 | thấp | Ghi chú biến thể sau điểm danh |

### Điểm tốt thật
1. **Cả ba bỏ lưới KPI khỏi màn đầu** và đặt "Điểm danh" làm điểm nhấn: đúng câu hỏi "mở màn để làm gì" (UX-001, chữa W3).
2. **B làm đúng tầng 20%**: mặt phẳng cam nhạt là figure–ground có nghĩa (gom việc hôm nay), không tô từng thẻ; chỉ một mảng cam đặc (nút). Đúng ghi chú COL-001.
3. **C có insight IA thật**: nối sinh viên cần chú ý với lớp đang dạy (quan hệ giữa dữ liệu, không để từng silo); đặt yêu cầu sửa vào khoảng trống 09:15–12:30.
4. **A dùng vùng ngón cái** (reachability) và một bậc display thật (PRM393 ~40px); trạng thái "đã bắt đầu 5 phút, bạn chưa điểm danh" chạm đúng nỗi sợ số 1 (Nielsen #1 visibility of system status).
5. Chú thích trung thực về đánh đổi dưới mỗi khung.

### Nếu chỉ sửa MỘT thứ
Pha loãng màu nhấn (#7) và tiêu đề ngày (#5) cùng một gốc: các phương án **thêm** điểm nhấn mà quên **hạ cấp** phần còn lại. Sửa một thứ: hạ ngày và mọi link/tab cam về trung tính, để mỗi khung chỉ còn **một** mảng thắng khi nheo mắt.

### Checklist chấm người dùng (Recall)
Vấn đề "phải tìm thấy" để Recall 2/2: ít nhất 3 trong {#1, #2, #3, #4, #5/#6, #7, #8}, trong đó có ít nhất một vấn đề UX (#2, #3 hoặc #8) chứ không chỉ thị giác.
</details>

## 5. Review
(chờ, Claude chấm cả hai sau khi người dùng phê bình)

## 6. Luật rút ra
(chờ)

## Tóm tắt cho khối sau
(viết khi kết thúc khối)

## Quiz nhớ lại (cho đầu CC-02)
(viết khi kết thúc khối)
