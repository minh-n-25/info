# CV — Nguồn nội dung chung (Single Source of Truth)

> File này là **nguồn dữ liệu chuẩn** cho toàn bộ nội dung CV. Ba file hiển thị (`index.html`, `cv.html`, `CV_..._Fullstack_Developer.pdf`) phải khớp với file này.
> Khi sửa nội dung CV: **sửa ở đây trước**, rồi đồng bộ sang cả 3 file. Xem [Checklist đồng bộ](#checklist-đồng-bộ) ở cuối.
>
> Cập nhật lần cuối: 2026-07-03

---

## Thông tin cơ bản

| Trường | Giá trị chuẩn |
|---|---|
| **Họ tên** | NGUYEN DO ANH MINH |
| **Chức danh** | Fullstack Developer \| RPA & DX |
| **Trạng thái** | Available in Ho Chi Minh City from Dec 2026 |

## Liên hệ

| Trường | Giá trị chuẩn |
|---|---|
| **Email** | anhminhnguyen.8x@gmail.com |
| **Điện thoại** | +81 70 4034 0789 \| +84 77 280 6044 |
| **LinkedIn** | linkedin.com/in/anh-minh-nguyen-jp2023 |
| **Địa chỉ** | Binh Thanh Ward, Ho Chi Minh City, Vietnam (from Dec 2026 \| currently Tokyo, Japan) |

> **Định dạng SĐT chuẩn:** dạng có khoảng cách `+81 70 4034 0789 | +84 77 280 6044`. `index.html` và `cv.html` đã theo chuẩn này. **PDF vẫn còn dạng liền** (`+817040340789 | +84772806044`) — cần tạo lại PDF để khớp.

## Career Summary

Fullstack & Backend Developer and Solution Architect with **4+ years designing, building, operating, and maintaining web systems end-to-end** (Laravel/PHP, MySQL, REST APIs, AWS, Docker, Linux) on top of **8+ years in infrastructure engineering and system design**. Drives digital transformation (DX) as an **RPA Developer** (BizRobo!, n8n) automating labor-intensive processes in the travel field, alongside server operation, debugging, and data analysis. **Returning to Vietnam in December 2026** and seeking a long-term Fullstack / Backend Developer, Solution Architect, or RPA Developer role in Ho Chi Minh City.

## Top Skills

- Fullstack & Backend Development (Laravel, PHP, MySQL, REST API, JavaScript)
- AI-Driven Development (LLMs, Agentic AI, BMAD-METHOD)
- RPA Development & DX (BizRobo!, n8n, Workflow Automation)
- Cloud & DevOps (AWS, Docker, Linux, VM Server)
- Solution Architecture, System Design & Operation
- Data Analysis & Reporting
- Networking (WAN, VPN Site-to-Site)
- Firewalls (Juniper, Fortigate, Zywall)

## Languages

| Ngôn ngữ | Trình độ | Bars (index.html) |
|---|---|---|
| Vietnamese | Native | 5 |
| Japanese | Intermediate | 3 |
| English | Upper-Intermediate | 4 |

> Ghi chú: `cv.html` và PDF chỉ liệt kê Japanese + English (tiếng Việt là bản ngữ nên bỏ qua). `index.html` liệt kê cả 3.
> Bản dịch JP cho English đã thống nhất: `英語 (中上級)` (= Upper-Intermediate).

## Work Experience

### 1. Fullstack Developer (RPA & DX)
- **Công ty:** H.I.S. Co., Ltd.
- **Thời gian:** September 2019 – Present (6 years 10 months)
- **Địa điểm:** Tokyo, Japan
- **Mô tả:**
  - **AI Research & Application (2024 – Present):** Applied **LLMs** (ChatGPT, Claude, Gemini, Perplexity) and the **Google AI ecosystem** (NotebookLM, Google AI Studio, Google Stitch) to accelerate fullstack development and RPA workflows; leveraged **agentic AI / AI-driven development** (Claude Code, Claude Cowork) and the **BMAD-METHOD** (Agile-based AI-agent workflow management) to speed up coding, automation design, and delivery.
  - **Fullstack Development (2022 – Present):** Designed, built, operated, and maintained internal web systems end-to-end with **Laravel/PHP, MySQL, JavaScript** — from requirements analysis and UI/database design to implementation, testing, deployment, and day-to-day operation.
  - **Server operation & maintenance:** Administered VM/AWS servers and Docker environments; monitored, debugged, and resolved production incidents to keep internal systems running stably.
  - **RPA & DX (2021 – Present):** Developed RPA robots (**BizRobo!, n8n**) automating reservation-management workflows, increasing productivity and reducing manual labor across travel operations.
  - **Data analysis:** Aggregated and analyzed booking and operational data to support reporting and business decisions.
  - **Infrastructure Focus (2019 – 2021):** Managed and supported internet network deployment for **international branches**; transformed and distributed **WAN NETWORK (CATO NETWORK)** for overseas branches, particularly in Southeast Asia.

### 2. Chief of IT Solution Dept.
- **Công ty:** H.I.S. SONG HAN VN TOURIST CO., LTD
- **Thời gian:** October 2013 – August 2019 (5 years 11 months)
- **Địa điểm:** Ho Chi Minh City, Vietnam
- **Mô tả:**
  - Led the IT Solution Department (System Team Leader: 5 staff).
  - **Managed Project:** Developed a system for managing bookings and arranging Car-Driver-Guide services using **PHP and Linux**.
  - Established **Active Directory** for 3 branch offices and 5+ stores, supporting over 400 computers and users.
  - Managed networking, including VPN site-to-site connectivity and working with **Juniper, Fortigate, Zywall** firewalls.

## Education

- **Bằng cấp:** Engineer's Degree
- **Trường:** HCMC University of Technology and Education
- **Thời gian:** 2006 – 2011
- **Chuyên ngành:** System, Networking, and LAN/WAN Management

## Stats (chỉ hiển thị ở index.html)

| Giá trị | Nhãn |
|---|---|
| 8+ | Years Infrastructure |
| 4+ | Years Fullstack Dev |
| 400+ | Users Managed |
| 2 | Countries Worked |

---

## Nơi nội dung nằm trong từng file

| File | Cách chứa nội dung |
|---|---|
| **index.html** | Mảng JavaScript gần cuối `<script>`: `skills`, `languages`, `experience`, `stats`. Career Summary nằm trong markup `<p class="summary">`. Sửa mảng, **không** sửa markup render. |
| **cv.html** | Nội dung hardcode trong markup + object `translations` (`en`/`jp`/`vi`). Mỗi node có `data-lang-key`. Khi đổi 1 fact phải sửa **cả markup lẫn cả 3 ngôn ngữ**. |
| **PDF** | `CV_Nguyen_Do_Anh_Minh_Fullstack_Developer.pdf` — phải **tạo lại/thay thế** thủ công khi nội dung đổi. Trích text kiểm tra: `pdftotext -layout <file.pdf> -`. |

Quy ước `**text**` → `<strong>` áp dụng ở cả `index.html` và `cv.html` (regex `/\*\*(.*?)\*\*/g`). Giữ nguyên cú pháp này khi sửa.

---

## Checklist đồng bộ

Mỗi khi thay đổi bất kỳ nội dung CV, **kiểm tra và cập nhật cả 4 nơi**:

- [ ] `CV_CONTENT.md` (file này) — cập nhật trước, đây là chuẩn
- [ ] `index.html` — mảng JS tương ứng (`skills`/`languages`/`experience`/`stats`) + `<p class="summary">`
- [ ] `cv.html` — markup **và** cả 3 ngôn ngữ trong `translations` (en/jp/vi)
- [ ] `CV_..._Fullstack_Developer.pdf` — tạo lại PDF cho khớp

Kiểm tra nhanh còn lệch không:
```bash
pdftotext -layout "CV_Nguyen_Do_Anh_Minh_Fullstack_Developer.pdf" - | less   # đọc text PDF
grep -n "Laravel" index.html cv.html                                          # so khớp 1 fact cụ thể
```

### Nhật ký kiểm tra

| Ngày | Thay đổi | Người/ghi chú |
|---|---|---|
| 2026-07-03 | Kiểm tra nhất quán 3 file sau khi pull. Sửa `cv.html`: `Laravel 9` → `Laravel` (markup + en/jp/vi), `5 stores` → `5+ stores` (markup). Tạo file nguồn chung này. Còn tồn: định dạng SĐT (index có cách vs cv/pdf liền) và dịch JP English `業務限定`. | Claude |
| 2026-07-03 | Thống nhất SĐT dạng có khoảng cách trong `cv.html` (markup + en/jp/vi) — khớp `index.html`. Đổi dịch JP English `業務限定` → `中上級`. **Lưu ý: PDF vẫn còn SĐT dạng liền, cần tạo lại PDF.** | Claude |
| 2026-07-03 | Thêm bullet **AI Research & Application (2024 – Present)** vào công ty hiện tại (H.I.S. Co., Ltd.), đặt trước bullet 2022–Present. Đồng bộ `index.html` (mảng JS) + `cv.html` (markup + en/jp/vi, key `job1_desc0`). **Lưu ý: cần tạo lại PDF để bổ sung nội dung mới.** | Claude |
| 2026-07-03 | Thêm skill **AI-Driven Development (LLMs, Agentic AI, BMAD-METHOD)** vào Top Skills (vị trí thứ 2). Đồng bộ `index.html` (mảng `skills`) + `cv.html` (markup `.skill-list`, không có bản dịch). **Lưu ý: cần tạo lại PDF.** | Claude |
| 2026-07-03 | PDF đã được cập nhật & đối chiếu — khớp toàn bộ nội dung chuẩn (bullet AI, skill AI, Laravel/PHP, SĐT có khoảng cách, 5+ stores). ✅ **3 file + PDF đã đồng bộ.** Xóa PDF cũ `CV_-_Nguyen_Do_Anh_Minh_-_Software_Developer.pdf` (không còn tham chiếu). | Claude |
| 2026-07-06 | Tối ưu keyword tuyển dụng: chèn vai trò **Backend Developer, Solution Architect, RPA Developer** + tech (REST API, Cloud & DevOps, Workflow Automation) vào **Career Summary** & **Top Skills**. Đồng bộ `index.html` (markup summary + mảng `skills`) và `cv.html` (markup summary + skill-list + cả 3 ngôn ngữ en/jp/vi). **Lưu ý: cần tạo lại PDF để khớp Summary + Skills mới.** | Claude |
