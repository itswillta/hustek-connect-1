---
name: naming-convention
description: >-
  When creating or renaming files or folders in the hustek-connect prep repo:
  use snake_case and Vietnamese without diacritics on paths; respect meta-file
  exceptions (AGENTS.md, CONTEXT.md, etc.).
---

# HuSTek Connect — quy ước đặt tên

Áp dụng khi **tạo file/folder mới**, **đổi tên**, hoặc **refactor cấu trúc** trong repo prep HUSTEK CONNECT. Không áp cho **nội dung văn bản** bên trong markdown (script, câu trả lời vẫn tiếng Việt **có dấu**).

---

## Ngoại lệ (giữ đúng tên)

| Tên | Ghi chú |
|-----|---------|
| `AGENTS.md` | Root — luật repo |
| `CLAUDE.md` | Optional mirror cho Claude Code |
| `CONTEXT.md` | Mỗi folder prep — context local |
| `SKILL.md` | Trong `.agents/skills/` |
| `README.md`, `LICENSE`, `CONTRIBUTING` | Nếu có sau này |
| Mọi path dưới `.agents/**` | Skills, rules, hooks |

---

## Quy tắc path

1. **`snake_case`**, chữ thường.
2. **Không** khoảng trắng, **không** dấu tiếng Việt trên tên file/folder.
3. Phần mô tả: **tiếng Việt không dấu** (vd. `chu_de_1`, `bai_dang_facebook`).
4. **Cho phép** token English / brand phổ biến: `pageai`, `faq`, `qa`, `ai`, `script`, `cheat_sheet`, `chu_de`, `jun2026`.

Ví dụ hợp lệ: `ta_quoc_huy/chu_de_1_answer_bank.md`, `tai_lieu_chung/kich_ban_moderator_workshop_jun2026.md`.

Ví dụ không hợp lệ: `KỊCH BẢN MODERATOR.md`, `Human Speech Technology Laboratory Post.md`, `ChuDe1/`.

---

## Cấu trúc repo chuẩn

| Folder | Vai trò |
|--------|---------|
| `tai_lieu_chung/` | Post FB, kịch bản moderator (reference), metadata sự kiện |
| `ta_quoc_huy/` | Prep diễn giả Tạ Quốc Huy |
| `ha_xuan_thuyen/` | Prep diễn giả Hà Xuân Thuyên |
| `phoi_hop/` | Co-lead, handoff, thống nhất thông điệp |

Mỗi folder trên có `CONTEXT.md` (ngoại lệ tên file).

---

## File canonical trong `ta_quoc_huy/`

Không đổi tên các file sau (chỉ nằm đúng folder `ta_quoc_huy/`):

- `chu_de_1_answer_bank.md`
- `chu_de_2_answer_bank.md`
- `anchor_script.md`
- `cheat_sheet.md`
- `faq_qa.md`
- `pageai_cases.md`
- `ideas.md`

---

## File canonical trong `tai_lieu_chung/`

- `bai_dang_facebook_hustek_connect_01.md` — source of truth timeline / pillar
- `kich_ban_moderator_workshop_jun2026.md` — reference only, không rewrite nội dung

---

## Bảng migration (path cũ → mới)

**Không tạo lại path cũ.**

| Cũ | Mới |
|----|-----|
| `shared/` | `tai_lieu_chung/` |
| `huy/` | `ta_quoc_huy/` |
| `thuyen/` | `ha_xuan_thuyen/` |
| `joint/` | `phoi_hop/` |
| `shared/Human Speech Technology Laboratory Post.md` | `tai_lieu_chung/bai_dang_facebook_hustek_connect_01.md` |
| `shared/KỊCH BẢN MODERATOR WORKSHOP JUN2026.md` | `tai_lieu_chung/kich_ban_moderator_workshop_jun2026.md` |
| `.agents/skills/hustek-connect-naming/` | `.agents/skills/naming-convention/` |

---

## Checklist trước khi hoàn tất thay đổi cấu trúc

- [ ] Tên path mới: snake_case, không dấu, không space
- [ ] Link trong `AGENTS.md`, `*/CONTEXT.md`, prep files trỏ folder mới
- [ ] `rg 'shared/|huy/|thuyen/|joint/'` trong repo — chỉ còn trong bảng migration ở skill này (nếu có)
- [ ] Không thêm file prep trùng vai trò file canonical đã liệt kê

---

## Tham chiếu

Root [AGENTS.md](../../AGENTS.md) — workflow prep và guardrails nội dung.
