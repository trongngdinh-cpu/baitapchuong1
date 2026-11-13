# Bài 2: So sánh phần đầu tài liệu của 3 trang web

| Thẻ | Facebook | Spotify | YouTube |
|---|---|---|---|
| DOCTYPE | có | có | có |
| lang | có | có | có |
| charset | không có meta, có header | có  | không có meta, có header |
| viewport | có | có | chỉ có sau JS |
| title | có | có | có |
| description | không | không | có |
| og | không | không | có |

## Hệ quả của các chỗ thiếu

- Facebook và Spotify không có description và og: - Facebook và Spotify không có `description` và `og`: Google sẽ không có đoạn tóm tắt do chủ trang viết, nên tự cắt một đoạn chữ nào đó trong trang để hiện dưới tiêu đề, có thể không đúng ý. Khi chia sẻ link lên mạng xã hội, thiếu Open Graph thì mạng xã hội tự đoán tiêu đề, mô tả và ảnh, nên thẻ xem trước có thể sai ảnh, mô tả bị cắt tuỳ tiện hoặc thiếu ảnh, và chủ trang không kiểm soát được.
- YouTube viewport chỉ có sau JS: trong lúc JS chưa chạy, điện thoại có thể dựng trang theo khổ mặc định 980px rồi giật lại khi thẻ xuất hiện, và nếu JS lỗi hoặc chậm thì trang vẫn bị chữ li ti. YouTube ít bị ảnh hưởng vì trang này vốn cần JS mới hiện nội dung; trang thường nên đặt viewport thẳng trong HTML.
