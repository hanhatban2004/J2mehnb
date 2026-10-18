# J2ME Web (không CheerpD / khong CheerpJ)

Môi trường chạy game J2ME (.jar) ngay trên trình duyệt, viết thuần bằng JavaScript (dựa trên J2ME.js / J2meJS, GPL-2.0). Không cần Java, không dùng CheerpJ.

## Chạy trên máy

    cd thu-muc-nay
    python3 -m http.server 8080

Mở http://localhost:8080

## Trang chính

- `index.html` — chọn file .jar trên máy, cài vào bộ nhớ trình duyệt rồi chạy.
- `main.html` — chạy trực tiếp qua tham số URL (jad, jars, midletClassName, gamepad...).
- `indexbatch.html` — cài nhiều .jar cùng lúc.

## Game kèm sẵn

- Mobi Army 3 (`games/mobi_army_3.jar`) — đã thêm vào danh sách trang chủ qua `gamelist.js`.

## Triển khai (Vercel / Netlify / hosting tĩnh)

Đây là trang tĩnh, triển khai trực tiếp được. Đã kèm `vercel.json`.

## Bản quyền

GPL-2.0 (xem LICENSE). Icon emoji trong `style/emoji/` theo CC-BY 4.0.
