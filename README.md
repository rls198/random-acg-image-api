## 📝 API端点

1. 横屏图片
**GET** - 获取随机横屏图片，分辨率4K-16K
```http
https://api.rls.ovh/horizontal

# 中文路径
https://api.rls.ovh/横屏

竖屏图片
GET - 获取随机竖屏图片，分辨率4K-12K

httpCopyhttps://api.rls.ovh/vertical

# 中文路径
https://api.rls.ovh/竖屏

自适应图片
GET - 根据当前设备返回横或竖图，例如手机、平板、电脑等

httpCopyhttps://api.rls.ovh/adaptive

# 中文路径
https://api.rls.ovh/自适应
Copy
这样编号就是连续的，看起来更清晰和专业。需要我把完整的 README 都按这种格式重新发给你吗？ CopyRetryC还是不行完整的发给我使用发代码的方式不要这样发送EditmarkdownCopy# RLS的随机图片API

累计调用次数：114,847

## 🌟 特点

- 支持横/竖/自适应三种模式，采用高速存储，并保证图片质量
- 图片为AVIF格式，已收录7066张，更新时间24/12/14  
- 提供超高清图片，最大16k分辨率
- 理论上需要填写图片地址的地方都可使用

## 📝 API端点

1. 横屏图片
**GET** - 获取随机横屏图片，分辨率4K-16K
```http
https://api.rls.ovh/horizontal

# 中文路径
https://api.rls.ovh/横屏

竖屏图片
GET - 获取随机竖屏图片，分辨率4K-12K

httpCopyhttps://api.rls.ovh/vertical

# 中文路径
https://api.rls.ovh/竖屏

自适应图片
GET - 根据当前设备返回横或竖图，例如手机、平板、电脑等

httpCopyhttps://api.rls.ovh/adaptive

# 中文路径
https://api.rls.ovh/自适应
💻 使用示例
HTML 使用
htmlCopy<img src="https://api.rls.ovh/adaptive">
JavaScript 使用
javascriptCopyfetch('https://api.rls.ovh/adaptive')
  .then(response => response.blob())
  .then(blob => {
    const img = document.createElement('img');
    img.src = URL.createObjectURL(blob);
    document.body.appendChild(img);
});
CSS 背景使用
cssCopy.background {
  background-image: url('https://api.rls.ovh/adaptive');
  background-size: cover;
  background-position: center;
}
推荐使用
cssCopy/* 默认使用竖图 */
.background {
    background-image: url('https://api.rls.ovh/vertical');
    background-size: cover;
    background-position: center;
}

/* 当前分辨率宽大于高时，使用横图 */
@media (orientation: landscape) {
    .background {
        background-image: url('https://api.rls.ovh/horizontal');
    }
}
⚠️ 注意事项

仅供个人学习研究使用，禁止用于商业用途
同一IP请求频率限制为3次/秒，请合理使用API
VPN等工具可能会影响API无法加载，点击IP查询
