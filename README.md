
# RLS 随机图片 API

RLS 随机图片 API 提供高质量的随机图片，支持多种模式与分辨率，适用于各种设备的图片加载需求。

## 🌟 特点
- **多种模式支持**：横屏、竖屏、自适应。
- **高速存储**：采用高效存储方式，并保证图片质量。
- **图片格式**：AVIF 格式。
- **图片数量**：已收录 7066 张（更新时间：2024/12/14）。
- **分辨率**：提供超高清图片，最大支持 16K。
- **兼容性**：理论上支持任何需要填写图片地址的场景。

---

## 📝 API 端点

### 1. 横屏图片
获取随机横屏图片，分辨率范围：4K - 16K。

```markdown
**API URL**
https://api.rls.ovh/horizontal

**中文路径**
https://api.rls.ovh/横屏
```

---

### 2. 竖屏图片
获取随机竖屏图片，分辨率范围：4K - 12K。

```markdown
**API URL**
https://api.rls.ovh/vertical

**中文路径**
https://api.rls.ovh/竖屏
```

---

### 3. 自适应图片
根据当前设备返回横屏或竖屏图片，适配手机、平板、电脑等设备。

```markdown
**API URL**
https://api.rls.ovh/adaptive

**中文路径**
https://api.rls.ovh/自适应
```

---

## 💻 使用示例

### HTML 示例
```html
<img src="https://api.rls.ovh/adaptive">
```

### JavaScript 示例
```javascript
fetch('https://api.rls.ovh/adaptive')
  .then(response => response.blob())
  .then(blob => {
    const img = document.createElement('img');
    img.src = URL.createObjectURL(blob);
    document.body.appendChild(img);
  });
```

### CSS 背景图片
```css
.background {
  background-image: url('https://api.rls.ovh/adaptive');
  background-size: cover;
  background-position: center;
}
```

### 推荐使用方式
```css
/* 默认使用竖屏图片 */
.background {
    background-image: url('https://api.rls.ovh/vertical');
    background-size: cover;
    background-position: center;
}

/* 当分辨率宽度大于高度时，使用横屏图片 */
@media (orientation: landscape) {
    .background {
        background-image: url('https://api.rls.ovh/horizontal');
    }
}
```

---

## ⚠️ 注意事项
1. **仅供个人学习研究使用**，禁止用于商业用途。
2. **请求频率限制**：同一 IP 最多 3 次/秒，请合理使用 API。
3. **网络工具限制**：VPN 等工具可能导致 API 加载失败。可[点击此处查询 IP](https://api.rls.ovh/)。

---

## 📈 调用统计
- 累计调用次数：114,847

