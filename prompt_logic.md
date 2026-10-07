# Prompt Logic — The Interactive Showcase

## Prompt 01 — Phân rã kiến trúc

> Hãy đóng vai Senior UI/UX Designer và Frontend Developer. Dựa trên challenge "The Interactive Showcase" của học phần Thiết kế Web, hãy phân rã một trang Smart Interface thành các phần Semantic HTML5: Header, Nav, Main, Hero, Project/Portfolio, Services, Team, Process, CTA và Footer. Ưu tiên cấu trúc dễ maintain, không lạm dụng div.

## Prompt 02 — Design System + Responsive

> Hãy xây dựng CSS theo tư duy Mobile First. Tạo CSS Variables cho màu sắc, typography, spacing, radius, transition-speed và cubic-bezier. Dùng Grid cho layout lớn, Flexbox cho component con. Desktop dùng Grid nhiều cột; Tablet 2 cột; Mobile 1 cột. Không dùng float và tránh width cố định cho container. Hình ảnh phải max-width:100%; height:auto.

## Prompt 03 — Intro Animation

> Thêm Intro Animation cho Header và Hero. Header fade-in + slide-down nhẹ, Hero content slide-up, visual slide-in từ bên phải. Chỉ animate transform và opacity, không animate top/left/margin. Dùng cubic-bezier(.22, 1, .36, 1) để chuyển động tự nhiên. Có delay hợp lý giữa các thành phần.

## Prompt 04 — Card Hover / Flip

> Thiết kế project card có hover lift bằng transform: translateY() và Team Card Flip 3D bằng perspective + transform-style: preserve-3d + rotateY(180deg). Trên mobile phải có keyboard focus để người dùng vẫn truy cập được mặt sau.

## Prompt 05 — AOS Scroll Reveal

> Tích hợp AOS qua CDN. Các section/card lần lượt dùng data-aos="fade-up", "fade-left" hoặc "zoom-in". Cấu hình once:true, duration khoảng 700–900ms, offset hợp lý. Tôn trọng prefers-reduced-motion để người dùng có thể giảm chuyển động.

## Prompt 06 — Micro-interaction

> Tạo CTA button có 3 trạng thái: bình thường, hover và active. Hover nâng nút lên 3px bằng transform và tăng shadow; active thu nhỏ nhẹ bằng transform: scale(.97). Dùng cubic-bezier để cảm giác click rõ nhưng không gây khó chịu.

## Prompt 07 — Performance Refactor

> Review toàn bộ CSS animation. Tuyệt đối không dùng top/left để tạo chuyển động. Thay bằng transform: translate/scale/rotate hoặc opacity. Tìm transition dư thừa, gom CSS Variables và đảm bảo animation không gây horizontal overflow trên mobile.

## Prompt "Bậc thầy" — cubic-bezier

> Hãy audit toàn bộ motion system của giao diện và chuẩn hóa timing function. Dùng cubic-bezier(.22, 1, .36, 1) cho reveal/entrance, cubic-bezier(.34, 1.56, .64, 1) cho micro-interaction có cảm giác spring. Giữ duration trong khoảng 300–800ms tùy mức độ chuyển động. Không animate layout properties như top, left, width, height, margin. Ưu tiên transform và opacity. Giải thích ngắn gọn vì sao từng easing phù hợp với từng nhóm animation.

## Tư duy UX đã áp dụng

- Intro: tạo cảm giác mở đầu có chủ đích nhưng không chặn nội dung.
- Project hover: phản hồi nhẹ để người dùng biết card có thể tương tác.
- Flip card: thông tin chính ở mặt trước, thông tin liên hệ ở mặt sau để giảm mật độ.
- AOS: chia nhịp đọc khi cuộn, tránh tất cả nội dung xuất hiện cùng lúc.
- CTA: hover/active giúp xác nhận hành động.
- Reduced motion: không ép hiệu ứng với người dùng nhạy cảm với chuyển động.
