# Jyutman-images

粤语文丛（Jyutman）的影像 manifest 仓。

## 定位

本仓只放影像 manifest（元数据清单），不放大图。每个条目记录：

- `object_key`：R2 对象键（ASCII）
- 尺寸：width / height
- checksum：sha256
- 来源：藏馆 / Internet Archive ID / 条目链接
- 许可与版权核查状态
- 页码映射：扫描序号与原书叶码

影像本体存放在 R2，不进 Git。影像默认不公开，须逐件核查扫描件条款与藏馆声明后，
在 manifest 中标记为开放；未核查的条目一律不对外提供。

## 内容组织

| 路径 | 内容 |
|---|---|
| `manifest/manifest.sample.json` | 示例条目，展示字段形状 |

真实 manifest 由站点同步脚本生成（待实现）。
