# Brief GV-001 cho lab2 (bản dán cho AI)

> Bản chữ của brief GV-001 ráp từ khối V-15 (`demos/V-15/brief.html`), ở **lựa chọn mặc định**: mọi phần kèm câu lệnh, mỗi quyết định lấy phương án đầu.
> Bảy quyết định trong phần Cá tính, Ràng buộc, Điều hướng, Trạng thái là **chưa chốt**: chỉnh trong artifact rồi copy lại, hoặc sửa thẳng ở đây.
> Dán nguyên khối dưới đây cho AI (Claude, v0, Figma Make…). Không cần đưa thêm `rules/`.

````text
# Brief: GV-001 Tổng quan · lab2, app điểm danh cho giảng viên

## 1. Mục tiêu
Màn GV-001 Tổng quan là tab đầu tiên của app Android điểm danh cho giảng viên đại học FPT.
Hành động chính, chỉ một: mở điểm danh cho slot đang diễn ra.
Thành công khi giảng viên mở app và bấm Điểm danh trong dưới 5 giây, không phải cuộn.
- Màn bắt đầu từ hành động chính, không từ số liệu. Hành động chính nằm trong màn đầu tiên (cao 640dp, cỡ chữ 115%).
- Đúng một điểm nhấn: thẻ slot đang diễn ra và nút Điểm danh. Mọi thứ khác nhỏ hơn, nhạt hơn. Làm mờ màn thì chỉ một mảng thắng.

## 2. Người dùng
Giảng viên dạy 3–4 slot mỗi ngày, quen mặt sinh viên.
Lúc dùng: 07:05 sáng thứ Ba, vừa vào lớp, đứng trong phòng học sáng đèn, cầm điện thoại một tay.
Việc cần làm: mở điểm danh đúng lớp thật nhanh, rồi biết em nào sắp bị cấm thi.
Nỗi lo: quên điểm danh thì bị trừ lương; phát hiện muộn em vắng quá 20% số buổi thì em đó bị cấm thi.
- Nút chính rộng hết màn, cao 48–56dp, nằm ở nửa dưới màn trong vùng ngón cái.
- Đọc được trong phòng sáng: chữ đạt WCAG 2.2 AA (4.5:1 chữ thường, 3:1 chữ từ 24px).

## 3. Nội dung thật
Theo thứ tự quan trọng (giữ nguyên dữ liệu):
1. Slot đang diễn ra: 07:00–09:15 · PRM393 · SE1801 · P.305 · 0/35 đã quét · nút Điểm danh (mở mã QR)
2. Chú ý: Lê Thu Trang (SE190142, SE1801) vắng 5/4 buổi cho phép, đã quá ngưỡng; Trần Minh Long (SE190155, SE1801) vắng 3/4, sắp chạm. Link Xem tất cả.
3. Slot sau: 12:30–14:45 · MMA301 · SE1805 · P.402
4. 2 yêu cầu sửa điểm danh
5. Ngữ cảnh: Thứ Ba, 20/10 · Fall 2026
6. Số tổng (4 lớp, 131 sinh viên, 94% có mặt tuần này): gộp thành một dòng phụ hoặc bỏ.
Có thể rỗng hoặc dài: hôm nay không có slot; nhóm Chú ý trống; tên sinh viên bốn chữ.
- Không lưới số liệu ở đầu màn. Cỡ chữ lớn nhất chỉ dành cho con số trả lời câu hỏi chính (0/35 đã quét).
- Mỗi hàng Chú ý: tên in đậm ở đầu dòng, trạng thái thành nhãn ở cuối dòng, có cả màu và chữ.
- Số và giờ dùng tabular figures.

## 4. Cá tính
- Ấm, KHÔNG trẻ con: cam FPT và chữ tròn, nhưng không gờ dày kiểu app học, không minh hoạ.
- Đáng tin, KHÔNG cứng nhắc: số liệu chính xác, nhãn rõ, nhưng có khoảng thở và một điểm nhấn.
- Nhanh, KHÔNG vội vàng: hành động chính ngay trước mắt, chuyển động ngắn, không nảy.
Muốn giống: các app Material 3 của Google (màu tonal, một nút chính đặc).
Không muốn giống: template dashboard có lưới bốn ô số; Duolingo (gờ dày, nảy).
Phong cách: Material 3 cho Android. Khối nền tonal (soft #FBEFE8) gom việc của hôm nay; thẻ thông tin phẳng; chỉ nút chính đặc màu.
- Chỉ thứ bấm được mới có bóng hoặc gờ. Mỗi khối chỉ một tín hiệu tách nền: khoảng trắng, hoặc nền, hoặc viền 1px, hoặc bóng.

## 5. Ràng buộc và token
Android, khung 360×800, status bar 07:05 ở trên. Font Nunito, tiếng Việt có dấu. Icon Lucide nét 2. Avatar dùng chữ cái đầu.
Chỉ dùng các màu: nền #FFFFFF; muted-surface #F4F4F4; border #E5E5E5; chữ #1F1F1F / #3C3C3C / #6B6B6B; primary #B9551F (pressed #8A3D14, soft #FBEFE8, chữ trên soft #9A4518); success #15803D / #ECFDF3; warning #A15C00 / #FFF6DD; danger #B42318 / #FEF0EF.
Khoảng cách theo lưới 4: 4, 8, 12, 16, 24, 32.
Vùng chạm tối thiểu 48dp. Nút cao 40 (trong thẻ) và 36 (trong hộp thoại) giữ cỡ nhìn thấy nhưng mở vùng chạm vô hình tới 48dp, cách nhau ít nhất 8dp.
- Thang chữ ít bậc nhưng cách xa: 13 / 15 / 18 / 24 / 36. Độ đậm 400 cho chữ đọc, 600 cho nhãn, 700 chỉ cho hai cỡ lớn nhất.
- Tầng màu phụ khoảng 20% diện tích là một mặt nền soft gom việc của hôm nay, không tô màu từng thẻ. Màu nhấn tối đa khoảng 10%, chỉ cho nút chính.
- Khoảng trong nhóm 8, giữa nhóm 24, giữa section 32. Lề màn 16.
- Bo đồng tâm, ba bậc: nút 8, thẻ 12, sheet 20, chip tròn hẳn.

## 6. Điều hướng
Thanh điều hướng dưới 4 tab: Tổng quan (đang chọn), Lịch, Lớp, Tài khoản.
Yêu cầu sửa điểm danh hiện ở Tổng quan thành một dòng có số; chạm để mở danh sách trong ngăn xếp của Tổng quan.
Chạm một em ở nhóm Chú ý thì mở hồ sơ trong ngăn xếp của Tổng quan; nút ‹ quay về Tổng quan, giữ vị trí cuộn.
Màn Điểm danh mở được từ Tổng quan và từ Lịch; nút ‹ về đúng nơi đã mở.
- Mỗi màn con có top app bar ghi tên mục đang xem và nút ‹. Mỗi tab giữ back stack riêng.
- Mở từ thông báo vào màn sâu thì dựng sẵn back stack đầy đủ và chọn đúng tab.

## 7. Trạng thái
Vẽ đủ các trạng thái: .D có dữ liệu; .L đang tải; .E hôm nay không có slot; .E2 lần đầu dùng; .X mất mạng.
.X mất mạng: giữ dữ liệu đã tải, hiện một dải báo có giờ cập nhật cuối; thao tác cần mạng vào hàng chờ và tự gửi khi có mạng.
Chốt điểm danh: chốt ngay, hiện snackbar "Đã chốt 34/35" có nút Hoàn tác khoảng 5 giây; không hộp xác nhận.
- Đang tải dùng skeleton đúng hình nội dung, không spinner giữa màn.
- Nút đổi trạng thái trong 0,1 giây khi chạm; chờ quá 1 giây thì nút thành "Đang mở…" và bị khoá.
- Empty state có một câu nói màn để làm gì và nút cho bước đầu; không dùng "Không có dữ liệu".
- Lỗi trả lời ba câu: hỏng gì, dữ liệu vừa nhập còn không, bấm gì để sửa.
- Sau khi chốt có màn hoặc thông báo kết thúc rõ, ghi kết quả cụ thể (34 có mặt, 1 vắng).

## 8. Chuyển động
Chuyển động ít và có mục đích; không có hoạt hình trang trí.
- Mở sheet mã QR: 300–400ms, easing cubic-bezier(0.05, 0.7, 0.1, 1), mở rộng từ nút Điểm danh; đóng 200–250ms, thu về đúng nút đó.
- Kéo sheet xuống để đóng dùng spring, damping ratio 0.8–1, truyền vận tốc cú vuốt.
- Đổi tab: fade through khoảng 250ms, không trượt ngang.
- Nút lún còn 0.97 trong khoảng 100ms khi chạm.
- Chỉ animate transform và opacity. Khi bật prefers-reduced-motion, thay bằng mờ dần tối đa 150ms.

## 9. Đầu ra và lệnh cấm
Đầu ra: ba hướng khác nhau về cấu trúc cho GV-001, cùng nội dung và token. Mỗi hướng ghi: tên phong cách; một câu về điểm nhấn và vì sao giảng viên cần thấy nó đầu tiên lúc 07:05; điều phương án hy sinh; tỉ lệ contrast của nút chính. Không tự chọn hướng tốt nhất, tôi sẽ chọn.
Nếu brief thiếu hoặc mâu thuẫn, hỏi tôi tối đa ba câu trước khi vẽ.
- Không dùng: gradient tím xanh, lưới bốn ô số ngang hàng, thẻ bo lớn có bóng cho mọi khối, emoji làm icon, font khác Nunito, tiêu đề kiểu khẩu hiệu, căn giữa nội dung.
- Mỗi màn đúng một nút đặc màu. Nhãn nút là động từ cộng đối tượng (Điểm danh, Chốt điểm danh). Không dùng switch để đánh dấu có mặt.
````
