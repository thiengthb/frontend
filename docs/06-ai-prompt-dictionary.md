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
| "Màu cam ở khắp nơi" | "Màu nhấn chỉ dùng cho **một mảng**: nút hành động chính. Link, tab đang chọn, chấm trạng thái chuyển về **trung tính đậm**." |
| "Thống nhất quá thành cứng" | "**Nhất quán ≠ đồng phục**: dùng cùng một thang, nhưng dùng nhiều bậc cách xa nhau (chữ, bo, độ nổi)." |

## V-02 · Typography (đã học sơ ở nửa đầu CC-02)
| Bạn cảm thấy | Câu lệnh cho AI |
|---|---|
| "Chữ phẳng, không phân tầng" | "Dùng **modular scale** gốc 15px tỉ lệ **1.25**, tối đa 5 cỡ (13 / 15 / 18 / 24 / 36). Được **bỏ bậc** để tạo khoảng nhảy ở điểm nhấn. Không dùng cỡ lẻ ngoài thang." |
| "Chữ nào cũng đậm" | "Độ đậm có vai: **400** cho chữ đọc, **600** cho tên và nhãn bấm được, **700** chỉ cho 2 cỡ lớn nhất. Tách tầng bằng cách **hạ cấp** chữ phụ (400, xám) trước khi phóng to chữ chính." |
| "Cột số lệch" | "Dùng **tabular figures** (`font-variant-numeric: tabular-nums`) và căn phải cho mọi cột số, giờ, x/4." |
| "Dấu tiếng Việt bị đụng" | "**line-height** ≥ 1.4 cho chữ nhiều dòng; chữ in hoa tiếng Việt cần rộng hơn. Chọn font vẽ dấu chồng tốt (thử 'Nguyễn Thị Hường – ỄỮẪ')." |
| "Số to mà chẳng để làm gì" | "Cỡ **display** chỉ dành cho con số trả lời câu hỏi chính của màn. Số đếm tổng (sĩ số, số buổi) thu về **một dòng meta** 13px." |
| "Nhấn mạnh kiểu gì" | "Gạch chân **chỉ cho link**. Nghiêng chỉ để nhấn trong câu. In hoa chỉ cho nhãn 1–2 từ, kèm letter-spacing +0.05em." |

## V-03 · Màu
| Bạn cảm thấy | Câu lệnh cho AI |
|---|---|
| "Đơn điệu, toàn trắng với xám" | "Thêm **tầng phụ** khoảng 20% diện tích bằng **một mặt phẳng nền** (accent-soft) gom [nhóm việc chính] để tạo **figure–ground**. Không tô màu từng thẻ để trang trí, không thêm hue mới." |
| "Màu rối, cam ở khắp nơi" | "Kiểm phân bổ **70-20-10 theo diện tích**. Màu nhấn tối đa ~10% và chỉ cho hành động chính; link, tab đang chọn, avatar, chấm trạng thái chuyển về **trung tính đậm** (tránh **accent dilution**)." |
| "Xám trông chết, lạnh" | "Dùng **neutral pha sắc** theo màu nhấn: trong **OKLCH** giữ hue [45], **chroma 0.005–0.015** cho nền, viền và chữ phụ. Không dùng xám thuần." |
| "Bảng màu tự chế lệch sáng tối" | "Sinh thang 50–900 bằng **OKLCH**: giữ hue, L giảm đều, chroma cao nhất ở giữa thang. Không sinh bằng HSL." |
| "Đỏ, vàng, xanh dùng lung tung" | "**Semantic color** (success / warning / danger / info) chỉ cho trạng thái thật, mỗi màu một cặp nền nhạt + chữ đậm, luôn kèm chữ hoặc icon (**color-not-alone**). Không dùng semantic để trang trí." |
| "Chữ trên nền màu khó đọc, xỉn" | "Chữ trên nền màu dùng **sắc độ cùng hue**, không dùng xám. Kiểm **contrast ratio**: chữ thường ≥ 4.5:1, chữ lớn và viền control ≥ 3:1." |

## V-04 · Khoảng cách, lưới, nhịp
| Bạn cảm thấy | Câu lệnh cho AI |
|---|---|
| "Đều đều, không thấy nhóm" | "Dùng **proximity** để nhóm: khoảng trong nhóm 8, giữa nhóm 24, giữa section 32–48 (mỗi bậc **≥ 2×** bậc dưới). Nhóm bằng khoảng trắng trước khi thêm viền hay nền." |
| "Khoảng cách lộn xộn" | "Chỉ dùng **spacing scale** 4/8: 4, 8, 12, 16, 24, 32, 48. Không dùng giá trị ngoài thang. Dùng **gap** của flex/grid thay cho margin trên từng phần tử." |
| "Chật, ngột" | "Lề màn 16, **padding** thẻ 16 (lớn hơn khoảng bên trong thẻ). Tăng **whitespace macro** giữa section trước khi thu nhỏ chữ." |
| "Nhàm, khối nào cũng như nhau" | "Tạo **rhythm**: lặp cấu trúc nhưng có biến tấu. Khối quan trọng nhất có khoảng thở lớn; danh sách thì dày. Nhất quán (cùng thang) ≠ đồng phục (cùng một giá trị)." |
| "Trông lệch lệch" | "Căn theo **lưới 4 cột, margin 16, gutter 16** cho màn 360dp. Mọi mép trái nằm trên cùng một đường; nút đôi mỗi nút đúng 2 cột." |
| "Danh sách dài, cuộn mãi" | "Chọn **density** theo việc: danh sách làm việc dùng compact, hàng 48 một dòng; màn đọc lướt 56–64. Vùng chạm không dưới 48. Danh sách dùng đường kẻ, không bọc mỗi hàng một thẻ." |

