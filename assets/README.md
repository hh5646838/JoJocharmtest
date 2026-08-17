# Assets 文件夹说明

本文件夹存放所有图片资源，供 `index.html` 和 `config.json` 引用。

## 必需的图片文件

### 1. 头像
- **文件名**: `avatar.png` (或 `.jpg`)
- **用途**: 首页浮动头像
- **建议尺寸**: 200x200px 或更大（正方形）
- **config.json 对应字段**: `profile.avatar`

### 2. 公众号二维码
- **文件名**: `qrcode.png` (或 `.jpg`)
- **用途**: 弹窗中的公众号二维码
- **建议尺寸**: 400x400px 或更大（正方形）
- **config.json 对应字段**: `profile.wechatQrCode`

### 3. 摄影集封面
- **文件名**: `photo.jpg` (或 `.png`)
- **用途**: "我的作品"章节 - 摄影集模块背景图
- **建议尺寸**: 1200x400px（横向，3:1 比例）
- **config.json 对应字段**: `sections[0].modules[0].image`

### 4. 旅行日记封面
- **文件名**: `travel.jpg` (或 `.png`)
- **用途**: "我的作品"章节 - 旅行日记模块背景图
- **建议尺寸**: 600x800px（竖向，3:4 比例）
- **config.json 对应字段**: `sections[0].modules[1].image`

### 5. 咖啡时光封面
- **文件名**: `coffee.jpg` (或 `.png`)
- **用途**: "我的作品"章节 - 咖啡时光模块背景图
- **建议尺寸**: 400x400px（正方形，1:1 比例）
- **config.json 对应字段**: `sections[0].modules[2].image`

### 6. 阅读清单封面
- **文件名**: `book.jpg` (或 `.png`)
- **用途**: "我的作品"章节 - 阅读清单模块背景图
- **建议尺寸**: 400x400px（正方形，1:1 比例）
- **config.json 对应字段**: `sections[0].modules[3].image`

### 7. 调酒艺术封面
- **文件名**: `cocktail.jpg` (或 `.png`)
- **用途**: "兴趣爱好"章节 - 调酒艺术模块背景图
- **建议尺寸**: 1200x400px（横向，3:1 比例）
- **config.json 对应字段**: `sections[1].modules[0].image`

### 8. 音乐收藏封面
- **文件名**: `music.jpg` (或 `.png`)
- **用途**: "兴趣爱好"章节 - 音乐收藏模块背景图
- **建议尺寸**: 600x800px（竖向，3:4 比例）
- **config.json 对应字段**: `sections[1].modules[1].image`

### 9. 茶道封面
- **文件名**: `tea.jpg` (或 `.png`)
- **用途**: "兴趣爱好"章节 - 茶道模块背景图
- **建议尺寸**: 400x400px（正方形，1:1 比例）
- **config.json 对应字段**: `sections[1].modules[2].image`

## 使用说明

1. **将图片放入此文件夹**：将上述 9 张图片按文件名放入 `assets/` 文件夹
2. **修改 config.json**：如果使用了不同的文件名，请同步修改 `config.json` 中对应的路径
3. **图片格式**：支持 `.jpg`、`.png`、`.webp` 等常见格式
4. **图片优化**：建议使用压缩工具优化图片大小，提升加载速度

## 从 CDN 迁移到本地

如果你之前使用的是 CDN 链接（如本项目原始版本），可以：

1. 下载 CDN 图片到本地 `assets/` 文件夹
2. 修改 `config.json` 中的 URL 为相对路径（如 `assets/avatar.png`）
3. 上传整个项目到 GitHub Pages

## 文件结构示例

```
github-pages/
├── index.html          # 主页面
├── style.css           # 样式文件
├── config.json         # 数据配置
└── assets/             # 图片资源
    ├── avatar.png
    ├── qrcode.png
    ├── photo.jpg
    ├── travel.jpg
    ├── coffee.jpg
    ├── book.jpg
    ├── cocktail.jpg
    ├── music.jpg
    └── tea.jpg
```
