# random-acg-image-api
随机二次元图片

### API 端点：

#### 横屏图片：

- **请求方式**：GET
- **URL**：[`https://api.rulian.us.kg/horizontal`](https://api.rulian.us.kg/horizontal)
- **图片数量**：500张
- **分辨率**：4K - 8K
- **描述**：获取适合横屏显示的高清ACG图片，分辨率从4K到8K。

#### 竖屏图片：

- **请求方式**：GET
- **URL**：[`https://api.rulian.us.kg/vertical`](https://api.rulian.us.kg/vertical)
- **图片数量**：500张
- **分辨率**：2K - 8K
- **描述**：获取适合竖屏显示的高清ACG图片，分辨率从2K到8K。

#### 自适应设备图片：

- **请求方式**：GET
- **URL**：[`https://api.rulian.us.kg/adaptive`](https://api.rulian.us.kg/adaptive)
- **描述**：自动检测设备屏幕方向，提供适合横屏或竖屏的图片。

### 图片来源：
所有图片都来自Pixiv（P站），是我一张一张挑选的，还对部分图片进行了超分辨率处理。

### 图片特点和性能：

- **图片大小**：每张图片的大小在40MB左右。
- **下载速度**：10MB/s的下载速度下，加载速度很快，没有问题。
- **图片数量**：目前有1000张图片，我会持续更新。
- **维护计划**：这个项目应该会一直维护。
