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

**🇬🇧 Giao diện chỉ tiếng Anh.** Ứng dụng chỉ dùng tiếng Anh; tài liệu này vẫn song ngữ.

> Bộ icon [**Majesticons**](https://majesticons.com/) (MIT) — logo là hình giọt nước, dùng cả trên web và làm icon tab trình duyệt.

---

## ✨ Tính năng

### 📁 1. Xem & chỉnh màu ACO
- Kéo thả (hoặc click) file `.aco` để mở. Hỗ trợ **ACO v1 & v2**, đọc được **tên màu** và các hệ màu RGB / HSB / CMYK / Lab / Grayscale.
- Mỗi màu hiện số thứ tự, tên, HEX, RGB và hệ màu gốc.
- **Tìm kiếm** theo tên/HEX/RGB · **sắp xếp** theo sắc độ / độ sáng / bão hoà / tên.
- Bộ lọc nâng cao: `hue:0-60` · `sat:>50` · `light:40-80` · `similar:#FF0000`.
- **Thêm / xóa / đổi tên / kéo thả đổi thứ tự** màu · **hoàn tác / làm lại** 60 bước · **lưu lại file .aco**.
- **Chuột phải** thẻ màu để mở menu nhanh.

### 🎛 2. Trình chỉnh màu — một trình cho mọi chỗ
- Nút **giọt màu** trên mỗi thẻ ACO, trên mỗi thẻ random, và trên ô màu của mỗi chip đang trộn.
- Mọi ô chọn màu khác (điểm dừng `.grd`, màu gốc…) cũng mở chính trình này.
- Ô **SV + thanh sắc độ**, xem trước **cũ → mới**, gõ được **HEX / RGB / HSL**.
- **Về màu cũ** lùi về đúng màu ban đầu · **Thêm** tạo màu mới thay vì thay thế.
- Nút **ống hút màu** (Chromium) lấy màu bất kỳ trên màn hình.
- Mọi thay đổi đều ghi vào lịch sử **hoàn tác**.

### ⚡ 3. Điều chỉnh hàng loạt & phím tắt
- Chọn các màu rồi bấm **Điều chỉnh** để **xoay sắc độ / bão hoà / độ sáng**, xem trước trực tiếp; **Đặt lại** để phục hồi, **Hủy** để quay lại.
- **Ctrl/Cmd + Z** hoàn tác · **Ctrl/Cmd + Shift + Z** (hoặc **Ctrl + Y**) làm lại
- **Ctrl/Cmd + A** chọn tất cả · **Delete / Backspace** xóa các màu đang chọn
- Menu **Trùng lặp**: đánh dấu · xóa mã trùng hoàn toàn · xóa màu gần giống nhau.

### 🌈 4. Gradient .grd
- Mở file gradient Photoshop (`.grd` **v3 & v5**) — dạng solid và noise.
- Chỉnh điểm màu, điểm trong suốt, điểm giữa, độ mượt, tham số noise; thêm / xóa gradient và điểm dừng.
- **Lưu lại file `.grd`** · copy CSS · xuất SVG · trích màu ra `.aco` · nạp vào tab ACO.

### 🎨 5. Trộn màu
- Thêm màu bằng ô chọn màu hoặc **mở file ACO** ngay trong tab; lưới chọn lọc để bỏ màu không muốn trộn.
- Tỷ lệ tự chia đều, kéo thanh trượt để chỉnh riêng từng màu; **cân bằng tỷ lệ** bằng một click.
- Bấm vào dòng **HEX / RGB / HSL** của kết quả để copy · **lưu vào lịch sử** · **nạp vào tab ACO**.
- Click ô màu của chip để đổi màu ngay trong lúc đang trộn.

### 🎲 6. Random màu
- Sinh 1–100 màu cho từng "thành viên", ngẫu nhiên hoàn toàn hoặc theo họ màu (8 họ), có chế độ không trùng.
- Click màu để copy · nút giọt màu để chỉnh tay từng màu · **nạp vào tab ACO**.

### 🌙 Giao diện — Liquid Glass (chỉ nền tối)
- **Liquid Glass**: blur nền thật kèm tăng bão hoà, viền khúc xạ và gờ sáng ở mép trên các bề mặt kính.
- **Chỉ chạy nền tối** — giao diện gần như không màu để màu của bạn là thứ duy nhất lên màu.
- **4 tab: Màu · Gradient · Trộn màu · Random**, mỗi tab chia hai cột theo đúng luồng việc.
- **Responsive**: màn hình rộng (≥1040px) có **thanh bên** dính kèm vạch trượt đánh dấu tab; điện thoại/tablet dùng **đầu trang gọn + dock kính nổi** ở đáy.
- Icon **SVG nét** bộ **Majesticons** (24×24) thay emoji, phân cấp chữ rõ ràng — không nảy, không phát sáng.
- Chuyển động tiết chế: mờ/đổi màu ngắn, vạch trượt ở menu, hiệu ứng xuất hiện so le nhỏ — và tắt hoàn toàn với `prefers-reduced-motion`.
- Ánh sáng nền sau lớp kính nhuốm theo bảng màu đang mở.

### ⚙️ Cài đặt
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
1. Mở tab **Màu ACO** → kéo thả file `.aco`.
2. Click thẻ màu để copy · nút giọt màu để chỉnh · bút chì để đổi tên.
3. Chọn nhiều màu rồi bấm **Điều chỉnh** để đổi sắc độ / độ sáng cả lô.
4. Bấm **Lưu .aco** để tải bảng màu đã chỉnh về máy.
5. Mở tab **Gradient .grd** → kéo thả file `.grd` để xem và chỉnh gradient Photoshop.
6. Mở **⚙️ Cài đặt** để đổi cỡ chữ hoặc xóa dữ liệu đã lưu.

---

## 🌐 Ngôn ngữ

**Giao diện ứng dụng chỉ dùng tiếng Anh.** Tài liệu được giữ song ngữ:

| Tài liệu | README | Hướng dẫn sử dụng |
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

## 🙏 Credits

- Icon — [**Majesticons**](https://majesticons.com/) của Gerrit Halfmann ([MIT](https://github.com/halfmage/majesticons)).
- Font, blur và các phép toán màu đều dùng API có sẵn của trình duyệt — không phụ thuộc thư viện khi chạy.

---

## 📄 Giấy phép

Tự do sử dụng cho mục đích cá nhân và công việc.
