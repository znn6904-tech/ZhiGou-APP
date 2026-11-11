# 智构

用中文写下需求，得到能计算的工业模型。这个目录只有手机应用。界面和结果在手机上查看，计算由本机 8000 端口的服务完成。

## 运行

```bash
flutter pub get
flutter emulators --launch Pixel_6_API_35
flutter run -d emulator-5554
```

本机账号：`admin` / `11111111`，`user1` / `11111111`。也可以在登录页注册。

计算服务已在本机 `8000` 端口启动时，Android 模拟器通过 `10.0.2.2:8000` 登录，并读取历史、知识库、笔记和通知。模拟器还需执行 `adb reverse tcp:8000 tcp:8000`。服务未启动时使用本机示例数据。
