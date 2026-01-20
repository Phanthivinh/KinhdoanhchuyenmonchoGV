# 🎬 Video Storyboard - Nền Trang Chủ

**Tên video:** Homepage Background Loop  
**Thời lượng:** 5-7 giây (loop vô hạn)  
**Độ phân giải:** 1920x1080 (Full HD)  
**Frame rate:** 60fps  
**Định dạng:** MP4 / WebM  

---

## Bảng Màu

| Màu | Hex | Sử dụng |
|-----|-----|---------|
| Xanh dương chính | #023e8a | Elements, shapes |
| Xanh navy | #03045e | Accents |
| Trắng | #ffffff | Background |
| Xanh nhạt | #90cdf4 | Highlights, glow |

---

## Mô Tả Tổng Quan

Video nền trang chủ với chuyển động chậm, mượt mà tạo cảm giác yên bình và truyền cảm hứng. Không có chữ, phù hợp để đặt text overlay phía trên.

---

## Storyboard Chi Tiết

### Frame 0:00 - 0:02 | Opening

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│     ○ ○            Nền trắng sạch                          │
│         ○                                                   │
│   ○         ○      Các hình tròn xanh (#023e8a)             │
│       ○           float nhẹ nhàng từ dưới lên              │
│                                                             │
│              ○        Độ mờ: 40-80%                         │
│   ○                   Soft blur edges                       │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

**Animation:**
- Circles float upward slowly (0.5px/frame)
- Subtle rotation (0.1deg/frame)
- Slight scale breathing (98%-102%)

---

### Frame 0:02 - 0:04 | Transition

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   ┌──┐  ○        Geometric shapes xuất hiện                │
│   └──┘      ◇                                               │
│        △         Squares, diamonds, triangles               │
│   ○         ┌──┐  màu xanh với viền bo tròn                │
│             └──┘                                            │
│      ◇           Fade in với soft glow                      │
│   △                                                         │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

**Animation:**
- New shapes fade in (opacity 0 → 60%)
- Gentle floating movement
- Subtle parallax effect (different speeds)

---

### Frame 0:04 - 0:06 | Peak

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   ○  ┌──┐  ◇     Tất cả elements di chuyển                 │
│      └──┘                                                   │
│        △    ○    Tạo pattern flowing                        │
│   ◇         ┌──┐                                            │
│     ○       └──┘  Light particles (#90cdf4)                 │
│        . . . .    xuất hiện và bay lên                      │
│   △     . . .                                               │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

**Animation:**
- Small light particles appear
- All elements in gentle motion
- Soft ambient glow effect

---

### Frame 0:06 - 0:07 | Loop Transition

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│     ○ ○            Elements fade và                         │
│         ○          reposition để match                      │
│   ○         ○      frame đầu tiên                          │
│       ○                                                     │
│                    Seamless loop                            │
│              ○                                              │
│   ○                                                         │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

**Animation:**
- Shapes gradually return to starting positions
- Smooth crossfade to beginning
- Perfect loop point

---

## Thông Số Kỹ Thuật

### Cài Đặt Render

```
Resolution: 1920 x 1080 px
Frame Rate: 60 fps
Duration: 7 seconds (420 frames)
Codec: H.264 (MP4) + VP9 (WebM)
Bitrate: 8-10 Mbps
Loop: Seamless
Audio: None
```

### CSS Implementation

```css
.hero-video-background {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: -1;
  opacity: 0.4; /* Để không overwhelm content */
}
```

### HTML Structure

```html
<section class="hero">
  <video class="hero-video-background" autoplay muted loop playsinline>
    <source src="hero-bg.webm" type="video/webm">
    <source src="hero-bg.mp4" type="video/mp4">
  </video>
  <div class="hero-content">
    <!-- Text overlay here -->
  </div>
</section>
```

---

## Tools Đề Xuất

1. **After Effects** - Animation chuyên nghiệp
2. **Lottie/Bodymovin** - Xuất ra web animation
3. **Rive** - Interactive vector animation
4. **CSS Animation** - Lightweight alternative

---

## Lưu Ý

- ✅ Không có text trong video
- ✅ Chuyển động chậm, không gây distraction
- ✅ Loop mượt, không có điểm nhảy
- ✅ Optimize file size cho web
- ✅ Fallback image cho slow connections
