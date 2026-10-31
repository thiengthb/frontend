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
| **Rhythm / Repetition** | Lặp lại có chủ đích (spacing, kiểu section) | Tạo nhất quán. Lặp mà không biến tấu thì sinh ra nhàm chán |
| **Proximity** | Phần tử gần nhau được xem là một nhóm | Là công cụ nhóm thông tin mạnh nhất, mạnh hơn cả khung viền |
| **Alignment** | Căn theo trục chung | Tạo trật tự, giúp giao diện trông "chuyên nghiệp" |
| **White space / Negative space** | Khoảng trống | Không phải là phí chỗ: nó tách nhóm, tạo nhịp, tạo cảm giác cao cấp |
| **Gestalt principles** | Các nguyên lý tri giác: proximity, similarity, closure, continuity, figure–ground, common region | Giải thích *vì sao* mắt người nhóm và hiểu các hình |
| **Affordance / Signifier** | Gợi ý cách dùng (nút trông như bấm được) | Người dùng không phải đoán |

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
| **Hue / Saturation / Lightness** | Sắc / độ bão hoà / độ sáng (HSL, OKLCH) | Hiểu ba trục này thì tự tạo được bảng màu |
| **Palette / Shades (50–900)** | Dải sắc độ của một màu | Các design system đều dùng thang này |
| **Semantic color** | Màu theo ý nghĩa: primary, success, warning, danger, info | Màu phải truyền đạt ý nghĩa, không chỉ để trang trí |
| **Neutral** | Xám (thường pha chút màu chủ đạo) | Chiếm phần lớn diện tích giao diện |
| **60-30-10 / 70-20-10** | Tỉ lệ diện tích nền / phụ / nhấn | Kiểm soát độ đơn điệu và độ rối |
| **Contrast ratio (WCAG)** | Tỉ lệ tương phản chữ/nền: 4.5:1 cho chữ thường, 3:1 cho chữ lớn | Là chuẩn trợ năng, mức bắt buộc |
| **Color harmony** | Bổ sung, tương đồng, bộ ba… | Giúp chọn màu phụ/nhấn có cơ sở |

## D. Bố cục (Layout & Spacing)
| Thuật ngữ | Nghĩa | Vì sao quan trọng |
|---|---|---|
| **Grid system** | Lưới cột (12 cột), gutter, margin | Là xương sống của bố cục |
| **8pt grid / Spacing scale** | Thang spacing 4/8/16/24/32/48/64 | Hai yếu tố quan trọng nhất cho sự nhất quán |
| **F-pattern / Z-pattern** | Kiểu mắt quét trang | Đặt nội dung quan trọng đúng vị trí mắt nhìn |
| **Above the fold** | Phần hiển thị trước khi cuộn | Ảnh hưởng đến ấn tượng đầu |
| **Responsive / Breakpoint** | Thích ứng theo kích thước màn hình | Mobile chiếm phần lớn lượng truy cập |
| **Container / Max-width** | Giới hạn chiều rộng nội dung | Giữ độ dài dòng hợp lý |
| **Density** | Mật độ thông tin (thoáng hay dày) | Dashboard khác landing page |

## E. Nguyên lý & định luật UX
| Thuật ngữ | Nghĩa ngắn |
|---|---|
| **Nielsen's 10 Heuristics** | 10 nguyên tắc đánh giá khả dụng (trạng thái hệ thống, kiểm soát, nhất quán, ngăn lỗi…) |
| **Fitts's Law** | Mục tiêu càng to và càng gần thì càng dễ bấm. Ảnh hưởng đến kích thước nút và vị trí CTA |
| **Hick's Law** | Càng nhiều lựa chọn thì quyết định càng chậm. Dẫn đến giảm hoặc nhóm lựa chọn |
| **Jakob's Law** | Người dùng mong web của bạn hoạt động giống các web họ đã quen. Dẫn đến tôn trọng quy ước |
| **Miller's Law** | Bộ nhớ ngắn hạn có giới hạn, nên chia nhỏ (chunking). ⚠️ Không phải "tối đa 7 mục" |
| **Tesler's Law** | Độ phức tạp không biến mất, chỉ chuyển từ người dùng sang hệ thống |
| **Doherty Threshold** | Phản hồi dưới ~400ms giữ được dòng tương tác |
| **Peak-End Rule** | Người dùng nhớ đỉnh cảm xúc và lúc kết thúc trải nghiệm |
| **Von Restorff Effect** ✅ | Thứ khác biệt sẽ được nhớ. Đây là cơ sở của màu nhấn |
| **Aesthetic-Usability Effect** | Thứ đẹp được cảm nhận là dễ dùng hơn. ⚠️ Có thể che giấu lỗi UX |
| **Cognitive load** | Tải nhận thức, tức người dùng phải nghĩ bao nhiêu |
| **Progressive disclosure** | Hé lộ dần, chỉ cho thấy cái cần lúc cần |
| **Mental model** | Hình dung của người dùng về cách hệ thống hoạt động |

## F. Quy trình & cấu trúc
| Thuật ngữ | Nghĩa ngắn |
|---|---|
| **User persona / JTBD** | Chân dung người dùng / công việc họ cần hoàn thành |
| **User flow / Journey map** | Luồng các bước / hành trình cảm xúc |
| **Information Architecture (IA)** | Tổ chức và đặt tên nội dung, điều hướng |
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
| **Primary / Secondary / Tertiary button** | Phân cấp nút theo mức quan trọng của hành động |
| **CTA (Call to action)** | Hành động chính mà ta muốn người dùng làm |
| **Empty state / Error state / Loading state** | Các trạng thái bị bỏ quên nhiều nhất, và là chỗ AI hay quên |
| **Microcopy / UX writing** | Chữ nhỏ trên nút, lỗi, gợi ý |
| **Microinteraction / Motion** | Phản hồi nhỏ khi thao tác, chuyển động có mục đích |
| **Easing / Duration** | Đường cong và thời lượng chuyển động (thường 150–300ms) |
| **Accessibility (a11y)** | Trợ năng: bàn phím, screen reader, tương phản, focus ring |

## H. Animation & motion (M9)
| Thuật ngữ | Nghĩa ngắn |
|---|---|
| **Duration / Timing** | Thời lượng chuyển động. Phản hồi nhỏ ~100–150ms, chuyển trạng thái ~200–300ms, chuyển cảnh ~300–500ms (heuristic) |
| **Easing / cubic-bezier** | Đường cong tốc độ. ease-out để *vào* (nhanh rồi chậm), ease-in để *ra* |
| **Spring (stiffness, damping, mass)** | Chuyển động theo mô hình lò xo vật lý, tự nhiên hơn tween khi bị ngắt giữa chừng |
| **Tween vs Spring** | Tween có thời lượng cố định; spring được quyết định bởi các tham số vật lý |
| **12 principles of animation** | 12 nguyên lý hoạt hình Disney: squash & stretch, anticipation, staging, follow-through, slow in/out, arc, timing… |
| **Choreography / Stagger** | Biên đạo nhiều phần tử: thứ tự, độ trễ lệch nhau |
| **Shared element / Layout animation** | Một phần tử "bay" từ vị trí cũ sang vị trí mới, giữ liên tục về không gian |
| **View Transitions API** | API trình duyệt cho chuyển cảnh giữa hai trạng thái DOM hoặc giữa hai trang |
| **FLIP** | First–Last–Invert–Play: kỹ thuật animate thay đổi layout bằng transform |
| **Microinteraction** | Trigger → rules → feedback → loops/modes (Dan Saffer) |
| **Reduced motion** | `prefers-reduced-motion`: người dùng nhạy cảm tiền đình; thay chuyển động bằng opacity, đừng tắt phản hồi |
| **Compositor-only properties** | `transform`, `opacity`: animate mượt vì không gây layout hay paint lại |

## I. Thuật ngữ từ chẩn đoán M0-01
| Thuật ngữ | Nghĩa ngắn |
|---|---|
| **Vanity metric** ✅ | Số liệu đẹp nhưng không dẫn tới quyết định hay hành động |
| **Squint test** ✅ | Nheo mắt nhìn màn hình: cái gì còn nổi bật là điểm nhấn thật |
| **Recognition vs recall** | Nhận ra (thấy nhãn) dễ hơn nhớ lại (đoán icon) — Nielsen #6 |
| **Signifier** | Dấu hiệu cho biết có thể tương tác (Norman). Khác với affordance là khả năng thật |
| **Figure–ground** | Tách hình khỏi nền. Tầng màu phụ 20% thường đóng vai trò "nền tổ chức" |
