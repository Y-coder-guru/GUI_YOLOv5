# 依赖安装说明（GUI_YOLOv5）

我已经把你现有的两个依赖来源做了整理：

1. `requirements.txt`：用于当前项目的**推荐安装清单**（已合并 Web + YOLOv5 核心依赖）。
2. `requirements_zhihuis_pip.txt`：由 `zhihuis.txt` 自动转换出的 **完整 pip 版本清单**（尽量保留原环境版本）。

## 你现在应该怎么装

### 方案 A（推荐，先跑起来）
```bash
pip install -r requirements.txt
```

### 方案 B（尽量贴近学姐环境）
```bash
pip install -r requirements_zhihuis_pip.txt
```

## 关于你提到的 YOLOv8 / alltrack

- 你这个仓库是 YOLOv5 项目，运行和训练 YOLOv5 **不需要** YOLOv8 的 `alltrack` 那个 txt。
- 所以你删掉 YOLOv8 的依赖文件，一般不影响这个仓库。

## 注意事项

- `zhihuis.txt` 是 Conda 导出的环境文件，里面很多是底层系统包，不能直接用于 `pip install -r`。
- 我已经把可 pip 安装的包转成了 `requirements_zhihuis_pip.txt`。
- 如果你在 Windows 或 Linux 上安装，像 `appnope` 这类 macOS 专用包可以忽略（报错就删掉该行重装）。
