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

## V-05 · Chiều sâu & hình khối
| Bạn cảm thấy | Câu lệnh cho AI |
|---|---|
| "Cái gì cũng nổi, nặng nề" | "Chỉ phần tử bấm được mới có bóng hoặc gờ (**signifier**). Thẻ thông tin phẳng, tách bằng khoảng trắng hoặc nền muted. Nút chính là thứ nổi rõ nhất màn." |
| "Bóng trông bẩn, cũ" | "Dùng **bóng hai lớp** nhạt (một lớp gần sắc, một lớp xa mờ, alpha 0.06–0.16) theo thang **elevation** 0–4. Không dùng một lớp đen đậm." |
| "Thẻ rối, nhiều đường viền" | "Mỗi khối chỉ **một tín hiệu** tách nền: khoảng trắng, hoặc nền, hoặc viền 1px, hoặc bóng. Không chồng viền + nền + bóng." |
| "Bo góc trông lệch" | "Bo lồng nhau **đồng tâm**: bo trong = bo ngoài − padding. Thang bo ba bậc cách xa + pill: nút 8, thẻ 12, sheet 20, chip pill." |
| "Dark mode phẳng lì" | "Trong dark mode bỏ bóng; thể hiện elevation bằng **surface tint** (nền sáng dần theo độ cao), vd #161412 → #24201D → #332E2A." |
| "Muốn vui như app học" | "Nút **gờ dày** chỉ dùng khi cả hệ cùng giọng: chữ to đậm, màu bão hoà, minh hoạ, chuyển động nảy. Nếu không, giữ phẳng và chỉ nút chính có gờ 2–4px." |


## V-06 · Bố cục màn mobile
| Bạn cảm thấy | Câu lệnh cho AI |
|---|---|
| "Màn mở ra toàn số liệu, không biết bấm gì" | "Bắt đầu màn từ **hành động chính**, không từ dữ liệu: hành động chính nằm trong **viewport đầu tiên** (above the fold) ở màn cao 640dp, cỡ chữ 115%. Số liệu không dẫn tới quyết định thì gom thành một dòng phụ ở cuối." |
| "Nút chính khó bấm khi cầm một tay" | "Đặt hành động chính trong **thumb zone**: nút rộng hết màn, dính đáy trong **bottom bar**. **Top app bar** chỉ chứa tiêu đề, nút quay lại và hành động phụ." |
| "Không biết màn này nên trông thế nào" | "Trước khi vẽ, viết một câu: người dùng mở màn này để làm gì. Rồi chọn **pattern** khớp câu đó (list, detail, overview, form, master–detail) và nói rõ vì sao chọn." |
| "Danh sách đọc mệt, toàn chữ" | "Mỗi hàng của **list** đưa từ khoá lên đầu dòng (tên in đậm) và trạng thái thành nhãn ở cuối dòng, để mắt không phải quét theo **F-pattern** qua cả câu dài." |
| "Form dài, nản" | "Gom các ô liên quan thành nhóm có tiêu đề; nếu quá 6–7 ô thì chia thành **multi-step form** có chỉ báo bước. Nút gửi luôn thấy trong bottom bar." |
| "Hai tab trông na ná nhau" | "Viết câu hỏi mà mỗi tab trả lời; nếu bố cục của tab này trả lời câu hỏi của tab khác thì bỏ phần trùng. **Mỗi tab một câu hỏi** (information architecture)." |

## V-07 · Nút & điều khiển đúng nghĩa
| Bạn cảm thấy | Câu lệnh cho AI |
|---|---|
| "Nhiều nút quá, không biết bấm cái nào" | "Áp **button hierarchy**: mỗi màn đúng một **primary** (đặc màu); việc thay thế là **secondary** (viền); thoát hoặc xem thêm là **tertiary** (chỉ chữ). Không đặt hai nút đặc màu cạnh nhau." |
| "Nút ghi OK, Xác nhận chung chung" | "Nhãn nút là **động từ cộng đối tượng**, nói đúng điều sẽ xảy ra ("Chốt điểm danh", "Gửi yêu cầu"). Nút huỷ ghi "Quay lại", không dùng cặp Có/Không." |
| "Dùng công tắc lung tung" | "Chọn control theo ý nghĩa: **switch** chỉ cho cài đặt có hiệu lực ngay, không cần nút Lưu; đánh dấu nhiều mục rồi xác nhận dùng **checkbox**; chọn một trong vài lựa chọn dùng **radio** hoặc **segmented control**." |
| "Hàng chip lẫn lộn" | "Hai nhóm khác nghĩa phải khác hình: chọn một dùng **segmented control**; bật tắt bộ lọc dùng **filter chip** có dấu ✓ khi bật. Mỗi nhóm có nhãn nhỏ và cách nhau một khoảng." |
| "Icon khó hiểu" | "Chỉ dùng **icon button** không nhãn cho icon quy ước (quay lại, đóng, tìm kiếm, thêm). Hành động riêng của app thì icon kèm nhãn chữ. Không dựa vào **tooltip**. Vùng chạm tối thiểu 48dp." |
| "Sợ bấm nhầm xoá" | "Nút **destructive** dạng chữ hoặc viền đỏ, đặt xa primary và ngoài vùng ngón cái, kèm hộp xác nhận ghi rõ hậu quả hoặc snackbar có nút **Hoàn tác (undo)**." |

## V-08 · Điều hướng & kiến trúc thông tin
| Bạn cảm thấy | Câu lệnh cho AI |
|---|---|
| "Vào sâu một chút là không biết mình đang ở đâu" | "Mỗi màn có **top app bar** ghi tên mục đang xem (vd "Lê Thu Trang", không ghi "Chi tiết"); tab của khu hiện tại luôn được tô trên **navigation bar**; mọi màn con có nút ‹ ở góc trên trái." |
| "Menu bị giấu hết, phải mở mới thấy" | "Dùng **navigation bar** cố định 3–5 tab cho các khu chính, mỗi tab trả lời một câu hỏi, nhãn 1–2 từ. Không giấu khu chính trong **navigation drawer** (menu ☰); drawer chỉ cho mục ít dùng." |
| "Bấm quay lại bị nhảy lung tung" | "Nút ‹ luôn về **màn cha** theo hierarchy, giữ vị trí cuộn. Mỗi tab giữ **back stack** riêng: đổi tab rồi quay lại thì về đúng màn đang xem; bấm lại tab đang mở thì về màn gốc của tab." |
| "Mở từ thông báo, bấm quay lại là thoát app" | "**Deep link** vào màn sâu phải dựng sẵn back stack đầy đủ (vd Lớp, SE1801, Lê Thu Trang) và chọn đúng tab, để nút ‹ đi lên từng bậc." |
| "Thanh tab dưới chật, chữ bị cắt" | "Navigation bar tối đa 5 mục, nhãn không bị cắt. Quá 5 khu thì gộp khu ít dùng vào Tài khoản hoặc đưa vào drawer. Không để thanh tab đổi nội dung theo từng màn." |
| "Tab chồng tab, lạc" | "Tab dưới chỉ cho các khu ngang hàng; các góc nhìn của cùng một nội dung (Hôm nay / Tuần) dùng **top tabs** hoặc segmented trong màn đó. Mỗi màn tối đa một tầng tab." |

## V-09 · Trạng thái & phản hồi
| Bạn cảm thấy | Câu lệnh cho AI |
|---|---|
| "Mở màn ra trắng trơn một lúc" | "Vẽ **loading state** bằng **skeleton** đúng hình nội dung (thẻ, dòng, ô số), không dùng màn trắng hay spinner giữa màn cho màn có bố cục cố định. Dữ liệu về thì đổ vào đúng chỗ, không khối nào đổi vị trí." |
| "Bấm nút không biết đã ăn chưa" | "Mọi nút đổi trạng thái trong **0,1 giây** khi chạm. Chờ quá **1 giây** thì nút thành "Đang [động từ]…" có spinner nhỏ và bị khoá để không gửi trùng. Quá **10 giây** thì báo tiến độ và cho rời màn." |
| "Màn trống trông như lỗi" | "Mỗi danh sách có **empty state** riêng: lần đầu thì một câu giải thích màn này để làm gì và nút cho bước đầu tiên; đã xử lý hết thì báo là xong. Không dùng "Không có dữ liệu"." |
| "Báo lỗi khó hiểu" | "Mọi **error state** trả lời ba câu bằng lời người dùng: hỏng gì, dữ liệu vừa nhập còn không, bấm gì để sửa (Thử lại, Để sau). Không hiện mã lỗi hay "Đã có lỗi xảy ra"." |
| "Mất mạng là mất hết" | "Khi **offline**, giữ dữ liệu đã tải và hiện một dải báo có giờ cập nhật cuối, không thay cả màn bằng màn lỗi. Thao tác cần mạng thì lưu vào hàng chờ trên máy và tự gửi khi có mạng." |
| "Hỏi Bạn có chắc hoài, phiền" | "Thao tác đảo được thì làm luôn và hiện **snackbar** có nút **Hoàn tác (undo)** trong khoảng 5 giây. Chỉ dùng hộp xác nhận cho thao tác không đảo được, ghi rõ hậu quả và nút có nhãn động từ." |

## V-10 · Định luật UX bằng hình
| Bạn cảm thấy | Câu lệnh cho AI |
|---|---|
| "Nút chính khó bấm, hay trượt" | "Áp **Fitts's law**: hành động chính rộng hết màn, cao 48–56dp, đặt ở vùng ngón cái (đáy màn). Hành động phụ có thể nhỏ hơn nhưng vùng chạm không dưới 48dp." |
| "Danh sách dài, tìm mãi" | "Áp **Hick's law** đúng cách: không cắt bớt mục mà sắp xếp theo việc của người dùng. Đưa mục liên quan tới hôm nay lên đầu thành nhóm riêng, phần còn lại sắp theo mã hoặc chữ cái." |
| "Mã dài khó đọc khó gõ" | "Hiển thị mã, số và ID theo **chunking**: chia thành nhóm 3–4 ký tự có khoảng cách (vd "4829 1736"), font monospace, chữ to. Ô nhập mã cũng tự chèn khoảng cách theo nhóm." |
| "AI bảo menu tối đa 7 mục" | "Không áp luật **Miller** cho menu đang hiển thị: người dùng nhận ra mục chứ không phải nhớ. Giữ đủ mục cần thiết, chia thành nhóm có tiêu đề, mục hay dùng ở đầu." |
| "Xong việc mà không thấy gì" | "Áp **peak-end rule**: mỗi luồng chính có màn kết thúc rõ ràng (kết quả cụ thể, vd "34 có mặt, 1 vắng", kèm Hoàn tác). Tìm bước gây khó chịu nhất của luồng và sửa nó trước khi trau chuốt các bước khác." |
| "Thử với người dùng ai cũng khen" | "Nhớ **aesthetic-usability effect**: thử luồng bằng bản wireframe xám trước để người dùng báo lỗi thật, sau đó mới thử bản đẹp. Ghi lại lỗi thao tác, không chỉ lời khen." |
