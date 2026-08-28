# Hướng Dẫn Thay Ảnh Cho Website LUMI DOOR

## Cấu trúc thư mục ảnh

```
assets/images/
├── banners/
│   └── banner-1.svg      ← Ảnh banner chính (1920x800)
├── categories/
│   ├── cua-soi-chi.svg   ← Ảnh danh mục Cửa Soi Chỉ
│   ├── cua-canh-phang.svg ← Ảnh danh mục Cửa Cánh Phẳng
│   ├── cua-vom.svg       ← Ảnh danh mục Cửa Vòm
│   └── cua-nha-ve-sinh.svg ← Ảnh danh mục Cửa Nhà Vệ Sinh
└── products/
    ├── lumi-sc-01.svg    ← Ảnh sản phẩm mẫu
    └── lumi-cp-02.svg    ← Ảnh sản phẩm mẫu
```

## Cách thay ảnh

### 1. Thay ảnh Banner (Hero Section)

**File:** `assets/images/banners/banner-1.svg`

**Kích thước khuyến nghị:** 1920x800px hoặc lớn hơn

**Cách thay:**
- Chuẩn bị ảnh banner thực tế của LUMI DOOR
- Đặt tên: `banner-1.jpg` (hoặc .png, .webp)
- Di chuyển vào thư mục: `assets/images/banners/`
- Mở file `index.html` và tìm đến phần Hero Slider
- Thay thế dòng:
```html
<img src="assets/images/banners/banner-1.svg" alt="LUMI DOOR" class="absolute inset-0 w-full h-full object-cover">
```
thành:
```html
<img src="assets/images/banners/banner-1.jpg" alt="LUMI DOOR" class="absolute inset-0 w-full h-full object-cover">
```

### 2. Thay ảnh Danh Mục Sản Phẩm

**Files:**
- `assets/images/categories/cua-soi-chi.svg`
- `assets/images/categories/cua-canh-phang.svg`
- `assets/images/categories/cua-vom.svg`
- `assets/images/categories/cua-nha-ve-sinh.svg`

**Kích thước khuyến nghị:** 600x750px (tỷ lệ 4:5)

**Cách thay:**
- Chuẩn bị 4 ảnh đại diện cho mỗi dòng sản phẩm
- Đặt tên theo quy ước:
  - `cua-soi-chi.jpg`
  - `cua-canh-phang.jpg`
  - `cua-vom.jpg`
  - `cua-nha-ve-sinh.jpg`
- Di chuyển vào thư mục: `assets/images/categories/`
- Mở file `index.html` và thay thế các dòng `<img src="assets/images/categories/xxx.svg"` thành đường dẫn ảnh thực

### 3. Thay ảnh Sản Phẩm Chi Tiết

**Files:** `assets/images/products/*.svg`

**Kích thước khuyến nghị:** 400x400px hoặc lớn hơn

**Cách thay:**
- Chuẩn bị ảnh sản phẩm thực tế
- Đặt tên theo mã sản phẩm: `lumi-sc-01.jpg`, `lumi-cp-02.jpg`, v.v.
- Di chuyển vào thư mục: `assets/images/products/`
- Cập nhật đường dẫn trong HTML

## Lưu ý quan trọng

1. **Định dạng ảnh:** Nên sử dụng định dạng `.jpg` hoặc `.webp` để tối ưu kích thước file
2. **Chất lượng ảnh:** Nên nén ảnh trước khi upload để website load nhanh hơn
3. **Kích thước đề xuất:**
   - Banner: 1920x800px
   - Danh mục: 600x750px
   - Sản phẩm: 400x400px
   - Projects: 800x600px

## Ví dụ nhanh

Sau khi có ảnh thực, chỉ cần:

1. Copy ảnh vào thư mục tương ứng
2. Đổi đuôi file từ `.svg` thành `.jpg` trong code HTML

Hoặc giữ nguyên file `.svg` nếu bạn đã tạo ảnh vector.
