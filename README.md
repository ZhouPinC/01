# Flutter Voice Wave Demo

一个 Flutter 音量条组件与演示应用。`VoiceWaveWidget` 使用自定义绘制展示从右向左滚动的音量波形，示例页通过随机样本模拟实时录音振幅。

## 功能

- 实时追加 `0.0` 到 `1.0` 的振幅样本。
- 使用圆角竖条绘制滚动波形。
- 可配置颜色、条宽、间距和显示高度。
- 支持开始/停止模拟以及清空波形。
- 工程包含 Android、iOS、Web、Windows、macOS 和 Linux 平台目录。

## 技术栈

- Flutter / Dart 3.10
- Material 3
- `CustomPainter` 驱动的自定义波形组件

## 目录结构

```text
01/
`-- Flutter01/
    |-- lib/main.dart                    # 示例应用
    |-- lib/widgets/voice_wave_widget.dart # 波形组件与控制器
    |-- test/                            # Flutter 测试
    |-- pubspec.yaml                     # 项目配置
    `-- 开发计划书.md                    # 需求、架构与里程碑
```

## 本地运行

```powershell
cd Flutter01
flutter pub get
flutter run
```

运行测试与静态检查：

```powershell
flutter analyze
flutter test
```

## 使用说明

通过 `VoiceWaveController.addSample()` 向组件写入归一化振幅；调用方负责真实录音、权限请求和振幅换算。当前演示页只生成模拟数据，不会访问麦克风。

## 状态

组件原型。基础绘制和模拟输入已实现，真实录音接入、性能基准和完整测试仍待补充。
