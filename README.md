# 随机二次元图片API

提供了高分辨率的ACG图片，可以根据屏幕方向、分辨率需求和网络运营商进行适配。

---

### API 端点

#### 横屏图片

- **请求方式**：GET
- **URL**：[`https://api.rls.icu/横屏`](https://api.rls.icu/横屏) 或 [`https://api.rls.icu/horizontal`](https://api.rls.icu/horizontal)
- **图片数量**：1000张
- **分辨率**：4K - 10K
- **线路参数**：支持手动指定运营商线路  
  - 电信：`?线路=电信` 或 `?isp=ctcc`
  - 联通：`?线路=联通` 或 `?isp=cucc`
  - 移动：`?线路=移动` 或 `?isp=cmcc`
  - **示例**：`https://api.rls.icu/横屏?线路=联通` 或 `https://api.rls.icu/horizontal?isp=cucc`
  - 自动选择线路：若不指定线路，根据IP地址自动判断运营商。

#### 竖屏图片

- **请求方式**：GET
- **URL**：[`https://api.rls.icu/竖屏`](https://api.rls.icu/竖屏) 或 [`https://api.rls.icu/vertical`](https://api.rls.icu/vertical)
- **图片数量**：1000张
- **分辨率**：2K - 8K
- **线路参数**：支持手动指定运营商线路  
  - 电信：`?线路=电信` 或 `?isp=ctcc`
  - 联通：`?线路=联通` 或 `?isp=cucc`
  - 移动：`?线路=移动` 或 `?isp=cmcc`
  - **示例**：`https://api.rls.icu/竖屏?线路=电信` 或 `https://api.rls.icu/vertical?isp=ctcc`
  - 自动选择线路：若不指定线路，根据IP地址自动判断运营商。

#### 自适应设备图片

- **请求方式**：GET
- **URL**：[`https://api.rls.icu/自适应`](https://api.rls.icu/自适应) 或 [`https://api.rls.icu/adaptive`](https://api.rls.icu/adaptive)
- **描述**：自动检测设备屏幕方向，提供适合横屏或竖屏的图片。
- **线路参数**：支持手动指定运营商线路  
  - 电信：`?线路=电信` 或 `?isp=ctcc`
  - 联通：`?线路=联通` 或 `?isp=cucc`
  - 移动：`?线路=移动` 或 `?isp=cmcc`
  - **示例**：`https://api.rls.icu/自适应?线路=移动` 或 `https://api.rls.icu/adaptive?isp=cmcc`
  - 自动选择线路：若不指定线路，根据IP地址自动判断运营商。

---

### 图片来源
所有图片均源自Pixiv（P站），是我一张一张挑选的，还对部分图片进行了超分辨率处理。
