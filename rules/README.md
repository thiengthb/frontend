# Bộ luật thiết kế (rules/)

> Đây là **sản phẩm chính** của repo. Khi làm project mới, đưa thư mục này cho AI kèm câu lệnh:
> *"Tuân thủ mọi luật `adopted`. Coi `draft` là gợi ý. Nếu phá luật, nêu ID và lý do."*

## Cách đọc một luật
Mỗi luật theo `templates/rule.md`, gồm:
- **ID**: `NHÓM-số`, ví dụ `COL-001`
- **Loại**: `standard` (chuẩn, gần bắt buộc) · `heuristic` (nên theo, có ngoại lệ) · `preference` (gu riêng)
- **Trạng thái**: `draft` → `adopted` → `deprecated`
- **Luật** (một câu), **Lý do**, **Áp dụng khi / Không áp dụng khi**, **Ví dụ**, **Nguồn**, **Bài học gốc**

## Khác biệt với thienui / ui-standard của sakubun
Luật ở đây ưu tiên **cấp trang và cấp ý nghĩa** (điểm nhấn, nhịp, hành động chính, ngữ nghĩa control).
Luật cấp pixel (cỡ icon, chiều cao nút) vẫn thuộc về design system của từng sản phẩm. Lý do: xem `lessons/M0-01-baseline.md`, W1 và W7.

## Mục lục
| File | Nhóm | Luật | Ghi chú |
|---|---|---|---|
| `visual.md` | VIS | 001–005 (draft) | 001–003 từ M0-01; 004–005 từ CC-01 |
| `typography.md` | TYP | — | M2 |
| `color.md` | COL | 001 (draft) | góp ý 70-20-10 của thầy, cập nhật sau M0-01 |
| `layout.md` | LAY | — | M1, M4 |
| `ux.md` | UX | 001–002 (draft) | 002 từ CC-01 |
| `content.md` | CNT | — | M5 |
| `components.md` | CMP | 001 (draft) | từ M0-01 |
| `interaction.md` | INT | — | M9 (animation) |
| `a11y.md` | A11Y | — | M7 |
| `tokens.md` | — | — | M10 |
| `process.md` | PRC | 004, 006 (adopted); 001, 002, 005 (draft); 003 (deprecated) | 004 Critique Loop; 005 Figma chỉ đọc; 006 mỗi khối một chat |

> Cập nhật bảng này mỗi khi thêm hoặc đổi trạng thái luật.
