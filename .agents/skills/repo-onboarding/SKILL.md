---
name: repo-onboarding
description: >-
  Onboard newcomers to the hustek-connect prep repo: explain purpose, structure,
  read order, and ask the user's role to recommend what to do next. Use when
  someone is new, asks what this repo is, repo structure, or what they should work on.
---

# HuSTek Connect — repo onboarding

Giúp **người mới** nắm repo prep HUSTEK CONNECT: ngữ cảnh là gì, cấu trúc, cách hoạt động, và **việc nên làm** theo vai trò. Không nhân bản toàn bộ nội dung prep — trỏ [AGENTS.md](../../AGENTS.md) và `*/CONTEXT.md`.

---

## Khi nào áp dụng

- Người mới clone repo; BTC/moderator hoặc collaborator lần đầu.
- Câu hỏi: “repo này là gì”, “đọc file nào trước”, “tôi nên sửa folder nào”, “tôi là Thuyên thì làm gì”.

---

## Bước 1 — Đọc nhanh (bắt buộc)

1. [AGENTS.md](../../AGENTS.md) — mục đích, 4 folder, guardrails, index CONTEXT.
2. [tai_lieu_chung/CONTEXT.md](../../tai_lieu_chung/CONTEXT.md) — sự kiện 13/06, timeline, pillar FB.

Không đọc hết answer bank trừ khi user hỏi sâu một chủ đề cụ thể.

---

## Bước 2 — Hỏi vai trò (một lần)

Dùng **AskQuestion** nếu có; không thì hỏi ngắn trong chat. Cho phép mô tả tự do — map vào ID gần nhất.

| ID | Vai |
|----|-----|
| `speaker_huy` | Diễn giả / prep **Tạ Quốc Huy** |
| `speaker_thuyen` | Diễn giả / prep **Hà Xuân Thuyên** |
| `co_lead` | Phối hợp 2 diễn giả (Chủ đề 2, handoff) |
| `btc` | BTC Lab / moderator / tài liệu chung |
| `readonly` | Chỉ xem, không sửa prep |
| `maintainer` | Sửa AGENTS, skills, cấu trúc repo |

**Không** tự gán `speaker_huy` nếu user chưa xác nhận.

---

## Bước 3 — Tóm tắt repo (luôn trả lời)

Gồm các ý sau (ngắn, có dấu):

- **Mục đích:** prep nội bộ **HUSTEK CONNECT #01** — không phải site công khai.
- **Sự kiện:** Thứ Bảy **13/06**, AI4LIFE. **Chủ đề 1** (9:00–10:15) tuyển dụng thời AI; **Chủ đề 2** (10:50–11:45) gốc rễ kỹ thuật.
- **Nguồn chính:** `tai_lieu_chung/bai_dang_facebook_hustek_connect_01.md`. Kịch bản moderator = reference only (thứ tự khác FB).
- **4 folder:** `tai_lieu_chung/`, `ta_quoc_huy/`, `ha_xuan_thuyen/`, `phoi_hop/` — mỗi folder có `CONTEXT.md`.
- **Skills:** `repo-onboarding` (file này), [naming-convention](../naming-convention/SKILL.md) (đặt tên path).
- **Path:** snake_case, Việt không dấu; nội dung markdown có dấu.

---

## Bước 4 — Route theo vai

| Vai | Đọc tiếp | Được sửa | Gợi ý việc tiếp (3 mục cụ thể, có path) |
|-----|----------|----------|------------------------------------------|
| `speaker_huy` | [ta_quoc_huy/CONTEXT.md](../../ta_quoc_huy/CONTEXT.md) | `ta_quoc_huy/` canonical | `chu_de_1_answer_bank.md`, `pageai_cases.md`, `anchor_script.md` |
| `speaker_thuyen` | [ha_xuan_thuyen/CONTEXT.md](../../ha_xuan_thuyen/CONTEXT.md) | `ha_xuan_thuyen/` | Tạo `chu_de_2_answer_bank.md` (mục 3–4), `chu_de_1` góc enterprise |
| `co_lead` | [phoi_hop/CONTEXT.md](../../phoi_hop/CONTEXT.md) + 2 CONTEXT diễn giả | `phoi_hop/` khi user yêu cầu phối hợp | Handoff notes, align bảng “câu thống nhất” |
| `btc` | [tai_lieu_chung/CONTEXT.md](../../tai_lieu_chung/CONTEXT.md) | `tai_lieu_chung/` (không rewrite kịch bản) | Timeline FB cho moderator; không drive outline từ kịch bản cũ |
| `readonly` | `tai_lieu_chung/` + post FB | Không sửa prep folders | Đọc `bai_dang_facebook_hustek_connect_01.md` |
| `maintainer` | AGENTS + `.agents/skills/` | AGENTS, skills, rename | Tuân [naming-convention](../naming-convention/SKILL.md) |

**Guardrails theo vai**

- `speaker_huy`: **không** sửa `ha_xuan_thuyen/`.
- `speaker_thuyen`: **không** sửa `ta_quoc_huy/` trừ khi được yêu cầu rõ.
- Tạo/đổi tên file: áp skill **naming-convention**.

Sau route: liệt kê **đúng 3 việc** với path file — không chung chung.

---

## Output format

```markdown
## Repo là gì
(mục đích, sự kiện, 4 folder — ngắn)

## Vai bạn
(ID + tên vai)

## Đọc theo thứ tự
1. ...
2. ...

## Việc nên làm tiếp
- [ ] path/...
- [ ] path/...
- [ ] path/...

## Không nên
- ...
```

---

## Tham chiếu

- [AGENTS.md](../../AGENTS.md) — workflow prep chi tiết
- [naming-convention](../naming-convention/SKILL.md) — quy tắc đặt tên path
