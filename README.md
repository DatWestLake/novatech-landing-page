# Landing Page Novatech — bản chạy thử

Trang bán hàng cho 3 sản phẩm: Smart Tivi Samsung QLED 55Q6F, 65Q6F và máy sấy bơm nhiệt Hisense DH80N1T.

> **Đây là bản nháp để góp ý, chưa vận hành.**
> Giá, khuyến mãi và các cam kết trên trang **chưa phải số liệu cuối cùng**.

## Xem thử

- Bản chạy trực tiếp: *(điền link GitHub Pages vào đây sau khi bật)*
- Xem dưới máy: tải repo về, mở thẳng `index.html` bằng trình duyệt. Không cần cài gì.

## Rất mong được góp ý về

1. **Nội dung bán hàng** — tiêu đề, mô tả sản phẩm đã đủ thuyết phục chưa, có chỗ nào khó hiểu không.
2. **Giá và khuyến mãi** — con số đã đúng chưa, cách trình bày giảm giá có rõ không.
3. **Form đặt hàng** — điền thử xem có vướng chỗ nào, báo lỗi đã dễ hiểu chưa.
4. **Hiển thị trên điện thoại** — mở bằng điện thoại xem có vỡ layout, chữ có bị nhỏ quá không.
5. **Tốc độ tải** — mở bằng 4G xem có chậm không.

Góp ý xin mở **Issue** trong repo này, hoặc nhắn trực tiếp.

## Đã có trên trang

- Đồng hồ đếm ngược 24 giờ cho chương trình khuyến mãi
- Thư viện ảnh sản phẩm, bấm vào ảnh mở popup xem cỡ lớn
- Form đặt hàng có kiểm tra định dạng số điện thoại Việt Nam
- Giao diện co giãn theo điện thoại, máy tính bảng và máy tính

## Sửa nội dung

Toàn bộ nội dung nằm trong khối `CAU_HINH` ở **đầu file `index.html`** — chia sẵn 10 mục có đánh số: thông tin liên hệ, danh sách sản phẩm, giá, ảnh, cam kết, nội dung form.
Không cần sửa phần HTML bên dưới.

Cách thêm ảnh sản phẩm: xem `images/DOC-DE-THEM-ANH.txt`.

## Cấu trúc

```
index.html                    toàn bộ trang (HTML + CSS + JS trong một file)
images/
  logo-mark.png               dấu hiệu hexagon
  logo-full.png               logo đầy đủ
  favicon.png                 biểu tượng tab trình duyệt
  samsung-q6f-*.webp          ảnh tivi Samsung
  dh80n1t-*.webp              ảnh máy sấy Hisense
  DOC-DE-THEM-ANH.txt         hướng dẫn thêm ảnh
```

## Ghi chú kỹ thuật

- Tailwind CSS nạp từ CDN nên **cần mạng** khi mở trang. Khi vận hành thật nên build CSS ra file tĩnh.
- Trang đang gắn thẻ `noindex` để Google không thu thập bản nháp. **Nhớ xoá thẻ đó trong `index.html` trước khi chạy thật.**
- Form hiện chưa gửi dữ liệu đi đâu. Chỗ nối API đã đánh dấu sẵn trong `index.html`, tìm theo từ khoá `GỬI ĐƠN VỀ HỆ THỐNG CỦA BẠN`.
