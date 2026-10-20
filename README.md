# 🌸 Website Chúc Mừng 20/10 - Bản Độc Quyền (Custom Edition)

Website chúc mừng ngày Phụ Nữ Việt Nam 20/10 với nhân vật hoạt hình "Nụ", hiệu ứng cực quang, pháo hoa, vườn hoa neon bập bùng theo nhịp nhạc và tính năng **"Rút quẻ may mắn 20/10"** độc đáo.

---

## ❓ Câu hỏi: "Cái này chỉ chạy local được thôi à, nếu đẩy lên GitHub thì có chạy được luôn không?"

👉 **TRẢ LỜI: KHÔNG PHẢI CHỈ CHẠY LOCAL, MÀ CHẠY ONLINE 100% TRÊN GITHUB!**

Trang web này được xây dựng hoàn toàn bằng **HTML5 + CSS3 + JavaScript + Web Audio API** (thuần, không cần backend server phức tạp).
Khi bạn đẩy lên GitHub và bật tính năng **GitHub Pages** (miễn phí trọn đời):
* GitHub sẽ cung cấp ngay một đường link website trực tuyến chính thức có dạng:
  `https://<tên-tài-khoản-github>.github.io/<tên-kho>/`
* Bất kỳ ai click vào đường link này từ điện thoại (iPhone, Android...), máy tính bảng hay PC đều có thể xem thiệp, nghe nhạc, xem pháo hoa và rút quẻ may mắn mượt mà 100% y hệt như trang mẫu bạn gửi.

---

## 🌐 Hướng dẫn 3 bước đẩy lên GitHub Pages (Ai cũng làm được)

### Bước 1: Tạo Repository trên GitHub
1. Truy cập [github.com/new](https://github.com/new) (đăng nhập tài khoản GitHub của bạn).
2. Đặt tên kho lưu trữ tại mục **Repository name** (ví dụ: `2010` hoặc `chuc-mung-2010`).
3. Chọn chế độ **Public** (Bắt buộc phải chọn Public để dùng GitHub Pages miễn phí).
4. Bấm nút xanh **Create repository**.

### Bước 2: Tải tệp `index.html` lên GitHub
1. Tại trang kho lưu trữ vừa tạo, bấm vào dòng chữ nhỏ: **"uploading an existing file"**.
2. Kéo thả tệp `index.html` từ thư mục `d:\2010` vào khung tải lên của trình duyệt.
3. Chờ tải xong, cuộn xuống dưới bấm nút xanh **Commit changes**.

### Bước 3: Kích hoạt GitHub Pages để lấy link
1. Trên thanh menu ngang của repository, bấm vào **Settings** (biểu tượng bánh răng).
2. Ở cột bên trái, tìm và bấm chọn mục **Pages**.
3. Tại phần **Build and deployment**:
   * Mục **Source**: chọn `Deploy from a branch`.
   * Mục **Branch**: chọn `main` (hoặc `master`), thư mục giữ nguyên là `/ (root)`.
   * Bấm nút **Save**.
4. Chờ khoảng 1 đến 2 phút rồi tải lại trang (F5). Bạn sẽ thấy xuất hiện một khung màu xanh có link trang web của bạn:
   👉 **`https://<username>.github.io/<tên-kho>/`**
5. Bạn copy đường link này gửi qua Zalo, Messenger, Facebook cho các chị em thưởng thức!

---

## ✏️ Hướng dẫn tự chỉnh sửa lời chúc & nội dung theo ý bạn

Bạn nhấp chuột phải vào tệp `index.html` -> chọn **Open with** -> chọn **Notepad** (hoặc **VS Code**):

### 1. Sửa lời chúc ở thẻ kết (Cuối câu chuyện)
Tìm đến đoạn có ghi chú `<!-- THẺ KẾT -->` (khoảng dòng 560):
```html
<!-- Danh xưng / Tên người nhận: -->
<p class="f-to" id="f-to">Thân gửi những người phụ nữ tuyệt vời ✨</p>

<!-- Lời chúc tâm huyết của bạn: -->
<p class="f-msg" id="f-msg">
  Mong mỗi ngày của bạn đều có hoa để ngắm, có nắng ban mai sưởi ấm, có nụ cười rạng rỡ trên môi...
</p>

<!-- Tên của bạn / Chữ ký người gửi: -->
<p class="f-sign" id="f-sign">From: Người luôn trân quý bạn 💖</p>
```
*Bạn có thể gõ bất kỳ câu chữ nào bạn thích vào đây.*

---

### 2. Sửa các câu thoại của bé Nụ trong câu chuyện
Tìm đến dòng có chữ `const S = [` (khoảng dòng 625):
* Bạn có thể đổi câu chữ bé Nụ nói, ví dụ:
  `{say: 'tớ là Nụ — nàng tiên nhỏ của vườn hoa', ...}`
  `{say: 'chúc cậu thật nhiều sức khỏe...', ...}`

---

### 3. Sửa danh sách các "Quẻ may mắn 20/10"
Tìm đến dòng `const FORTUNES = [` (khoảng dòng 740):
* Bạn có thể sửa câu chữ hoặc thêm các quẻ vui nhộn, hài hước, riêng tư cho nhóm bạn / đồng nghiệp:
```javascript
const FORTUNES = [
  "🌸 Quẻ Đắc Lộc: Tiền đầy túi, tim đầy tình, công việc hanh thông, vạn sự như ý!",
  "✨ Quẻ Nhan Sắc: Trẻ mãi không già, rạng rỡ kiêu sa, nụ cười tỏa nắng!",
  "💎 Quẻ Hạnh Phúc: Được nuông chiều như công chúa, được yêu thương vô điều kiện!",
  // Bạn có thể thêm quẻ mới ở đây...
];
```

---

## 🎵 Về nhạc nền
* Bản nhạc nền *"Từng Ngày Yêu Em"* đã được mã hóa tích hợp sẵn trực tiếp 100% bên trong tệp `index.html`. Do đó bạn chỉ cần đúng duy nhất 1 tệp `index.html` tải lên GitHub là nhạc tự động chạy mượt mà, không sợ bị lỗi mất file âm thanh.
* Trong thư mục `d:\2010` cũng có sẵn tệp [audio.mp3](file:///d:/2010/audio.mp3) để bạn nghe thử trên máy.
