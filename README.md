# Flip 一刻：翻页时钟

在线版：https://flipclock.sts.jx.cn/

一个全屏的翻页钟，顺带做了倒计时、秒表和番茄钟。纯前端，没有依赖，断网也能用。

## 跑起来

扔到任何静态服务器上就行，不用构建：

    python3 -m http.server 8000

## 有什么

- 时钟：24/12 小时制，翻页声能关
- 倒计时：常用时长有预设，也能自己输
- 秒表：百分秒精度，L 键计次
- 番茄钟：25+5 自动轮
- 指南：快捷键怎么按、OBS 怎么挂

## 为什么放出来

写翻页动效踩了不少坑，留个参考。代码不算精致，但能跑。

## 页面

    index.html      落地页
    clock.html      时钟
    countdown.html  倒计时
    stopwatch.html  秒表
    pomodoro.html   番茄钟
    guide.html      指南
    longtail/       12 个问答页（OBS、屏幕常亮、和 Fliqlo 的区别之类）

## 已知的毛病

- 低端手机上翻页会掉帧，每帧要重排的元素太多了
- 长尾页是后来批量补的，文案质量参差

## 许可

MIT。
