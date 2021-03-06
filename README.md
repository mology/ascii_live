# 🐸ASCII字符画视频流

> 自动实时转换视频到ASCII字符画视频

![](demo.gif)

只是一个小demo

灵感来自 https://github.com/HFO4/plus1s.live

[演示地址：https://xmader.github.io/ascii_live/](https://xmader.github.io/ascii_live/)

* 点一下字符画就能像视频一样播放/暂停

* 字符画可以像正常的文本一样复制/粘贴 <!-- 使用 CTRL-A 进行全选后复制 -->

* 滋磁调整ASCII字符画视频的字号 (字号越小分辨率越高，占用的CPU百分比也就越高)

* 滋磁播放本地视频 (转换完全在本地进行，视频不会上传到任何服务器，所以不必担心隐私问题)
<!-- 理论上滋磁浏览器<video>标签所滋磁的所有视频格式 https://developer.mozilla.org/zh-CN/docs/Web/HTML/Supported_media_formats ，包括但不限于mp4、webm和ogv -->

* 滋磁在ASCII字符画视频的左侧/上方同时显示转换前的原始视频

* 全屏观看效果更佳

* **v1.3.0新增** 打开控制台也能看到ASCII字符画视频 (目前只在字号为16px时可用) (仅在Firefox中测试通过) <!-- 同时输出到控制台 -->

## 这是如何实现的？

使用了canvas作为过渡，具体实现可以查看[源码](https://github.com/Xmader/ascii_live/blob/master/index.js)。

```
原始视频 => canvas => ASCII字符画视频
```

转换视频不依赖任何服务器，完全在你的浏览器中进行，离线也可以使用，具体转换效率取决于你的CPU性能。

## License

MIT
