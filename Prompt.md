# Hello JS Console — Đối thoại với trình duyệt (30 phút)

## Prompt sử dụng với AI

> Hãy đóng vai một lập trình viên JavaScript và hướng dẫn người mới học thực hành trực tiếp trong tab Console của trình duyệt. Giải thích ngắn gọn, dễ hiểu bằng tiếng Việt cách khai báo tên và tuổi, sau đó thực hiện phép cộng, trừ, nhân và chia. Hãy trả lời câu hỏi: “Tại sao khi cộng `'10' + 20` trong JavaScript lại ra `'1020'` mà không phải `30`?”. Giải thích sự khác nhau giữa chuỗi và số, quy tắc nối chuỗi của toán tử `+`, cách chuyển chuỗi thành số bằng `Number()`, và đưa ra các câu lệnh có thể tự gõ trong Console.

## Cách chạy bài thực hành

1. Mở tệp `index.html` bằng trình duyệt.
2. Nhấn **F12** (hoặc **Ctrl+Shift+J** trên Chrome) và chọn tab **Console**.
3. Xem các kết quả được in ra, rồi tự gõ các câu lệnh mẫu bên dưới để đối thoại với trình duyệt.

## Thử trực tiếp trong Console

```js
const ten = "Nguyễn An";
const tuoi = 20;

console.log("Xin chào, mình tên là " + ten + ".");
console.log("Năm nay mình " + tuoi + " tuổi.");

const a = 10;
const b = 20;
console.log(a + b); // 30
console.log(a - b); // -10
console.log(a * b); // 200
console.log(a / b); // 0.5

console.log("10" + 20); // "1020"
console.log(Number("10") + 20); // 30
```

> Nếu đã khai báo `const ten`, `const tuoi`, `const a` hoặc `const b` trong cùng Console, hãy dùng tên biến khác hoặc tải lại trang trước khi khai báo lại. Một `const` không thể được khai báo hai lần trong cùng phạm vi.

## Giải thích code

- `const ten = "Nguyễn An";` khai báo biến `ten` có giá trị là một **chuỗi**. Chuỗi được đặt trong dấu nháy.
- `const tuoi = 20;` khai báo biến `tuoi` có giá trị là một **số**.
- `console.log(...)` gửi nội dung ra tab Console để xem.
- Với hai toán hạng là số, `+`, `-`, `*` và `/` lần lượt thực hiện cộng, trừ, nhân và chia.
- Khi một toán hạng của `+` là chuỗi, JavaScript chuyển toán hạng còn lại thành chuỗi và **nối** chúng. Vì vậy:

  ```js
  "10" + 20 // "1020"
  ```

  Đây là kết quả dạng chuỗi `"1020"`, không phải phép cộng số học.
- `Number("10")` chuyển chuỗi `"10"` thành số `10`. Do đó:

  ```js
  Number("10") + 20 // 30
  ```

### Thời lượng gợi ý (30 phút)

- **5 phút:** Mở trang, mở Console và làm quen với `console.log()`.
- **10 phút:** Khai báo tên, tuổi và in lời chào.
- **10 phút:** Thử các phép cộng, trừ, nhân, chia với những số khác nhau.
- **5 phút:** So sánh `"10" + 20` với `Number("10") + 20`, rồi giải thích kết quả bằng lời của bạn.
