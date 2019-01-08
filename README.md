## DASH学习资料快速链接

* [fmp4实现开源方式](https://github.com/axiomatic-systems/Bento4)
* [fmp4 nginx实现-nginx-vod-module](https://github.com/kaltura/nginx-vod-module)
* [dash相关介绍](https://bitmovin.com/dynamic-adaptive-streaming-http-mpeg-dash)
* [hls vs dash](https://www.vidbeo.com/blog/hls-vs-dash)
* [fmp4开源-shaka-packager](https://github.com/google/shaka-packager/commit/4891d9a6bf96f3655a7df4b908f96cc036a8c51b)
* [nginx rtmp -> dash](https://github.com/arut/nginx-rtmp-module)
* [nginx ts->dash](https://github.com/arut/nginx-ts-module)
* [mp4协议介绍。学好 MP4，让直播更给力](https://www.villainhr.com/page/2017/08/21/%E5%AD%A6%E5%A5%BD%20MP4%EF%BC%8C%E8%AE%A9%E7%9B%B4%E6%92%AD%E6%9B%B4%E7%BB%99%E5%8A%9B)
* [媒体文件格式分析之FMP4](https://github.com/liwf616/awesome-dash/wiki)

## HLS学习资料快速链接

* [hls之m3u8、ts流格式详解](https://my.oschina.net/u/727148/blog/666824)

## Webrtc学习资料快速链接

* [完整WebRTC技术及应用概要](https://mp.weixin.qq.com/s/EC8Yd74HEoIO2QxJe8-iNQ)
* [rtc调研报告 && webrtc 技术栈学习](https://github.com/liwf616/awesome-live-stream/wiki/rtc_research)
* [webrtc学习之fec模块(ULPFEC Fec && Flex Fec)](https://xjsxjtu.github.io/2017-07-16/LearningWebRTC-fec/)
* [Comparative Study of WebRTC Open Source SFUs
for Video Conferencing](https://www.cosmosoftware.io/publications/andre2018_Comparative_Study_of_SFUs.pdf)
* [Improving Scale and Media Quality with Cascading SFUs](https://webrtchacks.com/sfu-cascading/)
* [Considerations for deploying a geographically distributed video conferencing system](https://jitsi.org/wp-content/uploads/2018/11/ccwc2018-geo.pdf)
* [**支持webrtc人脸实时检测**](https://github.com/justadudewhohacks/face-api.js)
* [webrtc开源项目--medooze(19年必学）](https://github.com/medooze/media-server)
* [webrtc开源项目--pions](https://github.com/pions/webrtc)
* [webrtc开源项目--janus](https://github.com/meetecho/janus-gateway)

## Quic && KCP 学习资料快速链接

* [Nginx支持quic的最新消息](https://trac.nginx.org/nginx/ticket/1057)
* [Golang版本quic<==>quic-go](https://github.com/lucas-clemente/quic-go)

## Nginx学习资料快速链接

* [Nginx 对udp多packet的支持](http://hg.nginx.org/nginx/rev/d27aa9060c95)
* [深入理解Nginx模块开发和架构解析](https://github.com/cjl3080434008/2014/blob/master/read_book/nginx/%E6%B7%B1%E5%85%A5%E7%90%86%E8%A7%A3Nginx%E6%A8%A1%E5%9D%97%E5%BC%80%E5%8F%91%E5%8F%8A%E6%9E%B6%E6%9E%84%E8%A7%A3%E6%9E%90.pdf)
* [Nginx开发从入门到精通](http://tengine.taobao.org/book/)
* [nginx-rtmp-module](https://github.com/arut/nginx-rtmp-module)
* [BLSS(NGINX-based Live Media Streaming Server)](https://github.com/gnolizuh/BLSS)


## 通用工具

* [dash 播放器](http://reference.dashif.org/dash.js/nightly/samples/dash-if-reference-player/index.html)
* [hls fmp4播放器](https://bitmovin.com/hls-news-wwdc-2016)
* [mp4box 工具](https://gpac.wp.imt.fr/mp4box/dash/)
* [hls.js 播放器](http://video-dev.github.io/hls.js/demo/)
* [mp4box 工具](https://gpac.wp.imt.fr/mp4box/dash/)
* [qt实现的mp4分析工具](https://github.com/ksvc/MediaParser)


## 协议规范

* [hls 最新的协议（cbcs）](https://tools.ietf.org/html/rfc8216)

* [mp4 规范(亚马逊的fmp4实现参照这个方案)](http://l.web.umkc.edu/lizhu/teaching/2016sp.video-communication/ref/mp4.pdf)

* [HLS对4K技术的支持](http://www.streamingmedia.com/Articles/Editorial/Featured-Articles/Apple-Got-It-Wrong-Encoding-Specs-for-HEVC-in-HLS--121878.aspx)

* [HLS对HDR技术的支持](https://streaminglearningcenter.com/blogs/apple-updates-hls-authoring-spec-4k-hdr.html)

* [HLS vs DASH vs HDS vs MSS](https://bitmovin.com/mpeg-dash-vs-apple-hls-vs-microsoft-smooth-streaming-vs-adobe-hds/)

## 音视频峰会

* [WWDC17 – HEVC with HLS](https://bitmovin.com/wwdc17-hevc-hls-apple-just-announced-feature-support-box/)

* [WWDC16: HLS Supports Fragmented MP4](https://bitmovin.com/hls-news-wwdc-2016/)

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

4. mp4dump工具

## 播放地址
* [HLS fmp4 h264点播播放地址](https://bitdash-a.akamaihd.net/content/MI201109210084_1/m3u8s-fmp4/f08e80da-bf1d-4e3d-8899-f0f6155f6efa.m3u8)
* [HLS fmp4 h265点播播放地址](http://bitmovin-a.akamaihd.net/content/dataset/multi-codec/hevc/stream_fmp4.m3u8)

[TOC]
