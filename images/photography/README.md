# 摄影作品 - 星空主题 / Photography - Starry Sky

## 📸 当前作品 / Current Photos

本文件夹包含星空主题的摄影作品。

This folder contains starry sky themed photography.

```
starry-sky/
├── starry1.jpg    # 星空之夜 / Starry Night
└── starry2.jpg    # 璀璨星河 / Brilliant Starry Sky
```

## 🎨 如何添加新照片 / How to Add New Photos

### 1. 添加照片文件
将新照片放入 `starry-sky/` 文件夹中。

### 2. 更新网站代码
在 `index.html` 文件中找到 `photos` 数组（约第919行），添加照片信息：

```javascript
{
  src: 'images/photography/starry-sky/your-photo.jpg',
  category: 'starry-sky',
  title: { zh: '您的标题', en: 'Your Title' },
  location: { zh: '拍摄地点', en: 'Location' },
  date: '2026'
}
```

### 3. 照片要求
- **格式**：JPG, PNG, WEBP
- **尺寸**：建议宽度 ≥ 1200px
- **大小**：建议 < 2MB

## ✨ 功能特性 / Features

- 响应式网格布局
- 灯箱查看大图
- 键盘导航（←/→ 切换，ESC 关闭）
- 中英文双语支持
- 悬停显示照片信息
