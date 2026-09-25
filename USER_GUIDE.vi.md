# 🎨 Chaereve ColorLab — Hướng dẫn sử dụng

Công cụ xem, trộn và xuất bảng màu Photoshop (`.aco`) chạy ngay trên trình duyệt.
**Không cần cài đặt, không cần tải dữ liệu lên mạng** — mọi thứ xử lý ngay trên máy bạn.

---

## Mục lục
1. [Bắt đầu](#1-bắt-đầu)
2. [Ngôn ngữ](#2-ngôn-ngữ)
3. [Tab "Xem ACO"](#3-tab-xem-aco)
4. [Tab "Trộn màu"](#4-tab-trộn-màu)
5. [Tab "Random màu"](#5-tab-random-màu)
6. [Công cụ — Tạo màu & Phân tích](#6-công-cụ--tạo-màu--phân-tích)
7. [Xử lý nhiều file (Batch)](#7-xử-lý-nhiều-file-batch)
8. [Tab "Gradient (.grd)"](#8-tab-gradient-grd)
9. [Cài đặt](#9-cài-đặt)
10. [Xuất ảnh & dữ liệu](#10-xuất-ảnh--dữ-liệu)
11. [Lịch sử trộn](#11-lịch-sử-trộn)
12. [Cài đặt làm App (PWA)](#12-cài-đặt-làm-app-pwa)
13. [Câu hỏi thường gặp](#13-câu-hỏi-thường-gặp)

---

## 1. Bắt đầu

- Mở file `index.html` bằng bất kỳ trình duyệt nào (Chrome, Edge, Firefox, Safari…).
- Trang có **7 tab** chính ở đầu:
  - **Xem** — mở, tìm kiếm, chỉnh sửa và xuất bảng màu từ file `.aco` / `.grd`.
  - **Tạo** — trộn màu, random màu, palette hài hòa, tạo gradient, trích màu từ ảnh, bộ màu có sẵn.
  - **Phân tích** — kiểm tra tương phản, mô phỏng mù màu, đánh giá truy cập, thống kê palette.
  - **Tệp** — gộp nhiều file `.aco`, mở và chỉnh sửa file gradient `.grd` của Photoshop.
- Nút **⚙️ Cài đặt** (góc phải trên) mở bảng cài đặt — ngôn ngữ, cỡ chữ, xóa dữ liệu và Giới thiệu.
- Nút **VI / EN** ở thanh trên cùng đổi ngôn ngữ ngay lập tức.

---

## 2. Ngôn ngữ

- Bấm **VI / EN** ở thanh trên cùng, hoặc mở **⚙️ Cài đặt → Ngôn ngữ** và chọn: Tiếng Việt hoặc English.
- Toàn bộ giao diện đổi ngay lập tức và lựa chọn được ghi nhớ cho những lần mở sau.

---

## 3. Tab "Xem ACO"

### Mở file
- **Kéo thả** file `.aco` vào ô giữa màn hình, **hoặc** click vào ô để chọn file.
- Hỗ trợ file ACO **v1 và v2**, đọc được **tên màu** và các hệ màu RGB / HSB / CMYK / Lab / Grayscale.

### Xem màu
- Mỗi màu hiển thị dạng thẻ: **số thứ tự** (1, 2, 3…), ô màu, tên màu, mã HEX, giá trị RGB và hệ màu gốc.
- Số thứ tự đi theo **thứ tự trong file ACO**, giúp bạn dễ đối chiếu.

### Sao chép mã màu
- **Click vào thẻ màu** để copy mã (định dạng tùy chọn: HEX / RGB / HSL — chọn ở menu "HEX" trên thanh công cụ).
- Nút **📋 Sao chép tất cả** để copy toàn bộ màu dưới dạng: danh sách HEX, CSS Variables, SCSS, JSON hoặc RGB.

### Chọn nhiều màu
- Click dấu **✓** ở góc thẻ để chọn/bỏ chọn màu.
- Nút **☑ Chọn** → Chọn tất cả / Bỏ chọn / Đảo ngược.

### Tìm kiếm & sắp xếp
- Ô **🔍** tìm theo tên, mã HEX hoặc RGB.
- Menu sắp xếp: theo thứ tự gốc, sắc độ (Hue), độ sáng, độ bão hòa hoặc tên.

### Tìm kiếm nâng cao
Gõ các từ khóa đặc biệt vào ô tìm kiếm để lọc chính xác:
- `hue:0-60` — màu có sắc độ trong khoảng này (ví dụ đỏ/vàng).
- `hue:>200` / `hue:<40` / `hue:120` — lớn hơn, nhỏ hơn, hoặc đúng sắc độ.
- `sat:>50` — độ bão hòa trên 50; `light:40-80` — độ sáng từ 40 đến 80.
- `similar:#FF0000` — màu gần với màu đó (khoảng cách RGB ≤ 80).
- Từ khóa thường vẫn dùng được; có thể kết hợp nhiều token.

### Chỉnh sửa palette
- **✏️ Đổi tên** màu ngay trên thẻ, **🗑 xóa** màu, hoặc **➕ thêm** màu mới.
- **↩ Hoàn tác / ↪ Làm lại** (tối đa 60 bước).
- **Chuột phải** thẻ màu để mở menu nhanh: copy, chi tiết, đổi tên, xuất 1 màu thành `.aco`, hoặc xóa.
- **💾 Lưu .aco** ghi các thay đổi ra file `.aco` mới.

### Chia sẻ palette
- Bấm **🔗 Chia sẻ** (trên thanh công cụ) để copy link dạng `…?palette=…`.
- Mở link đó sẽ tải đúng palette — không cần server hay tài khoản.

---

## 4. Tab "Trộn màu"

Tab này dùng **độc lập**, không cần mở ACO trước.

### Thêm màu vào danh sách trộn
Có 2 cách:
1. **Ô chọn màu** + nút "➕ Thêm màu này" — chọn bất kỳ màu nào.
2. **📁 Mở file ACO** — chọn file `.aco`, sau đó hiện **lưới chọn lọc**:
   - Mặc định tất cả màu được chọn (✓).
   - **Click vào ô màu** để loại bỏ những màu bạn **không muốn trộn**.
   - Nút **Chọn tất cả / Bỏ chọn / Đảo ngược**.
   - Bấm **"➕ Thêm N màu vào trộn"** để đưa các màu đã chọn vào.

### Chỉnh lại màu mà không cần tải lại file
- Bấm nút **🔁 Chỉnh lại màu** để **mở lại lưới chọn lọc của file ACO đã tải** (không phải up file lần nữa).
- Tích/bỏ tích rồi bấm "Thêm màu vào trộn" — ứng dụng sẽ **tự thêm màu mới và bỏ màu bạn đã bỏ chọn**.

### Tỷ lệ màu
- Tỷ lệ mỗi màu được **tự động chia đều** theo số lượng màu (ví dụ 4 màu → mỗi màu 25%).
- Nút **⚖️ Cân bằng tỷ lệ** để chia đều lại bất cứ lúc nào.
- **Kéo thanh trượt** để tăng/giảm tỷ lệ riêng từng màu — phần còn lại tự tính lại cho khớp 100%.

### Kết quả trộn
- Ô kết quả hiển thị màu đã trộn cùng mã **HEX / RGB / HSL**, cập nhật tức thời khi bạn đổi tỷ lệ.
- **📋 Copy HEX / RGB / HSL** để sao chép nhanh.
- **💾 Lưu vào lịch sử** để lưu lại màu vừa trộn.

---

## 5. Tab "Random màu"

Sinh màu ngẫu nhiên, mỗi màu ứng với một **thành viên**.

- **Chế độ:** 🌈 Hoàn toàn ngẫu nhiên, hoặc 🎯 Theo họ màu (đỏ / cam / vàng / xanh lá / cyan / xanh dương / tím / hồng).
- **Số lượng màu** = số thành viên.
- **Không trùng màu** — tick để tránh màu lặp.
- Bấm **🎲 Random ngay**, rồi **click vào thẻ màu** để copy (số thứ tự = thành viên).
- **📋 Copy tất cả** copy dạng `Thành viên #1: #XXXXXX`.

---

## 6. Công cụ — Tạo màu & Phân tích

Công cụ nằm trong hai nhóm: **Tạo** và **Phân tích**.

### Nhóm Tạo
| Công cụ | Chức năng |
|---------|-----------|
| 🧩 **Palette Generator** | Tạo palette hài hòa (complementary, analogous, triadic, split, tetradic) từ một màu gốc. |
| 🌈 **Gradient Generator** | Tạo gradient CSS tuyến tính / hướng tâm / **conic** và copy mã CSS. |
| 🖼 **Image → Palette / Chấm màu** | Chấm vào ảnh để lấy 1 màu, trích các màu chủ đạo, và **xuất thẳng ra .aco**. |
| 📦 **Presets & Templates** | Bấm một cái là có ngay palette cài sẵn (Material, Tailwind, Brand Colors, Pastel, Earth Tones). |

### Nhóm Phân tích
| Công cụ | Chức năng |
|---------|-----------|
| 🔳 **Contrast Checker** | Kiểm tra tỷ lệ tương phản WCAG giữa chữ và nền, kèm huy hiệu AA/AAA. |
| 👁 **Color Blindness Preview** | Xem palette dưới góc nhìn người mù màu (protanopia / deuteranopia / tritanopia / grayscale). |
| ♿ **Accessibility Audit** | % màu trong palette đạt chuẩn AA khi ghép với chữ trắng/đen. |
| 📊 **Palette Statistics** | Độ bão hòa/độ sáng trung bình và biểu đồ phân bố sắc độ. |

Ngoài ra, bấm nút **ℹ️** trên bất kỳ thẻ màu nào sẽ mở **bảng chi tiết màu** (HEX / RGB / HSL / HSV / CMYK / Lab, độ sáng, tương phản — click từng dòng để copy).

---

## 7. Xử lý nhiều file (Batch)

Trong nhóm **Tệp → Gộp nhiều file**:

- Bấm **Mở file** và chọn **nhiều file `.aco`** cùng lúc (hoặc kéo thả).
- Danh sách hiển thị từng file kèm số màu; bấm ✕ để bỏ từng file.
- **Gộp vào Viewer** hợp nhất vào tab Xem ACO (có thể tích "bỏ màu trùng").
- **Xuất .aco gộp** tải về một file `merged-palette.aco` duy nhất.

---

## 8. Tab "Gradient (.grd)"

Trong nhóm **Tệp → Gradient .grd** bạn có thể mở, chỉnh sửa và xuất file gradient Photoshop (`.grd`, v3 & v5).

### Mở file
- Bấm **📁 Mở file .grd** (hoặc kéo thả file `.grd` vào tab) để tải các gradient.
- Mỗi gradient hiện trong danh sách kèm **ảnh xem trước** và nhãn Solid/Noise; click để chỉnh sửa.

### Chỉnh sửa gradient solid
- **Đổi tên** ở ô phía trên; **🗑** xóa gradient.
- **➕ Thêm gradient** tạo gradient đen→trắng mới.
- **Điểm màu:** click ô màu để đổi, kéo **Vị trí** (0–100%) và **Điểm giữa** để định hình chuyển tiếp, **✕** xóa điểm, **➕ Thêm điểm màu** chèn điểm ở giữa.
- **Điểm trong suốt:** tương tự — Độ đục và Vị trí cho từng điểm.
- **Độ mượt** điều chỉnh nội suy tổng thể.

### Chỉnh sửa gradient noise
- **Seed / 🎲 Đổi ngẫu nhiên**, **Độ nhiễu**, **Không gian màu**, **Thêm trong suốt**, **Giới hạn màu**, và giá trị **nhỏ nhất / lớn nhất** cho từng kênh.
- Gradient noise được tái tạo **gần đúng** (Photoshop dùng thuật toán nội bộ riêng).

### Xuất
- **📋 Copy CSS** → chuỗi `linear-gradient(…)`.
- **📐 Xuất SVG** → file gradient vector độc lập.
- **🎨 Trích màu → .aco** → lưu các điểm màu thành palette.
- **📁 Nạp vào Viewer** → đưa màu sang tab Xem ACO.
- **💾 Lưu .grd** → ghi toàn bộ gradient ra file `.grd`.

> **Lưu ý:** điểm foreground/background sẽ được quy đổi thành màu cụ thể khi mở, và khi lưu luôn ghi dưới dạng điểm người dùng với màu RGB.

---

## 9. Cài đặt

Tab **⚙️ Cài đặt** cho phép bạn cá nhân hóa ứng dụng. Mọi lựa chọn được lưu trên thiết bị của bạn.

| Mục | Chức năng |
|-----|-----------|
| **Giao diện** | **Sáng**, **Tối** hoặc **Tự động** (theo hệ thống). Nút 🌙/☀️ ở góc phải trên vẫn đổi sáng/tối nhanh. |
| **Ngôn ngữ** | Chọn Tiếng Việt hoặc English. |
| **Cỡ chữ** | Nhỏ / Vừa / Lớn. |
| **Hiệu ứng chuyển động** | Bật hoặc tắt animation. |
| **Xóa dữ liệu đã lưu** | Xóa lịch sử trộn, ngôn ngữ, cỡ chữ và mọi tùy chọn đã lưu, rồi tải lại. |
| **Giới thiệu** | Mô tả ngắn về ứng dụng. |

---

## 10. Xuất ảnh & dữ liệu

Trong tab **Xem ACO**, chọn các màu muốn xuất rồi bấm **⬇ Xuất ảnh & dữ liệu**. Một cửa sổ cho phép:

- **Bố cục**: dải ngang / dải dọc / lưới (tùy số cột).
- **Kích thước ô** và **khoảng cách** giữa các ô.
- **Nhãn**: HEX / HEX + Tên / không nhãn.
- **Nền**: trắng hoặc trong suốt.
- **Xem trước** trực tiếp trước khi tải.

Các định dạng xuất:
| Định dạng | Mô tả |
|-----------|-------|
| 🖼 PNG | Ảnh bảng màu (nét cao) |
| 📐 SVG | Vector, chỉnh sửa được |
| 🎨 CSS | Biến màu `--color-1: #…;` |
| { } JSON | Dữ liệu màu có cấu trúc |
| 📄 TXT | Danh sách mã HEX, mỗi dòng một màu |

---

## 11. Lịch sử trộn

- Nằm ở cuối tab **Trộn màu**.
- Mỗi khi bạn **copy** hoặc **lưu** một màu trộn, màu đó tự thêm vào lịch sử.
- **Click vào ô màu** trong lịch sử để copy lại ngay.
- Nút **✕** xóa từng màu, nút **🗑 Xóa lịch sử** xóa toàn bộ.
- Lịch sử được **lưu tự động** trên trình duyệt (vẫn còn khi mở lại trang).

---

## 12. Cài đặt làm App (PWA)

Ứng dụng có thể cài thành app thật trên cả máy tính và điện thoại:

| Nền tảng | Cách cài |
|----------|----------|
| **Máy tính** (Chrome/Edge) | Mở link → bấm nút **📲** ở góc phải hoặc biểu tượng cài đặt trên thanh địa chỉ → **Install** |
| **Android** (Chrome) | Mở link → menu **⋮** → **Thêm vào Màn hình chính** |
| **iPhone/iPad** (Safari) | Mở link → nút **Chia sẻ** → **Thêm vào Màn hình chính** |

Sau khi cài: app có **icon riêng**, mở **cửa sổ độc lập** (không có thanh địa chỉ), và chạy được **cả khi không có mạng** (offline).

> **Yêu cầu:** app phải được mở qua **HTTPS** (link deploy như GitHub Pages/Netlify/Vercel). Không cài được khi mở file `file://` trực tiếp.

---

## 13. Câu hỏi thường gặp

**Hỏi:** Tôi mở file nhưng không thấy màu nào?
**Đáp:** Kiểm tra file có đúng định dạng `.aco` không. Một số file xuất từ phần mềm khác có thể dùng cấu trúc khác.

**Hỏi:** Dữ liệu của tôi có bị tải lên mạng không?
**Đáp:** Không. Ứng dụng chạy hoàn toàn trên trình duyệt, không gửi bất kỳ dữ liệu nào ra ngoài.

**Hỏi:** Trộn màu kiểu gì?
**Đáp:** Ứng dụng hòa trộn các màu theo tỷ lệ (trung bình có trọng số) — giống pha sơn. Kéo thanh trượt để màu nào đó "nặng" hơn.

**Hỏi:** Làm sao để trộn chỉ một phần màu trong file ACO?
**Đáp:** Bấm "📁 Mở file ACO", bỏ chọn (click) những màu không muốn, rồi bấm "Thêm màu vào trộn".
