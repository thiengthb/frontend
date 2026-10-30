# UI/UX Playbook

Bộ kiến thức, luật thiết kế và nhật ký học UI/UX cá nhân. Repo được xây dần qua từng bài học, dùng làm
"hiến pháp thiết kế" cho mọi project frontend sau này khi làm việc cùng AI.

## Cấu trúc
```
CLAUDE.md                ← hướng dẫn cho mọi phiên Claude (đọc đầu tiên)
docs/
  00-perspective.md      ← phản biện & góc nhìn nền tảng
  01-glossary.md         ← thuật ngữ UI/UX (sống, bổ sung dần)
  02-roadmap.md          ← lộ trình học chi tiết theo module
rules/                   ← BỘ LUẬT THIẾT KẾ (sản phẩm chính)
  README.md              ← cách đọc & mục lục luật
  color.md, typography.md, layout.md, ... (sinh ra dần)
lessons/                 ← mỗi bài học một file
templates/
  lesson.md              ← mẫu bài học
  rule.md                ← mẫu một luật
  design-brief.md        ← mẫu đề bài cho AI trước khi thiết kế
  review-checklist.md    ← checklist tự review giao diện
log/
  PROGRESS.md            ← đang ở đâu, bước tiếp theo
  DECISIONS.md           ← quyết định đã chốt
  SESSIONS.md            ← nhật ký từng phiên
```

## Cách dùng với Claude
- **Claude Code / tài khoản khác:** clone repo, Claude sẽ tự đọc `CLAUDE.md`.
- **claude.ai Project:** tải các file chính (`CLAUDE.md`, `log/`, `rules/`) vào Project knowledge, rồi mở đầu bằng: *"Đọc CLAUDE.md và PROGRESS.md rồi tiếp tục."*
- **Chat thường:** dán `CLAUDE.md` và `log/PROGRESS.md` vào đầu cuộc trò chuyện.

## Dùng cho project mới
Copy thư mục `rules/` và `templates/design-brief.md` vào project, rồi bảo AI: *"Tuân thủ rules/ đã adopted. Đọc brief trước khi thiết kế."*
