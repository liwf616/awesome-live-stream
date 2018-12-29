## 学习资料快速链接

* [fmp4实现开源方式]（https://github.com/axiomatic-systems/Bento4）
* [fmp4 nginx实现]（https://github.com/kaltura/nginx-vod-module）
* [dash相关介绍] （https://bitmovin.com/dynamic-adaptive-streaming-http-mpeg-dash ）
* [hls vs dash] (https://www.vidbeo.com/blog/hls-vs-dash）
* [fmp4开源 shaka-packager] （https://github.com/google/shaka-packager/commit/4891d9a6bf96f3655a7df4b908f96cc036a8c51b）
* [nginx rtmp -> dash] (https://github.com/arut/nginx-rtmp-module)
* [nginx ts->dash] (https://github.com/arut/nginx-ts-module)
* [mp4协议介绍。学好 MP4，让直播更给力](https://www.villainhr.com/page/2017/08/21/%E5%AD%A6%E5%A5%BD%20MP4%EF%BC%8C%E8%AE%A9%E7%9B%B4%E6%92%AD%E6%9B%B4%E7%BB%99%E5%8A%9B）
* [媒体文件格式分析之FMP4] (https://github.com/liwf616/awesome-dash/wiki)
* [rtc调研报告](https://github.com/liwf616/awesome-live-stream/wiki/rtc_research)


## 通用工具

* [dash 播放工具]（http://reference.dashif.org/dash.js/nightly/samples/dash-if-reference-player/index.html#）
* [hls fmp4播放地址]（  https://bitmovin.com/hls-news-wwdc-2016 ）
* [mp4box 工具]（https://gpac.wp.imt.fr/mp4box/dash/）
* [hls.js 播放工具]（http://video-dev.github.io/hls.js/demo/）
* [mp4box 工具]（https://gpac.wp.imt.fr/mp4box/dash/）


## 协议规范

* [hls 最新的协议（cbcs）] （https://tools.ietf.org/html/rfc8216）

* [mp4 规范, 亚马逊的fmp4实现参照这个方案] (http://l.web.umkc.edu/lizhu/teaching/2016sp.video-communication/ref/mp4.pdf)

* [HLS对4K技术的支持] (http://www.streamingmedia.com/Articles/Editorial/Featured-Articles/Apple-Got-It-Wrong-Encoding-Specs-for-HEVC-in-HLS--121878.aspx)

* [HLS对HDR技术的支持] (https://streaminglearningcenter.com/blogs/apple-updates-hls-authoring-spec-4k-hdr.html)

* [HLS vs DASH vs HDS vs MSS] (https://bitmovin.com/mpeg-dash-vs-apple-hls-vs-microsoft-smooth-streaming-vs-adobe-hds/)

## 音视频峰会

* [WWDC17 – HEVC with HLS] (https://bitmovin.com/wwdc17-hevc-hls-apple-just-announced-feature-support-box/)

* [WWDC16: HLS Supports Fragmented MP4] (https://bitmovin.com/hls-news-wwdc-2016/)

## 常用的命令

1. 用mp4box将ss.mp4切割成fragment mp4。

```
mp4box -dash 5000 -frag 5000 -rap -frag-rap -profile dashavc264:live ss.mp4 -out ss_dash.mpd
```

2. 用mp4将ss.mp4切割成fragment mp4。

```
1. mp4fragment ss.mp4 ss_fragment.mp4
2. mp4dash --use-segment-timeline ss_fragment.mp4
```

3. qt实现的mp4分析工具

```
https://github.com/ksvc/MediaParser
```

4. mp4dump工具

## 播放地址
* [HLS fmp4 h264] (https://bitdash-a.akamaihd.net/content/MI201109210084_1/m3u8s-fmp4/f08e80da-bf1d-4e3d-8899-f0f6155f6efa.m3u8)
* [HLS fmp4 h265] (http://bitmovin-a.akamaihd.net/content/dataset/multi-codec/hevc/stream_fmp4.m3u8)

