# 01 — Flutter 语音波形组件

从 0 到 1 开发一个 Flutter 自定义录音波形可视化组件，对标 iPhone 语音备忘录的音频波形动画效果。

## 目标

实现可独立复用、配置化的 `VoiceWaveWidget` + `VoiceWaveController`，提供：
- 📊 实时音频波形条渲染（Canvas CustomPainter）
- 🎨 可配置条宽/间距/颜色/圆角/镜像/滚动速度
- 🔄 支持实时录音数据注入与历史数据回放
- ⚡ 目标 60fps 稳定帧率

## 技术栈

- Flutter / Dart
- 自定义 `CustomPainter` 绘制
- `AnimationController` 驱动滚动

## 项目状态

当前处于原型开发阶段，详见 [开发计划书](./开发计划书.md)。

## 运行

```bash
flutter pub get
flutter run
```

## 相关项目

| 项目 | 说明 |
|------|------|
| [Test251204](https://github.com/ZhouPinC/Test251204) | Kotlin Android 端波形组件测试原型 |
| [ZPC](https://github.com/ZhouPinC/ZPC) | Java Android 端录音机成品（含 AudioWaveformView） |