# uglify-fend-p6
## index.html ，优化 CRP

### 如何打开
网页链接：[https://poblue.github.io/uglify-fend-p6/][1]
### 优化的地方
- 异步加载 字体 ，不阻塞生成
- 内联 `style.css`
- 压缩 *图片* 和压缩到合适的尺寸
- 加了关键字 `asyn` 让非关键的 JS 不阻塞
- 为 print.css 加了 media ，让它只在打印的时候阻塞，其它时候不阻塞


## pizza.html , 60 FPS

### 优化的地方
- 添加使用 `requestFrame()`
- 解决强制布局
- 根据屏幕大小生成适合大小的 披萨 数
- 背景披萨的移动，使用 `transform` 而不是改 `left` 



[1]:	https://poblue.github.io/uglify-fend-p6/