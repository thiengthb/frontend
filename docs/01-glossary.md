# 01 — Thuật ngữ UI/UX (glossary sống)

> Mỗi thuật ngữ gồm: **tên tiếng Anh**, nghĩa ngắn, *vì sao quan trọng*. Khi học bài mới thì bổ sung vào đây.
> Đánh dấu ✅ khi bạn đã học kỹ thuật ngữ đó qua một bài học.

## A. Nền tảng thị giác (Visual design)
| Thuật ngữ | Nghĩa | Vì sao quan trọng |
|---|---|---|
| **Visual hierarchy** ✅ | Thứ tự mắt người đọc lướt qua các phần tử | Quyết định người dùng thấy gì trước, hiểu gì trước |
| **De-emphasize** ✅ | Hạ cấp: làm phần phụ nhỏ hơn, nhạt hơn, nhẹ hơn để phần chính nổi | Cách rẻ nhất để tạo điểm nhấn, không cần phóng to (V-01) |
| **Consistency ≠ uniformity** ✅ | Nhất quán = cùng một thang; đồng phục = chỉ dùng một bậc của thang | Đồng phục xoá tương phản, sinh ra "đơn điệu" (V-01, W2) |
| **Concentric radius** ✅ | Bo góc lồng nhau đồng tâm: bán kính trong = ngoài − padding | Sai thì khe góc phình, trông rẻ (VIS-005, V-01) |
| **Contrast** | Sự khác biệt (kích thước, màu, độ đậm, khoảng cách, hình dạng) | Không có tương phản thì không có phân cấp, dẫn đến "đơn điệu" |
| **Emphasis / Focal point** ✅ | Điểm nhấn, nơi mắt dừng lại đầu tiên | Mỗi màn hình nên có một điểm nhấn chính |
| **Balance** | Cân bằng thị giác (đối xứng hoặc bất đối xứng) | Tạo cảm giác ổn định hoặc động |
| **Rhythm / Repetition** ✅ | Lặp lại có chủ đích (spacing, kiểu section) | Lặp có biến tấu; lặp y hệt thì đều đều (V-04) |
| **Proximity** ✅ | Phần tử gần nhau được xem là một nhóm | Mạnh hơn khung viền. Giữa nhóm ≥ 2× trong nhóm (V-04) |
| **Alignment** ✅ | Căn theo trục chung | Mép lệch 3–10px cộng lại thành "luộm thuộm" (V-04) |
| **White space / Negative space** | Khoảng trống | Không phải là phí chỗ: nó tách nhóm, tạo nhịp, tạo cảm giác cao cấp |
| **Gestalt principles** | Các nguyên lý tri giác: proximity, similarity, closure, continuity, figure–ground, common region | Giải thích *vì sao* mắt người nhóm và hiểu các hình |
| **Affordance / Signifier** ✅ | Affordance: khả năng thật (bấm được). Signifier: dấu hiệu báo khả năng đó (bóng, gờ, mũi tên ›) | Signifier không có affordance = nói dối (V-05) |
| **Elevation** ✅ | Độ cao giả lập trên trục z, thang 0–4 | Nền sáng: bóng; nền tối: nền sáng dần (V-05) |
| **Shadow (hai lớp)** ✅ | Một lớp gần sắc + một lớp xa mờ, alpha thấp | Bóng một lớp đen đậm trông bẩn, cũ (V-05) |
| **Ledge (gờ đáy)** ✅ | Dải đặc dưới đáy khối, giả nút vật lý | Tín hiệu bấm mạnh nhất; chỉ cho nút chính (V-05) |
| **Surface tint** ✅ | Dark mode: vật càng cao nền càng sáng | Thay cho bóng, vì bóng vô hình trên nền tối (V-05) |

## B. Typography
| Thuật ngữ | Nghĩa | Vì sao quan trọng |
|---|---|---|
| **Typeface vs Font** | Họ chữ (Inter) và một biến thể cụ thể (Inter Bold 16px) | Dùng đúng từ khi ra đề cho AI |
| **Serif / Sans-serif / Mono / Display** | Các nhóm chữ | Mỗi nhóm mang một "giọng" khác nhau |
| **Type scale** ✅ | Thang cỡ chữ theo tỉ lệ (vd 1.25 – Major Third) | Đảm bảo nhất quán, tránh 13px, 15px, 17px lộn xộn |
| **Weight** ✅ | Độ đậm (100–900) | Là công cụ phân cấp thứ hai sau cỡ chữ |
| **Line-height (leading)** ✅ | Khoảng cách dòng | Ảnh hưởng trực tiếp đến độ dễ đọc |
| **Letter-spacing (tracking)** | Khoảng cách chữ | Chữ in hoa và chữ lớn thường cần chỉnh |
| **Measure / Line length** ✅ | Độ dài dòng (~45–75 ký tự) | Dòng quá dài khiến mắt mỏi và lạc dòng |
| **Modular scale** ✅ | Thang tỉ lệ: cỡ gốc nhân liên tục với một tỉ lệ (1.2 / 1.25 / 1.333 / 1.5) | Ít bậc, cách xa; được bỏ bậc để tạo khoảng nhảy (V-02) |
| **Tabular figures** ✅ | Chữ số đều bề rộng (`font-variant-numeric: tabular-nums`) | Cột số, giờ, x/4 thẳng hàng, so nhanh (V-02) |
| **Dấu chồng (stacked diacritics)** ✅ | Hai dấu trên một chữ tiếng Việt (ễ, ữ, ẫ) | Cần line-height ≥ 1.4 cho đoạn; chọn font vẽ dấu tốt (V-02) |
| **Font pairing** | Ghép 2 font | Nên tương phản rõ hoặc cùng một họ, tránh "gần giống nhau" |
| **Italic / Underline / Bold** ✅ | Nhấn mạnh | Mỗi kiểu có vai trò riêng; underline trên web thường được hiểu là **link** |

## C. Màu sắc (Color)
| Thuật ngữ | Nghĩa | Vì sao quan trọng |
|---|---|---|
| **Hue / Saturation / Lightness** ✅ | Sắc / độ bão hoà / độ sáng (HSL, OKLCH) | Hiểu ba trục này thì tự tạo được bảng màu (V-03) |
| **OKLCH** ✅ | Ghi màu bằng L (độ sáng theo mắt) · C (độ rực) · H (góc hue). CSS: `oklch(0.57 0.14 45)` | Cùng L là cùng độ sáng thật; thang màu đều hơn HSL (V-03) |
| **Chroma** ✅ | Độ rực trong OKLCH: 0 là xám | Neutral pha sắc dùng chroma 0.005–0.015 (V-03) |
| **Palette / Shades (50–900)** | Dải sắc độ của một màu | Các design system đều dùng thang này |
| **Semantic color** ✅ | Màu theo ý nghĩa: success, warning, danger, info | Chỉ cho trạng thái; dùng để trang trí thì mất giá (V-03) |
| **Neutral** ✅ | Xám (thường pha chút màu chủ đạo) | Chiếm phần lớn diện tích giao diện; xám thuần trông vô chủ (V-03) |
| **Accent dilution** ✅ | Màu nhấn rải ra nhiều vai (link, avatar, tab, nút) | Cam ở 6 chỗ thì cam hết nghĩa "hành động" (V-03) |
| **60-30-10 / 70-20-10** ✅ | Tỉ lệ diện tích nền / phụ / nhấn | Tính theo diện tích; tầng phụ là mặt phẳng tổ chức; 10% là trần (V-03) |
| **Contrast ratio (WCAG)** ✅ | Tỉ lệ tương phản chữ/nền: 4.5:1 cho chữ thường, 3:1 cho chữ lớn và viền control | Là chuẩn trợ năng, mức bắt buộc (V-03, sâu ở V-11) |
| **Color-not-alone** ✅ | Không truyền thông tin chỉ bằng màu: kèm chữ hoặc icon | ~8% nam giới lẫn đỏ–lục (V-03) |
| **Color harmony** | Bổ sung, tương đồng, bộ ba… | Giúp chọn màu phụ/nhấn có cơ sở |

## D. Bố cục (Layout & Spacing)
| Thuật ngữ | Nghĩa | Vì sao quan trọng |
|---|---|---|
| **Grid system** ✅ | Lưới cột (mobile 4 cột, desktop 12), gutter, margin | Giữ ít đường căn; mobile: margin 16, gutter 16 (V-04) |
| **Gutter / Margin** ✅ | Gutter: khe giữa cột. Margin: lề hai bên màn | Lề 16 tránh chữ sát mép máy (V-04) |
| **8pt grid / Spacing scale** ✅ | Thang spacing 4/8/12/16/24/32/48 | Chỉ chọn trong thang; bậc cách xa nhau (V-04) |
| **Whitespace (micro / macro)** ✅ | Khoảng trống trong khối (chữ, nút) / giữa khối, section | Macro tạo nhóm và nhịp (V-04) |
| **Padding vs gap** ✅ | Padding: mép hộp → nội dung. Gap: giữa các phần tử anh em | Padding thẻ ≥ gap bên trong thẻ (V-04) |
| **F-pattern / Z-pattern** ✅ | Hình đường mắt khi lướt: chữ F trên màn nhiều chữ đều nhau, chữ Z trên màn ít chữ | F là triệu chứng của nội dung thiếu điểm bám (NN/g), không phải mục tiêu; Z là kinh nghiệm, ít bằng chứng hơn (V-06) |
| **Above the fold (viewport đầu tiên)** ✅ | Phần thấy được ngay khi mở màn, chưa cuộn | Hành động chính phải nằm ở đây, kể cả ở màn 640dp, cỡ chữ 115% (UX-001, V-06) |
| **List / Detail** ✅ | List: nhiều mục cùng loại để quét và chọn. Detail: mọi thứ về một mục đã chọn | Cặp pattern cơ bản nhất của app; detail nên là một cột cuộn (V-06) |
| **Overview** ✅ | Màn trả lời "bây giờ cần làm gì, có gì bất thường" | Hay bị biến thành dashboard lưới số liệu (W3, V-06) |
| **Master–detail** ✅ | List bên trái, detail bên phải trên cùng một màn rộng | Hợp tablet và máy tính; trên điện thoại tách thành list rồi detail (V-06) |
| **Thumb zone (vùng ngón cái)** ✅ | Phần màn ngón cái tới dễ khi cầm máy một tay, chủ yếu nửa dưới | Nút chính đặt ở đáy; mô hình gần đúng từ quan sát của Steven Hoober (V-06) |
| **Top app bar / Bottom bar** ✅ | Thanh trên: tiêu đề, quay lại, hành động phụ. Thanh dưới: nút hành động chính hoặc thanh tab | Top bar ở vùng khó với, không đặt nút chính (V-06) |
| **Multi-step form** | Form chia thành vài bước ngắn có chỉ báo bước | Bớt nản với form dài; nút tiếp tục luôn thấy (V-06) |
| **Responsive / Breakpoint** | Thích ứng theo kích thước màn hình | Mobile chiếm phần lớn lượng truy cập |
| **Container / Max-width** | Giới hạn chiều rộng nội dung | Giữ độ dài dòng hợp lý |
| **Density** ✅ | Mật độ thông tin: compact / comfortable / spacious | Chọn theo việc; vùng chạm luôn ≥ 48 (V-04) |

## E. Nguyên lý & định luật UX
| Thuật ngữ | Nghĩa ngắn |
|---|---|
| **Nielsen's 10 Heuristics** | 10 nguyên tắc đánh giá khả dụng (trạng thái hệ thống, kiểm soát, nhất quán, ngăn lỗi…) |
| **Fitts's Law** ✅ | Mục tiêu càng to và càng gần thì chạm càng nhanh; độ khó = log₂(1 + khoảng cách ÷ bề rộng). Fitts 1954 (V-10) |
| **Hick's Law** ✅ | Nhiều lựa chọn ngang nhau thì chọn chậm, nhưng tăng chậm dần (log). Sắp xếp theo việc của người dùng làm nó yếu đi. Hick 1952, Hyman 1953 (V-10) |
| **Jakob's Law** ✅ | Người dùng mong web của bạn hoạt động giống các web họ đã quen. Dẫn đến tôn trọng quy ước |
| **Miller's Law / Chunking** ✅ | Trí nhớ ngắn hạn giữ ít (Miller 1956: ~7; Cowan 2001: ~4 nhóm); gom nhóm để giữ nhiều hơn. ⚠️ Không phải "menu tối đa 7 mục" (V-10) |
| **Tesler's Law** | Độ phức tạp không biến mất, chỉ chuyển từ người dùng sang hệ thống |
| **Doherty Threshold** | Phản hồi dưới ~400ms giữ được dòng tương tác |
| **Peak-End Rule** ✅ | Người dùng nhớ lúc tệ (hay) nhất và lúc kết thúc, ít nhớ độ dài. Kahneman 1993, thí nghiệm nước lạnh (V-10) |
| **Von Restorff Effect** ✅ | Thứ khác biệt sẽ được nhớ. Đây là cơ sở của màu nhấn |
| **Aesthetic-Usability Effect** ✅ | Thứ đẹp được chấm là dễ dùng hơn (Kurosu & Kashimura 1995, ATM). ⚠️ Che lỗi khi thử bản mẫu đẹp: thử luồng bằng wireframe trước (V-10) |
| **Serial position effect** ✅ | Mục đầu và cuối danh sách dễ nhớ hơn mục giữa (V-10) |
| **Cognitive load** | Tải nhận thức, tức người dùng phải nghĩ bao nhiêu |
| **Progressive disclosure** | Hé lộ dần, chỉ cho thấy cái cần lúc cần |
| **Mental model** | Hình dung của người dùng về cách hệ thống hoạt động |

## F. Quy trình & cấu trúc
| Thuật ngữ | Nghĩa ngắn |
|---|---|
| **User persona / JTBD** | Chân dung người dùng / công việc họ cần hoàn thành |
| **User flow / Journey map** | Luồng các bước / hành trình cảm xúc |
| **Information Architecture (IA)** ✅ | Cách chia nội dung app thành các khu, các tầng và đặt tên. Mỗi tab trả lời một câu hỏi (UX-002, V-08) |
| **Wireframe → Mockup → Prototype** | Khung xương → hình ảnh hoàn chỉnh → bản tương tác được |
| **Design system** | Token, component, pattern và nguyên tắc dùng chung |
| **Design tokens** | Biến thiết kế (màu, spacing, radius…) dạng dữ liệu |
| **Atomic design** | Atoms → molecules → organisms → templates → pages (Brad Frost) |
| **UI pattern** | Lời giải đã được chứng minh cho vấn đề lặp lại (modal, tabs, empty state…) |
| **Usability testing** | Quan sát người thật dùng sản phẩm |
| **Design critique** | Phê bình có cấu trúc: mục tiêu → quan sát → tác động → đề xuất |

## G. Component & tương tác
| Thuật ngữ | Nghĩa ngắn |
|---|---|
| **Component states** | default, hover, focus, active, disabled, loading, error, empty |
| **Primary / Secondary / Tertiary button** ✅ | Phân cấp nút: đặc màu (việc chính, một nút mỗi màn) / viền (việc thay thế) / chỉ chữ (thoát, xem thêm). Thử nheo mắt: chỉ nút chính còn rõ (V-07) |
| **Destructive button** ✅ | Nút xoá hoặc làm mất dữ liệu: chữ hoặc viền đỏ, tách xa nút chính, kèm xác nhận hoặc undo (V-07) |
| **Checkbox / Radio / Switch** ✅ | Chọn nhiều rồi xác nhận / chọn một trong vài lựa chọn đang hiện / bật tắt cài đặt có hiệu lực ngay, không cần nút Lưu (CMP-001, V-07) |
| **Segmented control** ✅ | Thanh 2–4 ô, chọn một chế độ xem, nội dung đổi ngay (V-07) |
| **Chip (filter / choice)** ✅ | Viên nhãn bấm được; filter chip bật tắt bộ lọc, có ✓ khi bật. Chip khác nghĩa không được trông giống nhau (V-07) |
| **Icon button** ✅ | Nút chỉ có hình; chỉ ổn với icon quy ước (‹, ✕, tìm kiếm). Tooltip không có trên điện thoại (V-07) |
| **Button label (động từ + đối tượng)** ✅ | "Chốt điểm danh" thay cho "OK"; đọc riêng nút vẫn hiểu (V-07) |
| **Navigation bar (thanh tab dưới)** ✅ | 3–5 tab cố định ở đáy, mỗi tab một khu chính ngang hàng (quy ước Material). Không đổi theo màn (V-08) |
| **Top tabs (tab trên)** ✅ | Hàng tab gạch chân dưới tiêu đề, đổi góc nhìn của cùng một nội dung (Hôm nay / Tuần). Không đưa góc nhìn lên tab dưới (V-08) |
| **Back stack (ngăn xếp màn)** ✅ | Chồng các màn đã đi qua; chạm mục thì chồng thêm, ‹ thì rút ra. Mỗi tab giữ ngăn xếp riêng (V-08) |
| **Up / Back (‹ và quay lại hệ thống)** ✅ | ‹ luôn lên màn cha theo quan hệ cha–con; nút hệ thống còn bấm được ở màn gốc (V-08) |
| **Hierarchy (cha–con)** ✅ | Màn nằm bên trong màn khác: Lớp > SE1801 > Lê Thu Trang. Đi dọc = xuống con / lên cha; đi ngang = đổi khu (V-08) |
| **Breadcrumb** ✅ | Đường dẫn "Lớp › SE1801 › Lê Thu Trang", mỗi bậc là link. Hay dùng trên web; mobile thay bằng tiêu đề + ‹ (V-08) |
| **Navigation drawer (menu ☰)** ✅ | Danh sách khu giấu sau nút ☰. Chỉ cho mục ít dùng hoặc app > 5 khu; giấu khu chính là tệ (V-08) |
| **Deep link** ✅ | Mở thẳng màn sâu (vd từ thông báo); phải dựng sẵn back stack để ‹ đi lên từng bậc (V-08) |
| **CTA (Call to action)** | Hành động chính mà ta muốn người dùng làm |
| **State (trạng thái màn)** ✅ | Một khuôn mặt của màn theo tình huống; lab2 dùng mã .D .D1 .L .E .E2 .X .S. Mọi trạng thái giữ cùng bố cục với .D (V-09) |
| **Loading: spinner / skeleton** ✅ | Vòng xoay chỉ nói "đang làm"; khung xám đúng hình nội dung giữ chỗ, bố cục không nhảy. Màn bố cục cố định dùng skeleton; chờ trong nút dùng spinner nhỏ (V-09) |
| **Empty state** ✅ | Màn không có dữ liệu: lần đầu thì dạy và có nút bước đầu; xử lý hết thì báo là xong. Không dùng "Không có dữ liệu" (V-09) |
| **Error state** ✅ | Lỗi trả lời ba câu: hỏng gì, dữ liệu còn không, bấm gì để sửa (V-09) |
| **Offline** ✅ | Mất mạng: giữ dữ liệu đã tải + dải báo có giờ cập nhật; thao tác cần mạng vào hàng chờ, tự gửi lại (V-09) |
| **Toast / Snackbar** ✅ | Toast: dòng báo tự tắt, không nút. Snackbar: dòng báo ở đáy có một nút, thường là Hoàn tác (V-09) |
| **Undo (hoàn tác)** ✅ | Rút lại thao tác vừa làm; thay được hộp "Bạn có chắc?" cho thao tác đảo được (V-09) |
| **Optimistic UI** ✅ | Hiện kết quả ngay như đã xong, gửi máy chủ sau; hỏng thì báo và trả lại (V-09) |
| **Response time limits (0,1 / 1 / 10 giây)** ✅ | Tức thì / còn theo mạch / hết kiên nhẫn (Miller 1968, Nielsen). Heuristic, không phải chuẩn (V-09) |
| **Microcopy / UX writing** | Chữ nhỏ trên nút, lỗi, gợi ý |
| **Microinteraction / Motion** | Phản hồi nhỏ khi thao tác, chuyển động có mục đích |
| **Easing / Duration** | Đường cong và thời lượng chuyển động (thường 150–300ms) |
| **Accessibility (a11y)** ✅ | Trợ năng: bàn phím, screen reader, tương phản, focus ring |

## H. Animation & motion (M9)
| Thuật ngữ | Nghĩa ngắn |
|---|---|
| **Duration / Timing** ✅ | Thời lượng chuyển động. Token Material 3: short 50–200ms, medium 250–400ms, long 450–600ms, extra long 700–1000ms (quy ước). Phản hồi nhỏ ~100–150ms, hộp/sheet ~300–400ms, cả màn ≤ 500ms (V-12) |
| **Easing / cubic-bezier** ✅ | Đường cong tốc độ. ease-out để *vào* (nhanh rồi chậm), ease-in để *ra*, ease-in-out khi dời chỗ trên màn, linear chỉ cho spinner. Material: standard (0.2,0,0,1), emphasized decelerate (0.05,0.7,0.1,1), emphasized accelerate (0.3,0,0.8,0.15) (V-12) |
| **Spring (stiffness, damping, mass)** ✅ | Chuyển động theo mô hình lò xo vật lý, tự nhiên hơn tween khi bị ngắt giữa chừng |
| **Tween vs Spring** ✅ | Tween có thời lượng cố định; spring được quyết định bởi các tham số vật lý, giữ vận tốc khi bị ngắt. Dùng spring cho thứ người dùng điều khiển hoặc có thể ngắt (V-13) |
| **12 principles of animation** ✅ | 12 nguyên lý hoạt hình Disney: squash & stretch, anticipation, staging, follow-through, slow in/out, arc, timing… |
| **Choreography / Stagger** ✅ | Biên đạo nhiều phần tử: thứ tự, độ trễ lệch nhau |
| **Shared element / Layout animation** | Một phần tử "bay" từ vị trí cũ sang vị trí mới, giữ liên tục về không gian |
| **View Transitions API** | API trình duyệt cho chuyển cảnh giữa hai trạng thái DOM hoặc giữa hai trang |
| **FLIP** | First–Last–Invert–Play: kỹ thuật animate thay đổi layout bằng transform |
| **Microinteraction** ✅ | Trigger → rules → feedback → loops/modes (Dan Saffer) |
| **Reduced motion** ✅ | `prefers-reduced-motion`: người dùng nhạy cảm tiền đình; thay chuyển động bằng opacity, đừng tắt phản hồi |
| **Purpose of motion** ✅ | Năm mục đích: định hướng không gian, nối nhân và quả, hướng chú ý, cho thấy hệ thống đang làm, cá tính. Không có mục đích thì bỏ (V-12) |
| **Staging / anticipation / follow-through** ✅ | Dàn cảnh (mỗi lúc một thứ diễn) / lấy đà (lùi nhẹ trước khi đi) / đà còn lại (vượt nhẹ rồi về) (V-12) |
| **Fade through / shared axis** ✅ | Kiểu chuyển màn Material: mờ đi rồi hiện lại cho màn không liên quan (tab dưới) / trượt theo một trục cho màn có thứ tự (V-12) |
| **Damping ratio (tỉ lệ giảm chấn)** ✅ | damping / (2·√(stiffness·mass)). Dưới 1 thì nảy, từ 1 thì không. Giao diện thường 0,8–1; điểm nhấn vui ~0,5 (V-13) |
| **Spring mặc định của Motion** ✅ | stiffness 100, damping 10, mass 1 (tỉ lệ 0,5), đọc từ mã nguồn motion-dom 12; docs ghi stiffness 1 là sai (V-13) |
| **Compositor-only properties** ✅ | `transform`, `opacity`: animate mượt vì không gây layout hay paint lại |

## J. Phong cách thị giác & AI slop (V-14)
| Thuật ngữ | Nghĩa ngắn |
|---|---|
| **Skeuomorphism** ✅ | Giả vật liệu thật (da, gỗ, kim loại). Flat ra đời để phản ứng lại nó (V-14) |
| **Flat** ✅ | Màu đặc, không bóng, không vân. Windows Phone Metro (~2010), iOS 7 (2013). Phân cấp phải đến từ chữ, màu, khoảng trắng. Lab2 là flat thêm gờ đáy (V-14) |
| **Material** ✅ | Ngôn ngữ thiết kế của Google (2014), "giấy và mực": lớp cao hơn bóng rõ hơn; M3 thêm màu tonal. Quy ước của Android (V-14) |
| **Neumorphism** ✅ | Nút cùng màu nền, tách bằng bóng sáng và tối. Dribbble cuối 2019 (Oleksandr Plyuto), tên do Jason Kelley đặt, Michal Malewicz phổ biến. Hình nút ~1:1 với nền nên khó đạt trợ năng (V-14) |
| **Glassmorphism** ✅ | Lớp kính mờ nhìn xuyên thấy nền; tên phổ biến ~2020 (Malewicz), Windows 11 Acrylic/Mica, Apple Liquid Glass 2025. Chữ đổi độ rõ theo nền: đo ở vùng sáng nhất (V-14) |
| **Brutalism (web)** ✅ | Thô cố ý: viền đen dày, chữ đơn cách, không bo, bóng cứng (brutalistwebsites.com, ~2014–2016). Contrast cao nhưng hay phá quy ước (V-14) |
| **Bento grid** ✅ | Ô chữ nhật khác cỡ ghép khít; ô to cho thứ quan trọng. Mọi ô cùng cỡ thì thành lưới thẻ (V-14) |
| **AI slop** ✅ | Giao diện AI làm theo mặc định khi đề bài trống: gradient tím xanh, lưới 4 KPI, thẻ bo lớn có bóng mọi nơi, emoji làm icon, Inter mọi nơi, tiêu đề "Supercharge your…", căn giữa mọi thứ (V-14) |

## I. Thuật ngữ từ chẩn đoán M0-01
| Thuật ngữ | Nghĩa ngắn |
|---|---|
| **Vanity metric** ✅ | Số liệu đẹp nhưng không dẫn tới quyết định hay hành động |
| **Squint test** ✅ | Nheo mắt nhìn màn hình: cái gì còn nổi bật là điểm nhấn thật |
| **Recognition vs recall** | Nhận ra (thấy nhãn) dễ hơn nhớ lại (đoán icon) — Nielsen #6 |
| **Signifier** ✅ | Dấu hiệu cho biết có thể tương tác (Norman). Khác với affordance là khả năng thật (V-05) |
| **Figure–ground** ✅ | Tách hình khỏi nền. Tầng màu phụ 20% thường đóng vai trò "nền tổ chức" (V-03) |
| **WCAG 2.2 (A / AA / AAA)** ✅ | Chuẩn trợ năng web của W3C; AA là mức thường bị đòi | Là tầng "chuẩn", khác Material/HIG là "quy ước" (V-11) |
| **Relative luminance** ✅ | Độ sáng tương đối của một màu (0 đen, 1 trắng), kênh xanh lá nặng nhất | Contrast ratio = (L sáng + 0,05)/(L tối + 0,05) (V-11) |
| **Target size (vùng chạm)** ✅ | Vùng bấm được, có thể lớn hơn phần nút nhìn thấy | WCAG 2.5.8 AA 24px, 2.5.5 AAA 44px; Material 48dp (~9 mm), HIG 44pt (V-11) |
| **dp / pt / CSS px** ✅ | Đơn vị không phụ thuộc mật độ màn của Android / iOS / web | So sánh coi như gần bằng nhau (V-11) |
| **Focus ring** ✅ | Vòng hiện quanh mục đang chọn bằng bàn phím; dùng `:focus-visible` | WCAG 2.4.7 AA; xoá bằng `outline:none` là lỗi AI hay mắc (V-11) |
| **Screen reader và label** ✅ | Máy đọc màn hình (TalkBack, VoiceOver) chỉ đọc được nhãn bằng chữ: `aria-label`, `contentDescription` | Nút icon không nhãn chỉ được đọc là "Nút" (V-11) |
