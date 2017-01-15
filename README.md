# uglify-fend-p6
## index.html ，优化 CRP

### 如何打开和测速
1. 复制网址: `https://poblue.github.io/uglify-fend-p6/`
2. 打开 [pageSpeed][1] 粘贴上面的网址
3. 按 `分析` 按钮就能够测速了


### 优化的地方
- 异步加载 字体 ，不阻塞生成
- 内联 `style.css`
- 压缩 *图片* 和压缩到合适的尺寸
- 加了关键字 `asyn` 让非关键的 JS 不阻塞
- 为 print.css 加了 media ，让它只在打印的时候阻塞，其它时候不阻塞


## pizza.html , 60 FPS


### 如何运行和测速
1. 用浏览器打开 `views/pizza.html`
2. 打开浏览器的 `Console` 
3. 观察 `Console` 里的信息


### 优化的地方
- 添加使用 `requestFrame()`
- 解决强制布局
- 根据屏幕大小生成适合大小的 披萨 数
- 背景披萨的移动，使用 `transform` 而不是改 `left` 
- 使用  `getElementById()` 和 `getElementsByClassName()` 替代 `querySelectorAll()`
- 设置 `#movingPizzas1` 的 `style` 为 `position: fixed;`, 目的是：令得 披萨 都钉住在页面里



[1]:	https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fpoblue.github.io%2Fuglify-fend-p6%2F&tab=mobile "pageSpeed"