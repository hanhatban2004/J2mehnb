# J2ME Web (khong CheerpJ)

Môi trường chạy game J2ME (.jar) ngay trên trình duyệt, viết thuần bằng JavaScript (dựa trên J2ME.js / J2meJS, GPL-2.0). Không cần Java, không dùng CheerpJ.

## Chạy trên máy

    cd thu-muc-nay
    python3 -m http.server 8080

Mở http://localhost:8080

## Trang chính

- `index.html` — chọn file .jar trên máy, cài vào bộ nhớ trình duyệt rồi chạy.
- `main.html` — chạy trực tiếp qua tham số URL (jad, jars, midletClassName, gamepad...).
- `indexbatch.html` — cài nhiều .jar cùng lúc.

## Thêm game

Đặt file .jar vào thư mục `games/`, sửa `gamelist.js` để thêm vào danh sách trang chủ. Lưu ý các game online (như Mobi Army) cần máy chủ của nhà phát hành còn hoạt động mới chơi được.

## Triển khai (Vercel / Netlify / GitHub Pages)

Đây là trang tĩnh, triển khai trực tiếp được. Đã kèm `vercel.json`. Workflow GitHub Pages ở `.github/workflows/pages.yml` tự deploy mỗi lần push.

## Bản quyền

GPL-2.0 (xem LICENSE). Icon emoji trong `style/emoji/` theo CC-BY 4.0.
