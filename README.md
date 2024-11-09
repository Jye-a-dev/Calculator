1. Design.css <br>
This file provides the styling for the calculator interface.
Key styles include:
General Layout: The body element is set to a white background. Font color and size are customized for different tags (AA, AB, AC) to enhance text visibility on various buttons.
Containers:
.Container: Defines a primary container for the calculator, styled with a linear gradient background and a solid border, positioned slightly off-center.
.Display: Used for the calculator display screen, styled with a gray background and 3px solid border.
#Standard: Styles the calculator’s standard button layout with a hover effect changing the background color to light yellow.
.StandardCal: Defines the main area where buttons are displayed, with a gradient background and solid black borders.
Button Styles: Buttons are individually styled with width, height, border, and hover effects to change color. Each button is positioned using absolute values to maintain layout within .StandardCal.
<br>

2. Calculator.html <br>
This HTML file structures the calculator's UI, linking the styling from Design.css and scripting from Calculate.js.
HTML Structure:
Container and Display: A div with class .Container wraps the .Display where calculation results are shown.
Buttons: The calculator includes buttons for numbers (0-9), operations (+, -, *, /, ** for power, sqrt for square root), parentheses, and utility functions (e.g., Clear, Back, and = for calculation).
Classes and Styles: Each button is associated with a class or ID that links it to styling in Design.css and functionality in Calculate.js. Buttons use onclick events to call JavaScript functions (clearDisplay, deleteLastChar, appendToDisplay, and calculateResult).
<br>

3. Calculate.js <br>
This JavaScript file manages the calculator's functionality.
Key Functions:
appendToDisplay(value): Appends numbers, operators, or special functions to currentExpression and updates the display.
calculateResult(): Evaluates the expression stored in currentExpression. If an error occurs during evaluation (e.g., syntax error), "Error" is displayed.
clearDisplay(): Clears currentExpression and the display content.
deleteLastChar(): Removes the last character from currentExpression. Specific checks handle multi-character functions like Math.sqrt( and **.
Keyboard Events: The script listens for keydown events, mapping keys for digits, operators, Enter, Backspace, Escape, and other functions.
<br>
VIETNAMESE <br>

1. Thiết kế.css
Tệp này cung cấp kiểu dáng cho giao diện máy tính.
Các phong cách chính bao gồm:
Bố cục chung: Phần tử nội dung được đặt thành nền trắng. Màu sắc và kích thước phông chữ được tùy chỉnh cho các thẻ khác nhau (AA, AB, AC) để nâng cao khả năng hiển thị văn bản trên các nút khác nhau.
Thùng chứa:
.Container: Xác định vùng chứa chính cho máy tính, được tạo kiểu bằng nền gradient tuyến tính và đường viền liền nét, được đặt hơi lệch tâm.
.Hiển thị: Được sử dụng cho màn hình hiển thị máy tính, được tạo kiểu với nền màu xám và đường viền liền nét 3px.
#Standard: Tạo kiểu cho bố cục nút tiêu chuẩn của máy tính với hiệu ứng di chuột thay đổi màu nền thành màu vàng nhạt.
.StandardCal: Xác định khu vực chính nơi các nút được hiển thị, với nền chuyển màu và đường viền màu đen liền nét.
Kiểu nút: Các nút được tạo kiểu riêng với các hiệu ứng chiều rộng, chiều cao, đường viền và di chuột để thay đổi màu sắc. Mỗi nút được định vị bằng các giá trị tuyệt đối để duy trì bố cục trong .StandardCal.
<br>

2. Máy tính.html
Tệp HTML này cấu trúc giao diện người dùng của máy tính, liên kết kiểu dáng từ Design.css và tập lệnh từ Calculate.js.
Cấu trúc HTML:
Vùng chứa và Hiển thị: Một div có lớp .Container bao bọc .Display nơi hiển thị kết quả tính toán.
Các nút: Máy tính bao gồm các nút cho số (0-9), các phép toán (+, -, *, /, ** cho lũy thừa, sqrt cho căn bậc hai), dấu ngoặc đơn và các hàm tiện ích (ví dụ: Xóa, Quay lại và = cho tính toán).
Lớp và Kiểu: Mỗi nút được liên kết với một lớp hoặc ID liên kết nút đó với kiểu dáng trong Design.css và chức năng trong Calculate.js. Các nút sử dụng sự kiện onclick để gọi các hàm JavaScript (clearDisplay, deleteLastChar,appendToDisplay và CalculateResult).
<br>

3. Tính toán.js
Tệp JavaScript này quản lý chức năng của máy tính.
Chức năng chính:
appendToDisplay(value): Nối số, toán tử hoặc hàm đặc biệt vào currentExpression và cập nhật màn hình.
tínhResult(): Đánh giá biểu thức được lưu trữ trong currentExpression. Nếu xảy ra lỗi trong quá trình đánh giá (ví dụ: lỗi cú pháp), "Lỗi" sẽ được hiển thị.
clearDisplay(): Xóa currentExpression và nội dung hiển thị.
deleteLastChar(): Xóa ký tự cuối cùng khỏi currentExpression. Kiểm tra cụ thể xử lý các hàm nhiều ký tự như Math.sqrt( và **.
Sự kiện bàn phím: Tập lệnh lắng nghe các sự kiện nhấn phím, phím ánh xạ cho các chữ số, toán tử, Enter, Backspace, Escape và các chức năng khác.
