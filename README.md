# Winscope for Android 17

这是为 Android 17 编译的 Winscope Web 前端产物，可用于查看和分析 Android 系统跟踪数据。

## 本地运行

在仓库目录启动一个静态文件服务器：

```bash
python -m http.server 8000
```

然后访问 <http://localhost:8000/>。

## 通过 ADB 连接设备

实时采集需要 Python 3.10 或更高版本，并确保 `adb` 已加入 `PATH`：

```bash
python winscope_proxy.py
```

代理默认监听 `localhost:5544`。本构建所带的 Winscope ADB Connect proxy 版本为 `6.0.2`。

## 许可说明

Winscope 构建产物包含 Android Open Source Project 及第三方组件。相关声明请参见各文件头部和 [`3rdpartylicenses.txt`](3rdpartylicenses.txt)。

