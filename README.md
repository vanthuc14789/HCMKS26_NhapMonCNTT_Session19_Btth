---


---

<h1 id="bài-tập-session-18-an-toàn-thông-tin-cá-nhân-cho-developer">BÀI TẬP SESSION 18: AN TOÀN THÔNG TIN CÁ NHÂN CHO DEVELOPER</h1>
<h2 id="phần-1-–-nhận-diện-rủi-ro-và-xử-lý-sự-cố">Phần 1 – Nhận diện rủi ro và xử lý sự cố</h2>
<ol>
<li>Tình huống 1:</li>
</ol>
<ul>
<li>
<p>Loại tấn công: Phishing kết hợp Typosquatting.</p>
</li>
<li>
<p>Dấu hiệu giả mạo: Địa chỉ <code>githuh-security.com</code> giả dạng GitHub, cố tình thay chữ <code>b</code> bằng <code>h</code>.</p>
</li>
<li>
<p>Mục đích: Lừa người dùng truy cập trang giả và nhập mật khẩu để đánh cắp tài khoản.</p>
</li>
</ul>
<ol start="2">
<li>Tình huống 2:</li>
</ol>
<ul>
<li>
<p>Cạm bẫy: Mã độc Crack (Malware).</p>
</li>
<li>
<p>Nguy hiểm: Yêu cầu tắt Windows Defender để mã độc không bị phát hiện, có thể đánh cắp dữ liệu, mật khẩu và kiểm soát máy tính.</p>
</li>
</ul>
<ol start="3">
<li>Áp dụng Quy tắc 5 KHÔNG:</li>
</ol>
<ul>
<li>
<p>Tình huống 1: Không bấm vào đường link lạ, không cung cấp mật khẩu.</p>
</li>
<li>
<p>Tình huống 2: Không tải và cài phần mềm Crack, không tắt phần mềm diệt virus.</p>
</li>
</ul>
<ol start="4">
<li>
<p>Quy trình Cấp cứu 4 Bước khi lỡ chạy file Crack:</p>
</li>
<li>
<p>Ngắt kết nối Internet ngay lập tức.</p>
</li>
<li>
<p>Báo cho bộ phận IT hoặc người phụ trách.</p>
</li>
<li>
<p>Quét mã độc và xử lý thiết bị bằng phần mềm bảo mật.</p>
</li>
<li>
<p>Đổi mật khẩu trên thiết bị an toàn, thu hồi các phiên đăng nhập và kiểm tra tài khoản.</p>
</li>
</ol>
<h2 id="phần-2-–-chuyển-sang-password-manager">Phần 2 – Chuyển sang Password Manager</h2>
<ol>
<li>Rủi ro khi dùng chung mật khẩu:</li>
</ol>
<p>Nếu email nhóm bị lộ mật khẩu, hacker có thể dùng mật khẩu đó đăng nhập GitHub và Vercel.</p>
<p>Đây là kiểu tấn công Credential Stuffing (tái sử dụng thông tin đăng nhập bị lộ).</p>
<ol start="2">
<li>Zero-Knowledge Architecture:</li>
</ol>
<p>Bitwarden mã hóa dữ liệu ngay trên thiết bị người dùng trước khi đồng bộ lên máy chủ. Vì vậy, máy chủ chỉ lưu dữ liệu đã mã hóa, hacker không thể đọc được nếu không có khóa giải mã phù hợp.</p>
<ol start="3">
<li>Cấu hình Generator tạo 3 mật khẩu mới:</li>
</ol>

<table>
<thead>
<tr>
<th>Thông số</th>
<th>Giá trị cấu hình</th>
</tr>
</thead>
<tbody>
<tr>
<td>Độ dài</td>
<td>20 ký tự</td>
</tr>
<tr>
<td>Chữ hoa (A–Z)</td>
<td>Bật</td>
</tr>
<tr>
<td>Chữ thường (a–z)</td>
<td>Bật</td>
</tr>
<tr>
<td>Chữ số (0–9)</td>
<td>Bật</td>
</tr>
<tr>
<td>Ký tự đặc biệt</td>
<td>Bật</td>
</tr>
</tbody>
</table><p>Tạo 3 mật khẩu khác nhau cho GitHub, Vercel và Email nhóm. Không sử dụng chung mật khẩu.</p>
<h2 id="phần-3-–-kích-hoạt-2fa-cho-tài-khoản-github-tổ-chức">Phần 3 – Kích hoạt 2FA cho tài khoản GitHub tổ chức</h2>
<ol>
<li>Vì sao nên dùng Authenticator App (TOTP)?</li>
</ol>
<p>Nên dùng Google Authenticator thay SMS OTP vì:</p>
<ul>
<li>
<p>SMS OTP có nguy cơ bị đánh cắp qua tấn công SIM Swapping.</p>
</li>
<li>
<p>SMS OTP có thể bị nghe lén hoặc khai thác lỗ hổng mạng viễn thông SS7.</p>
</li>
</ul>
<p>TOTP tạo mã ngay trên điện thoại, không cần Internet hay sóng điện thoại.</p>
<ol start="2">
<li>
<p>Các bước kích hoạt 2FA bằng Google Authenticator:</p>
</li>
<li>
<p>Đăng nhập tài khoản GitHub.</p>
</li>
<li>
<p>Vào Settings → Password and authentication.</p>
</li>
<li>
<p>Chọn Enable two-factor authentication.</p>
</li>
<li>
<p>Chọn Authenticator App.</p>
</li>
<li>
<p>Mở Google Authenticator trên điện thoại.</p>
</li>
<li>
<p>Quét mã QR trên GitHub.</p>
</li>
<li>
<p>Nhập mã OTP 6 số hiển thị trên ứng dụng để xác nhận.</p>
</li>
<li>
<p>Lưu trữ 10 mã khôi phục:</p>
</li>
</ol>
<ul>
<li>
<p>Nên lưu: In ra giấy cất trong két sắt hoặc lưu trong Password Manager đã mã hóa.</p>
</li>
<li>
<p>Không nên lưu: Trong email, nhóm chat, thư mục công khai hoặc chụp ảnh lưu trong điện thoại không bảo vệ.</p>
</li>
</ul>
<h2 id="phần-4-–-bảo-vệ-secrets-trước-khi-push-code">Phần 4 – Bảo vệ Secrets trước khi Push Code</h2>
<ol>
<li>Hai giá trị Secret đang bị hardcode:</li>
</ol>
<ul>
<li>
<p>API Key: <code>sk-proj-abc123456789</code></p>
</li>
<li>
<p>DB Password: <code>SmartCampus@2026</code></p>
</li>
</ul>
<ol start="2">
<li>Code sau khi sửa (<code>config.js</code>):</li>
</ol>
<pre><code>const API_KEY = process.env.API_KEY;
const DB_PASSWORD = process.env.DB_PASSWORD;

function connectDatabase() {
  return connect(DB_PASSWORD);
}
</code></pre>
<ol start="3">
<li>Nội dung 3 file cần tạo</li>
</ol>
<p>File <code>.env</code> (chứa giá trị thật):</p>
<pre><code>API_KEY=YOUR_REAL_API_KEY
DB_PASSWORD=YOUR_REAL_DB_PASSWORD
</code></pre>
<p>Thay hai giá trị mẫu bằng Secret thật trong môi trường làm việc. Không đưa file này lên GitHub.</p>
<p>File <code>.gitignore</code>:</p>
<pre><code>.env
.env.*
!.env.example
node_modules/
</code></pre>
<p>File <code>.env.example</code> (chỉ chứa tên biến):</p>
<pre><code>API_KEY=
DB_PASSWORD=
</code></pre>
<ol start="4">
<li>
<p>Quy tắc 4 Bước Kiểm tra trước khi Push:</p>
</li>
<li>
<p>Kiểm tra mã nguồn, đảm bảo không còn mật khẩu hoặc API Key viết trực tiếp trong code.</p>
</li>
<li>
<p>Kiểm tra <code>.gitignore</code> đã bỏ qua file <code>.env</code>.</p>
</li>
<li>
<p>Kiểm tra <code>.env.example</code> chỉ chứa tên biến, không chứa Secret thật.</p>
</li>
<li>
<p>Kiểm tra bằng <code>git status</code> và <code>git diff</code> để chắc chắn không có dữ liệu bí mật trước khi chạy <code>git push</code>.</p>
</li>
</ol>
<p>Lưu ý: Nếu Secret đã từng bị đẩy lên GitHub, cần thu hồi và tạo Secret mới ngay, không chỉ xóa khỏi code.</p>

