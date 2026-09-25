# 🎨 Chaereve ColorLab — Hướng dẫn sử dụng

Công cụ xem và chỉnh bảng màu Photoshop (`.aco`) cùng gradient (`.grd`) ngay trên trình duyệt.
**Không cần cài đặt, không tải dữ liệu lên mạng** — mọi thứ xử lý trên máy bạn.

---

## Mục lục

1. [Bắt đầu](#1-bắt-đầu)
2. [Cỡ chữ & cài đặt](#2-c%E1%BB%A1-ch%E1%BB%AF--c%C3%A0i-%C4%91%E1%BA%B7t)
3. [Tab 1 — Màu ACO](#3-tab-1--màu-aco)
4. [Trình chỉnh màu](#4-trình-chỉnh-màu)
5. [Điều chỉnh hàng loạt & phím tắt](#5-điều-chỉnh-hàng-loạt--phím-tắt)
6. [Tab 2 — Gradient .grd](#6-tab-2--gradient-grd)
7. [Tab 3 — Trộn màu](#7-tab-3--trộn-màu)
8. [Tab 4 — Random màu](#8-tab-4--random-màu)
9. [Cài làm app (PWA)](#9-cài-làm-app-pwa)
10. [Câu hỏi thường gặp](#10-câu-hỏi-thường-gặp)

---

## 1. Bắt đầu

- Mở `index.html` bằng bất kỳ trình duyệt nào (Chrome, Edge, Firefox, Safari…).
- Ứng dụng có **4 tab** ở thanh giữa:
  - **Màu ACO** — mở, xem, tìm kiếm và chỉnh sửa bảng màu `.aco`.
  - **Gradient .grd** — mở và chỉnh file gradient Photoshop.
  - **Trộn màu** — trộn nhiều màu theo tỷ lệ.
  - **Random** — sinh màu ngẫu nhiên cho từng thành viên.
- Nút **⚙️** mở **Cài đặt** — ở thanh bên trên máy tính, ở đầu trang trên điện thoại.

---

## 2. Cỡ chữ & cài đặt

Giao diện **chỉ dùng tiếng Anh**.

- **⚙️ Cài đặt → Cỡ chữ**: Nhỏ / Vừa / Lớn.
- Lựa chọn được ghi nhớ cho những lần mở sau. **Xóa dữ liệu đã lưu** sẽ xóa lịch sử trộn và các tuỳ chọn này.

---

## 3. Tab 1 — Màu ACO

### Mở file
- **Kéo thả** file `.aco` (hoặc `.grd`) vào ô giữa màn hình, **hoặc** click vào ô để chọn file.
- Hỗ trợ **ACO v1 & v2**, đọc được **tên màu** và các hệ màu RGB / HSB / CMYK / Lab / Grayscale.
- Sau khi mở, ô kéo thả tự thu nhỏ lại để nhường chỗ cho bảng màu — vẫn có thể bấm vào đó để mở file khác.

### Xem màu
- Mỗi màu là một thẻ gồm: **số thứ tự** (1, 2, 3…), ô màu, tên màu, mã HEX, giá trị RGB và hệ màu gốc.
- Số thứ tự đi theo **thứ tự trong file ACO**.

### Sao chép
- **Click thẻ màu** để copy mã — định dạng HEX / RGB / HSL chọn ở menu trên thanh công cụ.
- **Sao chép tất cả** copy toàn bộ màu đang chọn theo cùng định dạng đó.

### Chọn nhiều màu
- Click dấu **✓** ở góc thẻ để chọn / bỏ chọn.
- Nút **Chọn** → Chọn tất cả / Bỏ chọn tất cả / Đảo ngược lựa chọn.

### Tìm kiếm & sắp xếp
- Ô tìm kiếm theo tên, mã HEX hoặc RGB.
- Sắp xếp theo: thứ tự gốc · sắc độ · độ sáng · độ bão hoà · tên.

### Tìm kiếm nâng cao
Gõ trực tiếp vào ô tìm kiếm:
- `hue:0-60` — sắc độ trong khoảng (đỏ → vàng). `hue:>200`, `hue:<40`, `hue:120` cũng dùng được.
- `sat:>50` — độ bão hoà lớn hơn 50. Hỗ trợ `<`, `>` và khoảng `20-80`.
- `light:40-80` — độ sáng trong khoảng.
- `similar:#FF0000` — các màu gần giống mã này nhất hiện viền trắng.

### Sửa palette
- **Thêm màu** — chọn màu ở ô vuông rồi bấm **Thêm màu**.
- **Đổi tên** — nút bút chì trên thẻ.
- **Xóa** — nút thùng rác trên thẻ.
- **Đổi thứ tự** — kéo thả thẻ màu.
- **Chuột phải** thẻ màu để mở menu nhanh (copy / chi tiết / đổi tên / xuất .aco / xóa).
- **Hoàn tác / Làm lại** — 60 bước.
- **Lưu .aco** — ghi đè toàn bộ palette ra file `.aco` (v2, có tên màu).
- **Xuất .aco** — chỉ xuất các màu đang chọn.

### Trùng lặp
Menu **Trùng lặp** có 3 lựa chọn:
- **Đánh dấu / bỏ đánh dấu** — viền vàng quanh các màu trùng hoặc gần giống.
- **Xóa mã trùng hoàn toàn** — giữ lại một màu cho mỗi mã HEX.
- **Xóa màu gần giống nhau** — bỏ các màu cách nhau một khoảng rất nhỏ.

---

## 4. Trình chỉnh màu

Một trình duy nhất dùng ở mọi nơi có màu:

| Nơi | Cách mở |
|---|---|
| Thẻ màu ACO | nút **giọt màu** trên thẻ |
| Chip đang trộn | click **ô màu** của chip |
| Thẻ random | nút **giọt màu** góc thẻ |
| Điểm dừng `.grd` | click ô màu của điểm dừng |
| Bất kỳ ô chọn màu nào | click vào ô |

Bên trong trình:
- **Ô vuông lớn** — kéo ngang = độ bão hoà, kéo dọc = độ sáng.
- **Thanh sắc độ** bên dưới — kéo để đổi màu cơ bản.
- Các ô **HEX / R G B / H S L** — gõ trực tiếp vào.
- **Xem trước cũ → mới** ở trên cùng, kèm tên màu gợi ý.
- **Về màu cũ** — lùi về đúng màu lúc mở.
- **Thêm** — tạo màu mới thay vì thay thế (chỉ hiện ở nơi hỗ trợ).
- Nút **ống hút** (Chromium) — lấy màu bất kỳ trên màn hình.

Mọi thay đổi đều ghi vào lịch sử **Hoàn tác**.

---

## 5. Điều chỉnh hàng loạt & phím tắt

- Chọn các màu, bấm **Điều chỉnh** trên thanh công cụ.
- Kéo **Xoay sắc độ / Bão hoà / Độ sáng** — bảng màu thay đổi ngay để xem trước.
- **Đặt lại** đưa các thanh về 0 · **Hủy** hoàn tác toàn bộ · **Áp dụng** giữ lại kết quả (và ghi vào Hoàn tác).

| Phím | Tác dụng |
|---|---|
| `Ctrl/Cmd + Z` | Hoàn tác |
| `Ctrl/Cmd + Shift + Z` hoặc `Ctrl + Y` | Làm lại |
| `Ctrl/Cmd + A` | Chọn tất cả màu |
| `Delete` / `Backspace` | Xóa các màu đang chọn |
| `Esc` | Đóng cửa sổ đang mở |

---

## 6. Tab 2 — Gradient .grd

- Kéo thả hoặc click để mở file `.grd` (**v3 & v5**), gồm dạng **solid** và **noise**.
- Danh sách gradient ở bên trái — click để chọn gradient cần sửa.
- Với gradient **solid**: chỉnh từng điểm màu (vị trí, điểm giữa, màu), điểm trong suốt và độ mượt.
- Với gradient **noise**: chỉnh seed, độ roughness, giới hạn màu, và các tuỳ chọn hiển thị.
- **Thêm gradient** · **Xóa gradient** · **Lưu .grd** ghi ra file mới.
- Ngoài ra có: copy CSS `linear-gradient`, xuất SVG, trích các màu ra `.aco`, hoặc nạp vào tab ACO.

---

## 7. Tab 3 — Trộn màu

- **Thêm màu** bằng ô chọn màu, hoặc **Mở file ACO** để chọn lọc từ cả bảng màu.
- Kéo thả file `.aco` thẳng vào panel cũng được.
- **Cân bằng tỷ lệ** chia đều các màu; kéo thanh trượt trên mỗi chip để chỉnh riêng.
- Click **ô màu** của chip để đổi màu đó ngay trong lúc trộn.
- Kết quả hiện HEX / RGB / HSL — **bấm vào dòng tương ứng để copy**.
- **Lưu vào lịch sử** để giữ lại kết quả; click vào mục trong lịch sử để copy lại.
- **Nạp vào ACO** đưa kết quả trộn sang tab Màu ACO để chỉnh tiếp.

---

## 8. Tab 4 — Random màu

- Chọn chế độ **Hoàn toàn ngẫu nhiên** hoặc **Theo họ màu** (8 họ: đỏ, cam, vàng, xanh lá, cyan, xanh dương, tím, hồng).
- Nhập **số lượng màu** (tương ứng số thành viên), tích **Không trùng màu** nếu muốn.
- Bấm **Random ngay** để sinh.
- Click thẻ để copy · nút **giọt màu** để chỉnh tay từng màu · **Nạp vào ACO** để đưa sang tab Màu ACO.

---

## 9. Cài làm app (PWA)

| Nền tảng | Cách cài |
|---|---|
| **Windows / macOS / Linux** (Chrome, Edge) | Mở link → biểu tượng **cài đặt** trên thanh địa chỉ |
| **Android** (Chrome) | Menu ⋮ → **Cài đặt ứng dụng** |
| **iPhone/iPad** (Safari) | Mở link → nút **Chia sẻ** → **Thêm vào Màn hình chính** |

App có icon riêng, mở cửa sổ độc lập và chạy **offline**.

---

## 10. Câu hỏi thường gặp

**Dữ liệu của tôi có bị tải lên không?**
Không. Mọi thứ đọc và xử lý ngay trong trình duyệt trên máy bạn.

**Mở được những file gì?**
`.aco` (v1 & v2) và `.grd` (v3 & v5).

**Có chỉnh được màu rồi lưu lại file gốc không?**
Có — chỉnh xong bấm **Lưu .aco**, bạn sẽ tải được file `.aco` mới.

**Hoàn tác được bao nhiêu bước?**
60 bước cho mỗi lần mở file.

**Tại sao không thấy nút ống hút màu?**
Nút này chỉ hiện trên trình duyệt Chromium (Chrome, Edge). Các trình duyệt khác vẫn chỉnh màu bình thường.

**Ứng dụng dùng ngôn ngữ gì?**
Chỉ tiếng Anh. Các tài liệu có bản Việt, nhưng giao diện app là tiếng Anh.
