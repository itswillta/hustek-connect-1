# AGENTS — HuSTek Connect Series #01 (repo prep)

Repo nội bộ chuẩn bị **HUSTEK CONNECT #01: Future-proof bản thân trong kỷ nguyên AI** (13/06, AI4LIFE). Collaborators: **Tạ Quốc Huy**, **Hà Xuân Thuyên**.

Mục tiêu chính của file này: hướng dẫn AI assistant (Cursor, v.v.) cách làm việc trong repo — **không** chứa toàn bộ talking points (nội dung sống trong `ta_quoc_huy/`, `ha_xuan_thuyen/`, `phoi_hop/`).

---

## Quy ước đặt tên

- **Path** (file & folder): `snake_case`, tiếng Việt **không dấu**; token English / brand được phép (vd. `pageai`, `faq`, `chu_de`).
- **Ngoại lệ tên file:** `AGENTS.md`, `CLAUDE.md`, `CONTEXT.md`, `SKILL.md`, `README.md`, … — xem [.agents/skills/naming-convention/SKILL.md](.agents/skills/naming-convention/SKILL.md).
- **Nội dung** markdown: tiếng Việt **có dấu** bình thường (script, câu trả lời).

Khi tạo hoặc đổi tên file/folder → đọc skill **naming-convention** trước.

---

## Người mới vào repo

Lần đầu / chưa rõ vai / hỏi “repo này là gì”, “tôi nên làm gì” → chạy skill **[repo-onboarding](.agents/skills/repo-onboarding/SKILL.md)** (AI đọc AGENTS + `tai_lieu_chung/CONTEXT.md`, hỏi vai trò, chỉ folder và việc tiếp theo).

---

## Skills (`.agents/skills/`)

| Skill | Khi dùng |
|-------|----------|
| [repo-onboarding](.agents/skills/repo-onboarding/SKILL.md) | Mới vào, hỏi cấu trúc repo / việc nên làm theo vai |
| [naming-convention](.agents/skills/naming-convention/SKILL.md) | Tạo hoặc đổi tên file/folder |

---

## Đọc trước khi làm việc

1. [tai_lieu_chung/CONTEXT.md](tai_lieu_chung/CONTEXT.md) — sự kiện, timeline chính thức, nguồn Facebook post.
2. Context theo người dùng:
   - Prep cho **Huy** → [ta_quoc_huy/CONTEXT.md](ta_quoc_huy/CONTEXT.md), sau đó các file canonical trong `ta_quoc_huy/`.
   - Prep cho **Thuyên** → [ha_xuan_thuyen/CONTEXT.md](ha_xuan_thuyen/CONTEXT.md) (chỉ khi user là Thuyên hoặc được yêu cầu rõ).
   - Phối hợp 2 diễn giả → [phoi_hop/CONTEXT.md](phoi_hop/CONTEXT.md).

---

## Thứ bậc nguồn (source of truth)

| Ưu tiên | Nguồn | Ghi chú |
|--------|--------|---------|
| 1 | [tai_lieu_chung/bai_dang_facebook_hustek_connect_01.md](tai_lieu_chung/bai_dang_facebook_hustek_connect_01.md) | Timeline 2 chủ đề, 3 pillar workshop |
| 2 | [phoi_hop/CONTEXT.md](phoi_hop/CONTEXT.md) | Chia vai Chủ đề 2, thống nhất thông điệp |
| 3 | [tai_lieu_chung/kich_ban_moderator_workshop_jun2026.md](tai_lieu_chung/kich_ban_moderator_workshop_jun2026.md) | **Reference only** — thứ tự khác FB post, không dùng làm outline prep |

---

## Cấu trúc repo

| Folder | Mục đích |
|--------|----------|
| `tai_lieu_chung/` | Post FB, kịch bản moderator (read-only), metadata sự kiện |
| `ta_quoc_huy/` | Prep diễn giả Tạ Quốc Huy |
| `ha_xuan_thuyen/` | Prep diễn giả Hà Xuân Thuyên |
| `phoi_hop/` | Co-lead, handoff, câu cần thống nhất |

Mỗi folder có **`CONTEXT.md`** — chi tiết vai trò và quy ước local. Root AGENTS chỉ mô tả luật chung.

---

## Guardrails (bắt buộc)

- **Không sửa** `ha_xuan_thuyen/` khi user là Huy (read-only để nắm context).
- **Không rewrite** [tai_lieu_chung/kich_ban_moderator_workshop_jun2026.md](tai_lieu_chung/kich_ban_moderator_workshop_jun2026.md) — giữ làm point of reference.
- **`phoi_hop/`**: chỉ chỉnh khi user yêu cầu rõ phối hợp / đồng bộ với Thuyên; ghi rõ thay đổi.
- **Không tạo file trùng** ngoài danh sách canonical trong [ta_quoc_huy/CONTEXT.md](ta_quoc_huy/CONTEXT.md) (trừ khi user yêu cầu).
- **Không tạo slide** trừ khi user yêu cầu riêng.

---

## Workflow AI (ví dụ cho Huy)

| Yêu cầu user | File chính | Ghi chú |
|--------------|------------|---------|
| Thêm ví dụ PageAI / tuyển dụng | `ta_quoc_huy/pageai_cases.md` | Cross-link sang `chu_de_1_answer_bank.md` nếu liên quan |
| Câu trả lời Chủ đề 1 | `ta_quoc_huy/chu_de_1_answer_bank.md` | Theo outline 1→5 trong `ta_quoc_huy/CONTEXT.md` |
| Câu trả lời Chủ đề 2 (phần Huy) | `ta_quoc_huy/chu_de_2_answer_bank.md` | Mục 1, 2, 5, 6 — không đè `ha_xuan_thuyen/` |
| Câu “neo” / rapid-fire | `ta_quoc_huy/anchor_script.md` | Đoạn ngắn + bullet; không văn dài cả buổi |
| In tay ngày 13/06 | `ta_quoc_huy/cheat_sheet.md` | Tối đa ~1 trang A4 |
| Q&A sinh viên | `ta_quoc_huy/faq_qa.md` | Câu dự đoán + gợi ý trả lời |
| Ý tưởng lẻ / link | `ta_quoc_huy/ideas.md` | Backlog, không nhét hết vào answer bank |

---

## Deliverable chuẩn (`ta_quoc_huy/`)

| File | Format |
|------|--------|
| `chu_de_*_answer_bank.md` | H2 theo block outline; mỗi block: bullet chính, optional anchor quote, link `pageai_cases.md` |
| `anchor_script.md` | Đoạn 2–4 câu cho moment then chốt; phần còn bullet |
| `cheat_sheet.md` | Bullet cực ngắn, checklist thông điệp, không paragraph dài |
| `faq_qa.md` | `## Câu hỏi` + bullet trả lời |
| `pageai_cases.md` | Case có consent; tag `[OK share]` / `[cần confirm]` |

---

## Tone & audience (tóm tắt)

- **Audience**: SV IT từ năm 3+, sắp tốt nghiệp, lo học tập & tuyển dụng.
- **Giọng**: ~80% mentor khích lệ; ~20% reality check (thẳng nhưng không toxic).
- **Ngôn ngữ**: Tiếng Việt chủ đạo; English chỉ khi ai cũng hiểu (AI, project, fresher, …).

Thông điệp bắt buộc và outline chi tiết: [ta_quoc_huy/CONTEXT.md](ta_quoc_huy/CONTEXT.md).

---

## Index CONTEXT

| File | Vai trò |
|------|---------|
| [tai_lieu_chung/CONTEXT.md](tai_lieu_chung/CONTEXT.md) | Sự kiện, timeline, pillar → chủ đề |
| [ta_quoc_huy/CONTEXT.md](ta_quoc_huy/CONTEXT.md) | Vai Huy, prep scope, canonical files |
| [ha_xuan_thuyen/CONTEXT.md](ha_xuan_thuyen/CONTEXT.md) | Vai Thuyên, mục 3+4 Chủ đề 2 |
| [phoi_hop/CONTEXT.md](phoi_hop/CONTEXT.md) | Co-lead, tránh overlap |
