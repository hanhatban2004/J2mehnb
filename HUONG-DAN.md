# Môi trường J2ME web (không CheerpJ)

Nguồn: github.com/Rosabis/J2meJS (GPL-2.0) - trình giả lập J2ME viết thuần bằng JavaScript.

## Chạy thử

Vào thư mục `j2mejs/java` rồi chạy:

    python3 -m http.server 8080

Mở `http://localhost:8080`. Thư mục `games/` chưa tồn tại, bạn tạo nó để đặt file `.jar` của mình.

## Trang chính

- `index.html`: chọn file `.jar` trên máy, cài vào bộ nhớ trình duyệt rồi chạy. Có tùy chọn kích thước màn hình, bàn phím ảo, tỷ lệ phóng và chọn nhân giả lập (tương thích / chuẩn / xem trước).
- `main.html`: chạy một `.jar` trực tiếp, hỗ trợ tham số URL (jad, jars, midletClassName, gamepad...).
- `indexbatch.html`: cài nhiều `.jar` cùng lúc.
- `updatelog.html`: nhật ký thay đổi.

## Thêm game vào danh sách trang chủ

Sửa `gamelist.js`, ví dụ:

    var GameList = [{ name: "Game của tôi", jarName: "games/MyGame.jar", picPath: "img/MyGame.png" }];

Đặt file `.jar` vào `java/games/`, ảnh minh họa vào `java/img/`.

## Đã loại bỏ so với repo gốc

- Thư mục game demo `java/jar/` (khoảng 20 MB) và toàn bộ nhánh KaiOS.
- Script thống kê Baidu trong index.html và indexbatch.html.
- Danh sách game mẫu trong gamelist.js, thay bằng danh sách rống kèm ví dụ.

## Giấy phép

GPL-2.0, giữ nguyên file LICENSE từ dự án gốc.
