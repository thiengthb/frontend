# 06 — Từ điển ra lệnh cho AI

> Mỗi khối V-xx thêm một mục. Cột trái là cách nói mơ hồ; cột phải là câu lệnh dùng đúng thuật ngữ, copy dán cho AI được.
> Mục đích: biến cảm giác ("nhạt", "rối", "xấu") thành chỉ dẫn mà AI làm đúng.

## V-01 · Phân cấp & điểm nhấn (đã học sơ ở CC-01)
| Bạn cảm thấy | Câu lệnh cho AI |
|---|---|
| "Nhạt, đơn điệu, cái gì cũng như nhau" | "Tạo **một focal point duy nhất** cho màn: [hành động/số liệu]. Mọi thứ khác **de-emphasize** (nhỏ hơn, nhạt hơn, nhẹ hơn). Kiểm bằng **squint test**: làm mờ màn thì chỉ một mảng thắng." |
| "Màn này để làm gì?" | "Màn bắt đầu từ **hành động chính**, không bắt đầu từ số liệu. Hành động chính phải nằm trong **viewport đầu tiên**. Bỏ **vanity metric** (số không dẫn tới quyết định)." |
| "Tiêu đề to quá" | "Tiêu đề màn **không phải điểm nhấn mặc định**: đặt nó 13–16px; cỡ lớn nhất dành cho [điều người dùng mở màn để làm]." |
| "Bo góc trông lệch" | "Bo góc lồng nhau **đồng tâm**: bán kính trong = bán kính ngoài − padding." |
| "Thống nhất quá thành cứng" | "**Nhất quán ≠ đồng phục**: dùng cùng một thang, nhưng dùng nhiều bậc cách xa nhau (chữ, bo, độ nổi)." |

## V-02 · Typography (đã học sơ ở nửa đầu CC-02)
| Bạn cảm thấy | Câu lệnh cho AI |
|---|---|
| "Chữ phẳng, không phân tầng" | "Dùng **modular scale** gốc 15px tỉ lệ **1.25**, tối đa 5 cỡ (13 / 15 / 18 / 24 / 36). Được **bỏ bậc** để tạo khoảng nhảy ở điểm nhấn. Không dùng cỡ lẻ ngoài thang." |
| "Chữ nào cũng đậm" | "Độ đậm có vai: **400** cho chữ đọc, **600** cho tên và nhãn bấm được, **700** chỉ cho 2 cỡ lớn nhất. Tách tầng bằng cách **hạ cấp** chữ phụ (400, xám) trước khi phóng to chữ chính." |
| "Cột số lệch" | "Dùng **tabular figures** (`font-variant-numeric: tabular-nums`) và căn phải cho mọi cột số, giờ, x/4." |
| "Dấu tiếng Việt bị đụng" | "**line-height** ≥ 1.4 cho chữ nhiều dòng; chữ in hoa tiếng Việt cần rộng hơn. Chọn font vẽ dấu chồng tốt (thử 'Nguyễn Thị Hường – ỄỮẪ')." |
| "Nhấn mạnh kiểu gì" | "Gạch chân **chỉ cho link**. Nghiêng chỉ để nhấn trong câu. In hoa chỉ cho nhãn 1–2 từ, kèm letter-spacing +0.05em." |
