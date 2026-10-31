# 05 — Crash course trực quan (Visual Crash Course, VCC)

> **v2 · 2026-10-31** (D-018). Thay bản v1 "Critique Loop" (CC-01..CC-13, người dùng làm bài và bị chấm).
> Người dùng làm rõ giai đoạn học hiện tại: **học để biết và nhận diện**, chưa phải học để tự giải quyết.
> Bản v1 nằm trong lịch sử git (commit trước 2026-10-31 21:00). CC-01 và nửa đầu CC-02 đã học theo v1; tài liệu của chúng được tái dùng làm ví dụ.

## 1. Người học đang ở đâu (thang Bloom)
| Tầng | Nghĩa | VCC nhắm tới? |
|---|---|---|
| Nhớ (remember) | Gọi tên được thuật ngữ, pattern | **Có** |
| Hiểu sơ (understand) | Nhìn ví dụ thì nhận ra cái tốt và cái tệ, biết đại khái vì sao | **Có** |
| Áp dụng | Tự sửa một màn | Chưa: để lab2 và deep track |
| Phân tích / đánh giá | Tự phê bình có cấu trúc | Chưa: Critique Loop (PRC-004) để dành cho sau |

**Mục tiêu đầu ra:** sau khoá, người dùng (1) nhìn một màn là gọi được tên vấn đề, (2) ra lệnh cho AI bằng đúng thuật ngữ, (3) biết phương án tốt nhất mặc định và các phương án tệ hay gặp.
**Rủi ro đã biết, chấp nhận có ý thức:** học thụ động tạo cảm giác "hiểu rồi" mạnh hơn mức hiểu thật (W10). Đổi lại là tốc độ. Bù bằng: lab2 sẽ là nơi áp dụng thật; mỗi trang có một phần "tự kiểm tra" tuỳ chọn, bấm là lộ đáp án, không chấm, không ghi điểm.

## 2. Định dạng một khối (V-xx)
Mỗi khối = **một artifact HTML tương tác** do Claude dựng trực tiếp (không còn subagent làm bài), đọc và nghịch trong khoảng 20–30 phút. Cấu trúc cố định để quét nhanh:

1. **Một câu cốt lõi** (big idea) ở đầu trang.
2. **Bản đồ nhanh**: 3–6 thuật ngữ của khối, mỗi cái một dòng.
3. **Cặp TỆ ↔ TỐT** (nhiều cặp): cùng nội dung, chỉ đổi một biến; có nút gạt / thanh trượt để tự thấy khác biệt. Mỗi cặp ghi tên lỗi bằng thuật ngữ.
4. **Phương án tốt nhất mặc định**: "nếu không biết chọn gì, làm thế này", kèm con số cụ thể.
5. **Các phương án tệ hay gặp** (nhất là mặc định của AI) và vì sao tệ.
6. **Trên lab2**: trước/sau trên màn thật của người dùng.
7. **Câu lệnh mẫu cho AI**: 3–5 câu copy được, dùng đúng thuật ngữ vừa học.
8. **Tự kiểm tra** (tuỳ chọn): 3 câu bấm lộ đáp án. Không ghi điểm.

Luật thiết kế của chính các trang này: dùng `artifact-design` skill; ví dụ minh hoạ dùng bảng màu lab2 (cam đất `#B9551F`, Nunito) để quen mắt; tiếng Việt có dấu đủ; chạy được trên điện thoại.

Đầu ra lưu repo mỗi khối: `demos/V-xx/*.html` (nguồn artifact), một mục trong `docs/06-ai-prompt-dictionary.md` (từ điển ra lệnh AI, cộng dồn), thuật ngữ mới vào `docs/01-glossary.md`, một dòng vào `log/PROGRESS.md`. **Không** viết luật mới trong `rules/` trong lúc học lướt, trừ khi người dùng muốn (luật cần hiểu sâu; đó là việc của lúc làm lab2).

## 3. Lịch học (15 khối, ~3 ngày, 5 khối/ngày)
| Khối | Chủ đề | Thuật ngữ chính | Ví dụ lab2 |
|---|---|---|---|
| **Ngày 1 · NHÌN** | | | |
| V-01 | Phân cấp & điểm nhấn | visual hierarchy, focal point, Von Restorff, squint test, de-emphasize, consistency ≠ uniformity | GV-001: bản cam vs 3 bố cục CC-01 |
| V-02 | Typography | modular scale, type ramp, weight, tabular figures, line-height, measure, dấu chồng tiếng Việt | GV-103 (bài subagent CC-02, có chú thích) |
| V-03 | Màu | OKLCH, neutral, semantic color, 60-30-10 / 70-20-10, accent, figure–ground, contrast | GV-001 thêm tầng 20% |
| V-04 | Khoảng cách, lưới, nhịp | spacing scale 4/8, proximity, rhythm, grid, gutter, density | GV-102 nhịp đều đều vs có nhịp |
| V-05 | Chiều sâu & hình khối | elevation, shadow, border, radius (đồng tâm), "chỉ thứ bấm được mới nổi" | gờ đáy 2px khắp nơi |
| **Ngày 2 · PATTERN** | | | |
| V-06 | Bố cục màn mobile kinh điển | list, detail, dashboard, form, master–detail, F/Z pattern, thumb zone | 4 màn lab2 xếp theo pattern |
| V-07 | Nút & điều khiển đúng nghĩa | button hierarchy (primary/secondary/tertiary), checkbox, radio, switch, segmented, chip | 35 switch GV-102 |
| V-08 | Điều hướng & kiến trúc thông tin | IA, bottom nav, tabs, top app bar, back, breadcrumb, mỗi tab một câu hỏi | Tổng quan vs Lịch (UX-002) |
| V-09 | Trạng thái & phản hồi | empty, loading (skeleton), error, success, offline, toast, snackbar, undo | GV-001 các trạng thái .E .L .X |
| V-10 | Định luật UX bằng hình | Fitts, Hick, Miller (đúng nghĩa), Jakob, Doherty, peak-end, aesthetic-usability | nút Điểm danh, menu lớp |
| **Ngày 3 · CHẠM & ÁP DỤNG** | | | |
| V-11 | Trợ năng bằng con số | contrast 4.5:1 / 3:1, target 24/44/48, focus ring, color-not-alone, reduced motion | vì sao nút 48dp (W10) |
| V-12 | Chuyển động 1 | purpose of motion, duration, easing (ease-out/in), 12 nguyên lý | mở QR, chuyển tab |
| V-13 | Chuyển động 2 | spring (stiffness, damping), stagger, micro-interaction, transform/opacity | nút Chốt điểm danh |
| V-14 | Phong cách & "AI slop" | flat, material, neumorphism, glass, brutalism, bento; dấu hiệu mặc định AI | gallery |
| V-15 | Tổng hợp: ra lệnh AI làm lại lab2 | design brief, từ điển ra lệnh, checklist nhận diện | brief GV-001 hoàn chỉnh |

**Sau V-15:** người dùng làm lại lab2 qua AI bằng brief và từ điển. Lúc đó mới bật lại phê bình (PRC-004) nếu người dùng muốn.

## 4. Nhịp chat
- **Một chat làm liên tiếp nhiều khối** (2–3 khối) tới khi chat dài thì mở chat mới (PRC-006 sửa theo D-019).
- Mở chat: clone → đọc PROGRESS → làm khối tiếp theo ngay, **không hỏi, không quiz đầu khối**. Tóm tắt đầu phiên tối đa 2 dòng.
- Trong khối: Claude dựng artifact, publish, giải thích ngắn trong chat (≤ 10 dòng) những gì nên bấm thử. Người dùng có thể hỏi; Claude **không** giao bài, **không** chấm.
- Cuối khối: cập nhật từ điển, glossary, PROGRESS, push. Hỏi đúng một câu: "Sang khối tiếp?".
