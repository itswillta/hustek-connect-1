# HuSTek Connect — repo prep (Series #01)

Kho tài liệu **nội bộ** chuẩn bị workshop **HUSTEK CONNECT #01: Future-proof bản thân trong kỷ nguyên AI**. Repo này không phải website công khai — dùng để gom timeline, script, ý tưởng diễn giả và phối hợp với BTC Lab / moderator trước ngày sự kiện.

| | |
|--|--|
| **Ngày** | Thứ Bảy **13/06/2026**, sáng |
| **Địa điểm** | AI4LIFE |
| **Lab** | [HuSTek Lab](https://hustek.io.vn/) — Human Speech Technology Laboratory, ĐHBK HN |
| **Liên hệ BTC** | trangntt@soict.hust.edu.vn |
| **Fanpage** | https://www.facebook.com/hustek.lab/ |

**Diễn giả:** Tạ Quốc Huy (PageAI) · Hà Xuân Thuyên (NCB / Sun Group)

---

## Mục đích repo

1. **Một nguồn sự thật** cho nội dung đã đăng (post Facebook) và timeline chính thức.
2. **Prep tách theo người** — mỗi diễn giả có folder riêng; phần phối hợp nằm ở `phoi_hop/`.
3. **Hỗ trợ soạn nội dung** — markdown dễ sửa; có thể dùng AI (Cursor) theo [AGENTS.md](AGENTS.md) và skills trong `.agents/skills/`.
4. **Tùy chọn làm slide** — từ nội dung đã soạn, dùng skill [revealjs](.agents/skills/revealjs/SKILL.md) để tạo bài trình chiếu HTML (mở trình duyệt, chuyển slide như PowerPoint).

---

## Ngữ cảnh sự kiện

### Timeline chính thức (theo bài đăng Facebook)

| Thời gian | Nội dung |
|-----------|----------|
| **9:00–10:15** | **Chủ đề 1:** Nghịch lý tuyển dụng thời AI — Doanh nghiệp cần gì ở sinh viên mới |
| 10:15–10:30 | Tea-break |
| 10:30–10:50 | Biểu diễn piano (Lab) |
| **10:50–11:45** | **Chủ đề 2:** Gốc rễ kỹ thuật vững trước thay đổi liên tục của công nghệ |

Nguồn chi tiết: [tai_lieu_chung/bai_dang_facebook_hustek_connect_01.md](tai_lieu_chung/bai_dang_facebook_hustek_connect_01.md)

### Ba chủ đề xuyên suốt (toàn buổi)

- **Học & AI** — AI là trợ lý, tránh phụ thuộc tool kiểu “con vẹt”.
- **Gốc rễ vs công cụ** — cân bằng fundamentals và ship nhanh.
- **Tuyển dụng** — kỹ năng, kinh nghiệm, CV trong mùa thị trường khắt khe hơn.

> **Lưu ý:** File [kich_ban_moderator_workshop_jun2026.md](tai_lieu_chung/kich_ban_moderator_workshop_jun2026.md) là **tham khảo** (thứ tự câu hỏi khác timeline FB). Điều phối trên sân khấu nên bám timeline Facebook.

---

## Cấu trúc thư mục

```
hustek-connect-1/
├── AGENTS.md                 # Luật chung cho AI + cộng tác viên dùng Cursor
├── README.md                 # File này — hướng dẫn cho người
├── tai_lieu_chung/           # Timeline, post FB, kịch bản moderator
├── ta_quoc_huy/              # Prep diễn giả Tạ Quốc Huy
├── ha_xuan_thuyen/           # Prep diễn giả Hà Xuân Thuyên
├── phoi_hop/                 # Phối hợp 2 diễn giả (Chủ đề 2, handoff)
└── .agents/skills/           # Hướng dẫn cho AI (onboarding, đặt tên, slide…)
```

Mỗi folder prep có **`CONTEXT.md`** — đọc file đó trước khi sửa nội dung trong folder.

### Ai nên đọc / sửa folder nào?

| Vai trò | Folder | Việc thường làm |
|---------|--------|------------------|
| BTC Lab, cô giáo, **moderator** | `tai_lieu_chung/` | Xem timeline, post FB; tham khảo kịch bản |
| **Tạ Quốc Huy** | `ta_quoc_huy/` | Answer bank, script, case study, cheat sheet, FAQ |
| **Hà Xuân Thuyên** | `ha_xuan_thuyen/` | Prep phần enterprise / platform (mục 3–4 Chủ đề 2) |
| Cả hai diễn giả | `phoi_hop/` | Thống nhất kịch bản và slides giữa 2 diễn giả, tránh trùng nội dung |

---

## Cách sử dụng

### 1. Đọc và chỉnh markdown

- Nội dung chính là file `.md` (tiếng Việt **có dấu** trong file).
- Tên file/folder: `snake_case`, tiếng Việt **không dấu** (vd. `chu_de_1_answer_bank.md`). Chi tiết: skill [naming-convention](.agents/skills/naming-convention/SKILL.md).

### 2. Lần đầu vào repo

- Đọc [tai_lieu_chung/CONTEXT.md](tai_lieu_chung/CONTEXT.md) rồi `CONTEXT.md` trong folder của bạn.
- Nếu dùng **Cursor / AI**: mở [AGENTS.md](AGENTS.md); có thể nhắc AI chạy skill **[repo-onboarding](.agents/skills/repo-onboarding/SKILL.md)** để được hỏi vai trò và gợi ý việc tiếp theo.

### 3. Prep diễn giả (ví dụ `ta_quoc_huy/`)

| File | Mục đích |
|------|----------|
| `chu_de_1_answer_bank.md` | Nội dung Chủ đề 1 (tuyển dụng) |
| `chu_de_2_answer_bank.md` | Nội dung Chủ đề 2 (phần Huy) |
| `anchor_script.md` | Câu “neo” / rapid-fire |
| `cheat_sheet.md` | Tóm tắt 1 trang in ngày workshop |
| `faq_qa.md` | Câu hỏi SV dự đoán + gợi ý trả lời |
| `pageai_cases.md` | Case study (có tag đồng ý chia sẻ) |
| `ideas.md` | Ý tưởng lẻ, link tham khảo |

Danh sách đầy đủ và outline: [ta_quoc_huy/CONTEXT.md](ta_quoc_huy/CONTEXT.md).

### 4. Làm slide trình chiếu (Reveal.js)

**Reveal.js** là thư viện slide chạy trên **trình duyệt** (HTML + CSS), không bắt buộc PowerPoint.

- Soạn / chỉnh nội dung trong repo trước.
- Nhờ AI (Cursor) dùng skill **[revealjs](.agents/skills/revealjs/SKILL.md)** để tạo file HTML (vd. `presentation.html`).
- Mở file bằng Chrome/Edge → trình chiếu (phím mũi tên, fullscreen).

Ví dụ tham khảo trong repo: `.agents/skills/revealjs/examples/`.

---

## Skills cho AI (`.agents/skills/`)

| Skill | Khi dùng |
|-------|----------|
| [repo-onboarding](.agents/skills/repo-onboarding/SKILL.md) | Mới vào repo; hỏi “repo này là gì”, “tôi nên làm gì” |
| [naming-convention](.agents/skills/naming-convention/SKILL.md) | Tạo hoặc đổi tên file/folder |
| [revealjs](.agents/skills/revealjs/SKILL.md) | Tạo slide / presentation HTML |

Người không dùng AI vẫn làm việc bình thường chỉ với markdown và link ở trên.
