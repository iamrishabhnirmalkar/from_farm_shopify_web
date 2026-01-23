# Rishu Custom Sections - Documentation

## 📋 Table of Contents
- [Hero Banner Section](#hero-banner-section)
- [Announcement Bar Section](#announcement-bar-section)
- [Image Specifications](#image-specifications)
- [Optimization Guidelines](#optimization-guidelines)

---

## 🎨 Hero Banner Section

### Image Size Recommendations

#### **For Home Page Banner (Recommended)**

Use the **Auto (Full Image)** height setting with these sizes:

**Desktop/Tablet Image:**
- **Size**: `1920 x 1080px` (16:9 ratio) ✅ **RECOMMENDED**
- **Format**: JPG
- **Max File Size**: 400-500 KB
- **Why**: Shows complete banner without cropping on all devices

**Mobile Image (Optional):**
- **Size**: `1080 x 1080px` (1:1 square) ✅ **RECOMMENDED FOR MOBILE**
- **Alternative**: `800 x 1200px` (2:3 portrait)
- **Format**: JPG
- **Max File Size**: 250-300 KB
- **Why**: Better composition for mobile screens

> **💡 Pro Tip**: Create ONE banner at 1920x1080px for desktop. The auto height mode will show the complete image without any cropping. Optionally add a square (1080x1080) version for mobile if you want different composition.

---

#### Alternative Sizes (For Fixed Height Mode)

If using fixed viewport heights (60vh, 80vh, etc.):

**Desktop Images:**
- **Standard**: `1920 x 1080px` (16:9 ratio)
- **Minimum**: `1600 x 900px`
- **Maximum**: `3840 x 2160px` (4K)
- **Aspect Ratio**: 16:9 (landscape)

**Mobile Images (Optional):**
- **Recommended**: `800 x 1200px` (2:3 ratio)
- **Minimum**: `600 x 900px`
- **Maximum**: `1200 x 1800px`
- **Aspect Ratio**: 2:3 (portrait) or 1:1 (square)

> **Note**: The section only supports **2 image uploads**:
> 1. **Desktop Image** (required) - Used for desktop AND tablet
> 2. **Mobile Image** (optional) - Used only for mobile devices
> 
> Tablets automatically use the desktop image at an optimized size.

### File Format Guidelines

| Format | Best For | Max File Size | Quality |
|--------|----------|---------------|---------|
| **JPG** | Photos, gradients, complex images | 300-500 KB | 80-85% |
| **PNG** | Graphics, logos, transparency needed | 200-400 KB | High |
| **WebP** | Modern browsers (auto-converted by Shopify) | 200-300 KB | High |

### Height Settings

The hero banner uses different height modes:

| Mode | Mobile | Tablet | Desktop | Best For |
|------|--------|--------|---------|----------|
| **Auto (Default)** ✅ | Full image | Full image | Full image | **Home page banners - shows complete 1920x1080 image** |
| 60vh | 60% screen | 60% screen | 60% screen | Small hero sections |
| 70vh | 60% screen | 70% screen | 70% screen | Medium sections |
| 80vh | 60% screen | 70% screen | 80% screen | Large hero sections |
| 90vh | 60% screen | 70% screen | 90% screen | Extra large sections |
| 100vh | 60% screen | 70% screen | 100% screen | Full screen takeover |

> **Recommended**: Use **Auto** mode for home page banners to show the complete image without cropping!

---

## 📢 Announcement Bar Section

### Text Recommendations
- **Character Limit**: 50-80 characters per announcement
- **Number of Announcements**: 3-5 for best performance
- **Font Size**: Auto-adjusts (14px desktop, 13px mobile)

---

## 🖼️ Image Specifications

### Single Responsive Image (Recommended)

**Best Practice**: Use ONE image that works across all devices

#### Specifications:
- **Size**: `1920 x 1080px`
- **Format**: JPG (for photos) or PNG (for graphics)
- **File Size**: Under 500 KB
- **Safe Zone**: Keep important content in center 60% of image

#### Why Single Image?
✅ Simpler to manage  
✅ Better performance (fewer HTTP requests)  
✅ Shopify auto-optimizes for all devices  
✅ Automatic WebP conversion  

### Device-Specific Images (Advanced)

**When to Use**:
- Text in images needs different sizing
- Important content gets cropped on mobile
- Different messaging for mobile vs desktop

#### Desktop Image:
```
Size: 1920 x 1080px
Format: JPG/PNG
Max File Size: 500 KB
```

#### Mobile Image:
```
Size: 800 x 1200px (portrait)
OR: 1080 x 1080px (square)
Format: JPG/PNG
Max File Size: 300 KB
```

---

## ⚡ Optimization Guidelines

### Before Upload

#### 1. Resize Images
Use these dimensions based on your needs:

| Device | Width | Height | Use Case |
|--------|-------|--------|----------|
| Desktop | 1920px | 1080px | Standard hero banner |
| Desktop (Large) | 2560px | 1440px | High-res displays |
| Mobile | 800px | 1200px | Portrait orientation |
| Mobile (Square) | 1080px | 1080px | Square format |

#### 2. Compress Images

**Recommended Tools**:
- **TinyPNG** (https://tinypng.com) - Best for PNG
- **Squoosh** (https://squoosh.app) - Advanced options
- **ImageOptim** (Mac) - Batch processing
- **JPEG Optimizer** - For JPG files

**Target File Sizes**:
- Desktop images: 300-500 KB
- Mobile images: 200-300 KB
- Thumbnail/small images: Under 100 KB

#### 3. Choose Right Format

```
Photos/Complex Images → JPG (80-85% quality)
Graphics/Logos → PNG-8 or PNG-24
Transparency Needed → PNG-24
Modern Browsers → WebP (Shopify auto-converts)
```

### Shopify Automatic Optimization

Shopify automatically:
- ✅ Generates multiple sizes (375px, 750px, 1100px, 1500px, etc.)
- ✅ Converts to WebP for supported browsers
- ✅ Serves appropriate size based on device
- ✅ Lazy loads images below the fold
- ✅ Uses CDN for fast delivery

### Performance Best Practices

#### Image Content Guidelines:
1. **Safe Zone**: Keep text/logos in center 60% of image
2. **Focal Point**: Place main subject in center
3. **Avoid Small Text**: Text should be readable at mobile size
4. **High Contrast**: Ensure text overlays are readable

#### Slider Settings:
- **Number of Slides**: 3-5 slides maximum
- **Autoplay Speed**: 5-7 seconds per slide
- **Animation**: Use "Fade" for best performance
- **Preload**: First slide loads with high priority

#### File Naming:
```
✅ Good: hero-banner-summer-sale.jpg
✅ Good: mobile-hero-promo-2024.jpg
❌ Bad: IMG_1234.jpg
❌ Bad: banner final FINAL v3.png
```

---

## 📐 Image Dimension Calculator

### Aspect Ratio Guide

| Ratio | Desktop Example | Mobile Example | Best For |
|-------|----------------|----------------|----------|
| 16:9 | 1920 x 1080 | 800 x 450 | Landscape, cinematic |
| 4:3 | 1600 x 1200 | 800 x 600 | Traditional, balanced |
| 2:3 | 1080 x 1620 | 800 x 1200 | Portrait, mobile-first |
| 1:1 | 1080 x 1080 | 1080 x 1080 | Square, social media |

### Quick Reference

```
Desktop Hero Banner:
- Standard: 1920 x 1080px (16:9)
- Wide: 2560 x 1080px (21:9)
- 4K: 3840 x 2160px (16:9)

Mobile Hero Banner:
- Portrait: 800 x 1200px (2:3)
- Square: 1080 x 1080px (1:1)
- Landscape: 800 x 450px (16:9)
```

---

## 🎯 Optimization Checklist

Before uploading images to Shopify:

- [ ] Resized to recommended dimensions
- [ ] Compressed to target file size
- [ ] Correct format chosen (JPG/PNG)
- [ ] Alt text prepared for accessibility
- [ ] File named descriptively
- [ ] Tested on multiple devices
- [ ] Important content in safe zone
- [ ] Text is readable at mobile size

---

## 🔧 Troubleshooting

### Image Looks Blurry
- Upload larger image (try 2560 x 1440px)
- Use higher quality JPG (90% instead of 80%)
- Check if image was compressed too much

### Image Loads Slowly
- Reduce file size (compress more)
- Use JPG instead of PNG for photos
- Reduce image dimensions if too large

### Image Cropped on Mobile
- Use mobile-specific image
- Keep important content in center
- Test on actual mobile devices

### Colors Look Different
- Save in sRGB color space
- Avoid CMYK (for print)
- Use consistent color profile

---

## 📞 Support

For issues or questions about the Rishu custom sections:
1. Check this README first
2. Review the walkthrough.md file
3. Test in Shopify theme editor preview

---

**Version**: 1.0  
**Last Updated**: January 2026  
**Author**: Rishabh Nirmalkar
