---
name: "An Tâm Healthcare Portal"
description: "Hệ thống thiết kế gọn gàng, rõ ràng và đáng tin cậy cho cổng đặt lịch và tiếp nhận khám bệnh phòng khám giả lập (Agile/Scrum Demo)."
---

## Overview

**An Tâm Healthcare Portal** được thiết kế theo phong cách **Corporate / Modern Minimalism** dành riêng cho môi trường y tế: ưu tiên sự rõ ràng, tốc độ quét thông tin và khả năng phân biệt trạng thái tức thì. Giao diện sử dụng nền sáng trung tính dịu mắt, loại bỏ hoàn toàn yếu tố trang trí dư thừa (gradient, đổ bóng nặng, hiệu ứng kính mờ) để người đặt khám và nhân viên tiếp nhận tập trung vào hai nhiệm vụ cốt lõi: chọn bác sĩ – khung giờ và xử lý yêu cầu đặt lịch.

Mọi màn hình tuân thủ nguyên tắc phân cấp thị giác rõ ràng: một thao tác chính nổi bật duy nhất trên mỗi ngữ cảnh, nhãn trạng thái luôn kết hợp **biểu tượng + văn bản + màu ngữ nghĩa** (không bao giờ chỉ dùng màu sắc).

## Colors

Bảng màu lấy sắc **Xanh ngọc y tế (Clinical Teal)** làm màu chủ đạo để tạo cảm giác an tâm, chuyên nghiệp và sạch sẽ. Hệ thống phân tách rõ màu thương hiệu/tương tác và màu ngữ nghĩa trạng thái lịch hẹn.

- **Primary (`#00544F`):** Dùng cho nút hành động chính ("Gửi yêu cầu đặt lịch", "Xác nhận lịch"), liên kết đang chọn và điểm nhấn điều hướng.
- **Surface & Neutral (`#F7FAF8` → `#FFFFFF`):** Tạo phân lớp nhẹ nhàng giữa nền trang và thẻ nội dung, giữ độ tương phản chữ đạt chuẩn WCAG AA (≥ 4.5:1).
- **Màu trạng thái lịch hẹn (luôn đi kèm nhãn chữ và icon):**
  - `status-pending-container` / `on-status-pending-container`: Trạng thái **"Chờ xác nhận"** (vàng hổ phách dịu, dễ nhận biết nhưng không báo lỗi).
  - `status-confirmed-container` / `on-status-confirmed-container`: Trạng thái **"Đã xác nhận"** (xanh lục y tế).
  - `status-reschedule-container` / `on-status-reschedule-container`: Trạng thái **"Đề nghị thời gian khác"** (xanh chàm trung tính).

```yaml
colors:
  status-pending: "#92400E"
  on-status-pending: "#FFFFFF"
  status-pending-container: "#FEF3C7"
  on-status-pending-container: "#78350F"
  status-confirmed: "#065F46"
  on-status-confirmed: "#FFFFFF"
  status-confirmed-container: "#D1FAE5"
  on-status-confirmed-container: "#064E3B"
  status-reschedule: "#3730A3"
  on-status-reschedule: "#FFFFFF"
  status-reschedule-container: "#E0E7FF"
  on-status-reschedule-container: "#312E81"
  light:
    primary: "#00544F"
    on-primary: "#FFFFFF"
    primary-container: "#0D6E68"
    on-primary-container: "#9CEDE5"
    secondary: "#476461"
    on-secondary: "#FFFFFF"
    secondary-container: "#C9E9E5"
    on-secondary-container: "#183533"
    tertiary: "#753A21"
    on-tertiary: "#FFFFFF"
    tertiary-container: "#925136"
    on-tertiary-container: "#FFD6C7"
    error: "#BA1A1A"
    on-error: "#FFFFFF"
    error-container: "#FFDAD6"
    on-error-container: "#93000A"
    background: "#F7FAF8"
    on-background: "#181C1C"
    surface: "#F7FAF8"
    surface-dim: "#D7DBD9"
    surface-bright: "#FFFFFF"
    surface-container-lowest: "#FFFFFF"
    surface-container-low: "#F1F4F3"
    surface-container: "#EBEFED"
    surface-container-high: "#E6E9E7"
    surface-container-highest: "#E0E3E2"
    on-surface: "#181C1C"
    surface-variant: "#DAE5E2"
    on-surface-variant: "#3E4947"
    outline: "#6E7977"
    outline-variant: "#BEC9C7"
    inverse-surface: "#2D3130"
    inverse-on-surface: "#EEF1F0"
    inverse-primary: "#84D5CD"
  dark:
    primary: "#84D5CD"
    on-primary: "#003734"
    primary-container: "#0D6E68"
    on-primary-container: "#9CEDE5"
    secondary: "#AECDC9"
    on-secondary: "#183533"
    secondary-container: "#2F4C49"
    on-secondary-container: "#C9E9E5"
    tertiary: "#FFB598"
    on-tertiary: "#542109"
    tertiary-container: "#925136"
    on-tertiary-container: "#FFD6C7"
    error: "#FFB4AB"
    on-error: "#690005"
    error-container: "#93000A"
    on-error-container: "#FFDAD6"
    background: "#101414"
    on-background: "#E0E3E2"
    surface: "#101414"
    surface-dim: "#101414"
    surface-bright: "#363A39"
    surface-container-lowest: "#0B0F0E"
    surface-container-low: "#181C1C"
    surface-container: "#1C2020"
    surface-container-high: "#272B2A"
    surface-container-highest: "#313635"
    on-surface: "#E0E3E2"
    surface-variant: "#3E4947"
    on-surface-variant: "#BEC9C7"
    outline: "#889391"
    outline-variant: "#3E4947"
    inverse-surface: "#E0E3E2"
    inverse-on-surface: "#2D3130"
    inverse-primary: "#026A64"
```

## Typography

Hệ thống sử dụng cặp font hỗ trợ đầy đủ dấu tiếng Việt với độ rõ nét cao: **Plus Jakarta Sans** cho tiêu đề (tạo sự thân thiện, hiện đại), **Be Vietnam Pro** cho toàn bộ nội dung chức năng và nhãn nút (tối ưu cho dấu tiếng Việt ở kích thước nhỏ), và **Source Code Pro** cho mã yêu cầu (`YC-1024`), khung giờ (`08:30`) và số liệu bảng. Mọi con số giờ hẹn, mã phiếu và ngày tháng đều dùng `tabular-nums`.

```yaml
typography:
  display-lg:
    fontFamily: "Plus Jakarta Sans"
    fontSize: 36px
    fontWeight: 700
    lineHeight: 44px
    letterSpacing: -0.5px
  display-lg-mobile:
    fontFamily: "Plus Jakarta Sans"
    fontSize: 28px
    fontWeight: 700
    lineHeight: 36px
    letterSpacing: -0.25px
  headline-lg:
    fontFamily: "Plus Jakarta Sans"
    fontSize: 28px
    fontWeight: 700
    lineHeight: 36px
    letterSpacing: -0.25px
  headline-md:
    fontFamily: "Plus Jakarta Sans"
    fontSize: 22px
    fontWeight: 600
    lineHeight: 30px
    letterSpacing: -0.15px
  title-lg:
    fontFamily: "Plus Jakarta Sans"
    fontSize: 18px
    fontWeight: 600
    lineHeight: 26px
    letterSpacing: 0px
  title-md:
    fontFamily: "Be Vietnam Pro"
    fontSize: 16px
    fontWeight: 600
    lineHeight: 24px
    letterSpacing: 0px
  body-lg:
    fontFamily: "Be Vietnam Pro"
    fontSize: 16px
    fontWeight: 400
    lineHeight: 24px
    letterSpacing: 0px
  body-md:
    fontFamily: "Be Vietnam Pro"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 22px
    letterSpacing: 0px
  label-lg:
    fontFamily: "Be Vietnam Pro"
    fontSize: 14px
    fontWeight: 600
    lineHeight: 20px
    letterSpacing: 0px
  label-md:
    fontFamily: "Be Vietnam Pro"
    fontSize: 12px
    fontWeight: 600
    lineHeight: 16px
    letterSpacing: 0.2px
  label-sm:
    fontFamily: "Be Vietnam Pro"
    fontSize: 11px
    fontWeight: 500
    lineHeight: 16px
    letterSpacing: 0.2px
  mono-md:
    fontFamily: "Source Code Pro"
    fontSize: 13px
    fontWeight: 500
    lineHeight: 18px
    letterSpacing: 0px
```

## Layout & Spacing

Giao diện web sử dụng **Fixed-Max-Width Grid (tối đa 1280px)** trên màn hình desktop và **Fluid Grid** trên thiết bị nhỏ hơn. Mọi khoảng cách đều tuân thủ bội số của **8px** (với bước nửa 4px cho khoảng cách vi mô bên trong chip hoặc icon-text).

- **Cấu trúc trang Người đặt khám:** Bố cục 2 cột bất đối xứng (`8 cột` chọn chuyên khoa, bác sĩ & khung giờ + `4 cột` khung tóm tắt yêu cầu và quy tắc xác nhận cố định bên phải).
- **Cấu trúc trang Nhân viên tiếp nhận:** Bố cục 1 cột rộng cho bảng/danh sách yêu cầu kèm thanh lọc trạng thái ở trên cùng, giúp quét nhanh hàng chục yêu cầu mà không phải cuộn ngang.

```yaml
spacing:
  gutter-xs: 4px
  gutter-sm: 8px
  gutter-md: 16px
  gutter-lg: 24px
  gutter-xl: 32px
  section: 48px
  page-margin: 24px
```

## Elevation & Depth

Hệ thống áp dụng chiến lược **Tonal layers + Low-contrast outlines** (phân lớp bề mặt kết hợp viền mảnh độ tương phản thấp `outline-variant`) thay cho đổ bóng dày. Thẻ nội dung dùng nền `surface-container-lowest` (`#FFFFFF`) đặt trên nền trang `surface` (`#F7FAF8`) với viền `1px` mảnh. Tuyệt đối không dùng hiệu ứng glassmorphism hay bóng đổ đậm.

## Shapes

Bo góc vừa phải, mang lại cảm giác thân thiện nhưng vẫn giữ sự chỉn chu của phần mềm nghiệp vụ y tế:
- `sm` (4px): Ô nhập liệu nhỏ, thẻ tóm tắt khung giờ.
- `DEFAULT` (8px): Nút bấm, ô chọn khung giờ khám, input form.
- `md` (12px): Thẻ bác sĩ, thẻ yêu cầu, bảng danh sách.
- `lg` (16px): Khung tóm tắt đặt lịch, hộp thoại xác nhận.
- `full` (9999px): Nhãn trạng thái (Status Badge), avatar bác sĩ.

```yaml
rounded:
  sm: 4px
  DEFAULT: 8px
  md: 12px
  lg: 16px
  xl: 24px
  full: 9999px
```

## Motion & Micro-interaction

Chuyển động nhanh, dứt khoát và không gây phân tâm. Chỉ tạo hiệu ứng trên `opacity`, `transform` và màu sắc; tôn trọng `prefers-reduced-motion`. Không có animation lặp vô hạn.

```yaml
motion:
  state-change:
    duration: 120ms
    delay: 0ms
    timingFunction: ease-out
  surface-enter:
    duration: 200ms
    delay: 0ms
    timingFunction: cubic-bezier(0.2, 0, 0, 1)
  surface-exit:
    duration: 150ms
    delay: 0ms
    timingFunction: cubic-bezier(0.3, 0, 1, 1)
```

## Voice & Content Strategy

- **Giọng văn:** Lịch sự, rõ ràng, trung lập và minh bạch. Tránh từ ngữ tiếp thị phóng đại hoặc hứa hẹn tuyệt đối.
- **Quy tắc đặt tên & viết hoa:** Viết hoa chữ cái đầu câu (Sentence case) cho tiêu đề, nút bấm và nhãn trạng thái. Tên bác sĩ ghi đầy đủ học vị viết tắt chuẩn (`BS. CKII`, `ThS. BS.`).
- **Thuật ngữ thống nhất:**
  - Dùng **"Yêu cầu đặt lịch"** (không dùng "Đơn hàng" hay "Vé khám") trước khi được nhân viên duyệt.
  - Dùng **"Gửi yêu cầu đặt lịch"** (không dùng "Đặt lịch ngay" hay "Xác nhận đặt") ở phía người đặt để phản ánh đúng quy tắc: gửi yêu cầu chưa đồng nghĩa với lịch đã được xác nhận.
  - Ba trạng thái chuẩn cố định: **"Chờ xác nhận"**, **"Đã xác nhận"**, **"Đề nghị thời gian khác"**.
- **Định dạng ngày giờ & mã:** Giờ dùng định dạng 24h (`08:30`, `14:00`), ngày dùng `DD/MM/YYYY` (`22/11/2026`), mã yêu cầu dùng tiền tố `YC-` (`YC-1042`).
- **Quy tắc thiết kế dùng chung (Shared Design Rules):**
  1. Mọi trạng thái phải hiển thị đồng thời **Icon + Nhãn chữ + Màu nền/chữ tương phản cao**.
  2. Mỗi thẻ hoặc dòng dữ liệu chỉ có **1 thao tác chính** (Primary) và tối đa 1–2 thao tác phụ rõ ràng.
  3. Không ẩn thông tin quan trọng (tên bác sĩ, ngày giờ đề xuất, trạng thái) vào tooltip.
  4. Luôn hiển thị thông báo giải thích quy trình xác nhận ngay tại điểm gửi yêu cầu.

## Components

Component implementations live as individual HTML sticker sheet files in
`components/`. Each file contains the canonical, styled HTML components with
`<!-- COMPONENT: name -->` comment markers. Read each file before use.

- **Badge** → `@components/badge.html`: `badge-numeric`, `badge-dot`
- **Button** → `@components/button.html`: `button-primary`, `button-icon`, `button-with-icon`
- **Card** → `@components/card.html`: `card-elevated`, `card-action`, `card-interactive`, `card-interactive-2`
- **Table** → `@components/table.html`: `table-standard`, `table-interactive`, `table-selectable`
- **Tabs** → `@components/tabs.html`: `tabs-horizontal`, `tabs-with-icon`
