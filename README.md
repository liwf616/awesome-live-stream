## 学习资料快速链接

* [fmp4实现开源方式]（https://github.com/axiomatic-systems/Bento4）
* [fmp4 nginx实现]（https://github.com/kaltura/nginx-vod-module）
* [dash相关介绍] （https://bitmovin.com/dynamic-adaptive-streaming-http-mpeg-dash/）
* [hls vs dash] (https://www.vidbeo.com/blog/hls-vs-dash）
* [fmp4开源 shaka-packager] （https://github.com/google/shaka-packager/commit/4891d9a6bf96f3655a7df4b908f96cc036a8c51b）
* [nginx rtmp -> dash] (https://github.com/arut/nginx-rtmp-module)
* [nginx ts->dash] (https://github.com/arut/nginx-ts-module)
* [mp4协议介绍。学好 MP4，让直播更给力](https://www.villainhr.com/page/2017/08/21/%E5%AD%A6%E5%A5%BD%20MP4%EF%BC%8C%E8%AE%A9%E7%9B%B4%E6%92%AD%E6%9B%B4%E7%BB%99%E5%8A%9B）


## 通用工具

* [dash 播放工具]（http://reference.dashif.org/dash.js/nightly/samples/dash-if-reference-player/index.html#）
* [hls fmp4播放地址]（https://bitmovin.com/hls-news-wwdc-2016/）
* [mp4box 工具]（https://gpac.wp.imt.fr/mp4box/dash/）


##  协议草案

* [hls 最新的协议（cbcs）] （https://tools.ietf.org/html/rfc8216）

* [mp4 规范, 亚马逊的fmp4实现参照这个方案] (http://l.web.umkc.edu/lizhu/teaching/2016sp.video-communication/ref/mp4.pdf)


## 常用的命令

1. 将ss.mp4切割成fragment mp4。

```
mp4box -dash 5000 -frag 5000 -rap -frag-rap -profile dashavc264:live ss.mp4 -out ss_dash.mpd
```

2. qt实现的mp4分析工具

```
https://github.com/ksvc/MediaParser
```

3. mp4dump工具

