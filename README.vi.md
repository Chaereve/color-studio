# 🎨 Chaereve ColorLab

<p align="center">
  <a href="https://github.com/chaereve/chaereve-colorlab/releases"><img alt="Tải xuống" src="https://img.shields.io/badge/T%E1%BA%A3i%20xu%E1%BB%91ng-2ea043?style=for-the-badge"></a>
</p>

<p align="center">
  <a href="README.md"><img alt="English" src="https://img.shields.io/badge/English-1a3fd6?style=for-the-badge"></a>&nbsp;
  <a href="README.vi.md"><img alt="Tiếng Việt" src="https://img.shields.io/badge/Ti%E1%BA%BFng%20Vi%E1%BB%87t-22d3ee?style=for-the-badge"></a>&nbsp;
</p>

Công cụ **xem, trộn và xuất bảng màu Photoshop (`.aco`)** — chạy **ngay trên trình duyệt**. Không cần cài đặt, không cần đăng ký, không tải dữ liệu lên mạng.

> Mọi dữ liệu được xử lý **hoàn toàn cục bộ** trên máy/điện thoại của bạn.

**🌐 Song ngữ:** Tiếng Việt · English — đổi ngay ở thanh trên cùng hoặc trong **⚙️ Cài đặt**.

---

## ✨ Tính năng

### 📁 Xem ACO
- Kéo thả (hoặc click) file `.aco` để mở.
- Hỗ trợ **ACO v1 & v2**, đọc được **tên màu** và các hệ màu RGB / HSB / CMYK / Lab / Grayscale.
- Mỗi màu hiển thị **số thứ tự**, tên màu, HEX, RGB và hệ màu gốc.
- **Tìm kiếm** theo tên/HEX/RGB và **sắp xếp** theo sắc độ, độ sáng, bão hòa, tên.
- **Tìm kiếm nâng cao** — lọc theo dải `hue:0-60`, `sat:>50`, `light:40-80`, hoặc tìm màu gần với `similar:#FF0000`.

### ✏️ Chỉnh sửa palette (trực tiếp)
- **Đổi tên** màu (✏️), **xóa** (🗑), hoặc **thêm** màu mới — rồi **lưu lại file .aco**.
- **Hoàn tác / làm lại** đầy đủ (tối đa 60 bước).
- **Chuột phải** thẻ màu để mở menu nhanh (copy / chi tiết / đổi tên / xuất / xóa).

### 📋 Sao chép
- Click thẻ màu để copy mã (**HEX / RGB / HSL** — tùy chọn).
- **Copy tất cả** dưới dạng: danh sách HEX, CSS variables, SCSS, JSON, RGB, **Tailwind config**, **Styled Components**.

### 🎨 Trộn màu (dùng độc lập — không cần mở ACO)
- Thêm màu bằng **ô chọn màu** hoặc **mở file ACO** ngay trong tab này.
- Lưới chọn lọc giúp **loại bỏ màu không muốn trộn** bằng một click.
- **Chỉnh lại lựa chọn** mà không cần tải lại file.
- Tỷ lệ **tự động chia đều** theo số lượng màu; kéo thanh trượt để chỉnh riêng.
- **Lịch sử trộn** tự lưu, click để copy lại.

### 🎲 Random màu (cho từng thành viên)
- Sinh 1–100 màu ngẫu nhiên cho từng "thành viên", hoàn toàn ngẫu nhiên hoặc theo họ màu (đỏ / cam / vàng / xanh lá / cyan / xanh dương / tím / hồng), có chế độ không trùng màu.

### 🛠 Công cụ thiết kế
Tách thành 2 tab — **🧩 Tạo màu** và **🔍 Phân tích**:
- **Palette Generator** — complementary / analogous / triadic / split / tetradic.
- **Gradient Generator** — gradient CSS tuyến tính / hướng tâm / **conic**, copy mã CSS.
- **Image → Palette / Chấm màu** — chấm vào ảnh lấy màu, trích màu chủ đạo, và **xuất thẳng ra .aco**.
- **Presets & Templates** — thư viện cài sẵn: Material Design, Tailwind, Brand Colors, Pastel, Earth Tones.
- **Contrast Checker** — tỷ lệ tương phản WCAG kèm huy hiệu AA/AAA.
- **Accessibility Audit** — % màu trong palette đạt AA khi ghép với chữ trắng/đen.
- **Palette Statistics** — độ bão hòa/độ sáng trung bình và biểu đồ phân bố sắc độ.
- **Color Blindness Preview** — protanopia / deuteranopia / tritanopia / grayscale.
- **Bảng chi tiết màu** — HEX / RGB / HSL / HSV / CMYK / Lab, độ sáng, tương phản.
- **Phát hiện trùng lặp** và **tìm màu tương tự**.

### 📦 Xử lý nhiều file (Batch)
- Mở **nhiều file .aco** cùng lúc, **gộp** thành một palette (có chế độ bỏ trùng) hoặc **xuất .aco gộp**.

### 🔗 Chia sẻ palette
- Tạo **link chia sẻ** (`?palette=...`) mã hóa palette hiện tại — ai mở link cũng thấy cùng màu, không cần server.

### 📐 Gradient (.grd)
- Mở file **gradient Photoshop** (`.grd`, **v3 & v5**) — dạng solid và noise.
- **Xem trước** từng gradient, rồi **chỉnh sửa** điểm màu, điểm trong suốt, điểm giữa, độ mượt, và các tham số noise (seed, roughness, min/max).
- **Thêm / xóa gradient** và điểm dừng, rồi **lưu lại file `.grd`**.
- Xuất gradient ra **CSS `linear-gradient`** hoặc **SVG**, và **trích màu ra `.aco`** hoặc nạp thẳng vào Viewer.

### ⬇ Xuất
- **PNG / SVG / CSS / JSON / TXT** với tùy chọn bố cục, kích thước, nhãn, nền (kể cả trong suốt).
- **Xuất .aco** (v2, có tên màu) từ các màu đã chọn.

### 🌙 Giao diện — Liquid Glass (chỉ nền tối)
- Chất liệu **Liquid Glass**: blur nền thật kèm tăng bão hòa, viền khúc xạ và gờ sáng ở mép trên của các bề mặt kính.
- **Chỉ chạy nền tối** — giao diện gần như không màu để màu của bạn là thứ duy nhất lên màu.
- Gọn từ 7 tab rời rạc xuống **4 nhóm: Xem · Tạo · Phân tích · Tệp**.
- Dùng **icon SVG nét** thay emoji, hệ thống chữ có phân cấp rõ ràng, chuyển động chỉ ở mức màu sắc/độ mờ — không nảy, không phát sáng.
- Ánh sáng nền phía sau lớp kính nhuốm theo bảng màu bạn đang mở.
- Tương thích tốt trên màn hình nhỏ.

### ⚙️ Cài đặt
- **Ngôn ngữ** — Tiếng Việt / English.
- **Cỡ chữ** (nhỏ / vừa / lớn).
- **Xóa dữ liệu đã lưu** và mục **Giới thiệu**.

### 📲 Cài làm app (PWA)
- Cài được trên **máy tính (Windows/macOS/Linux)** và **điện thoại (Android/iOS)**.
- Có icon riêng, mở cửa sổ độc lập, chạy **offline**.

### 🖥 Bản desktop (Windows)
- Đóng gói thành **ứng dụng desktop Windows** bằng Electron — xem thư mục `electron-app/`.
- Build bộ cài **Windows**: `.exe` (bộ cài NSIS + bản portable).
- Logo ứng dụng được bo **góc vuông** như các app hiện đại.

---

## 🚀 Cách dùng

### Trên máy tính / điện thoại
Mở `index.html` bằng trình duyệt bất kỳ (nhấp đúp), hoặc truy cập link đã deploy.

### Quy trình nhanh
1. Mở tab **📁 Xem ACO** → kéo thả file `.aco`.
2. Click màu để copy, hoặc tick nhiều màu để xuất.
3. Mở tab **🎨 Trộn màu** → thêm màu → xem kết quả trộn ngay.
4. Bấm **⬇ Xuất ảnh & dữ liệu** để tải bảng màu.
5. Mở tab **📐 Gradient** → kéo thả file `.grd` để xem và chỉnh sửa gradient Photoshop.
6. Mở **⚙️ Cài đặt** (hoặc bấm **VI / EN** ở thanh trên cùng) để đổi ngôn ngữ và cỡ chữ.

---

## 🌐 Ngôn ngữ (2)

Đổi bằng nút **VI / EN** ở thanh trên cùng, hoặc qua **⚙️ Cài đặt → Ngôn ngữ**: Tiếng Việt · English. Toàn bộ giao diện đổi ngay lập tức và lựa chọn được ghi nhớ cho những lần sau.

| Ngôn ngữ | README | Hướng dẫn sử dụng |
|----------|--------|-------------------|
| 🇬🇧 English | [README.md](README.md) | [USER_GUIDE.md](USER_GUIDE.md) |
| 🇻🇳 Tiếng Việt | [README.vi.md](README.vi.md) | [USER_GUIDE.vi.md](USER_GUIDE.vi.md) |

---

## 📲 Cài làm app (PWA)

Sau khi app deploy (qua HTTPS), bạn có thể cài thành app thật:

| Nền tảng | Cách cài |
|----------|----------|
| **Máy tính** (Chrome/Edge) | Mở link → nút **📲** hoặc biểu tượng cài đặt trên thanh địa chỉ → **Install** |
| **Android** (Chrome) | Mở link → menu **⋮** → **Thêm vào Màn hình chính** |
| **iPhone/iPad** (Safari) | Mở link → nút **Chia sẻ** → **Thêm vào Màn hình chính** |

> **Lưu ý:** PWA cần phục vụ qua **HTTPS** (GitHub Pages, Netlify, Vercel đều có sẵn). Không cài được khi mở `file://` trực tiếp.

---

## ❓ FAQ

**Dữ liệu có bị tải lên mạng không?**
Không. App chạy hoàn toàn trên trình duyệt.

**Mở file không thấy màu?**
Kiểm tra file có đúng `.aco` không. Một số phần mềm xuất ACO cấu trúc khác.

**Trộn màu kiểu gì?**
Pha theo tỷ lệ (trung bình có trọng số) — giống pha sơn. Kéo thanh trượt để màu "nặng" hơn.

**Muốn trộn một phần màu trong file?**
Mở ACO ở tab **Trộn màu** → bỏ chọn màu không muốn → bấm **Thêm màu vào trộn**.

---

## 📚 Hướng dẫn

Hướng dẫn sử dụng:
- 🇬🇧 [USER_GUIDE.md](USER_GUIDE.md) · 🇻🇳 [USER_GUIDE.vi.md](USER_GUIDE.vi.md)

---

## 📄 Giấy phép

Tự do sử dụng cho mục đích cá nhân và công việc.
