# 技术阅读蒸馏站

把一本书或一项技术压成一页可交互的 HTML 的合集 —— **读书蒸馏页**与**技术说明页**。

站点入口：**https://svenkunkka.github.io/chip-book-distill/**

全部为单文件页面：没有构建步骤、没有外部框架、没有统计代码，直接打开即可阅读。

---

## 页面目录

| 页面 | 类型 | 链接 |
| --- | --- | --- |
| 芯片通识课：一本书读懂芯片技术（赵秋奇） | 读书蒸馏 · 五板块浏览型 | [/chip-book/](https://svenkunkka.github.io/chip-book-distill/chip-book/) |
| 产品经理认证（NPDP）知识体系指南（第二版）（PDMA） | 读书蒸馏 · 工具型 | [/npdp/](https://svenkunkka.github.io/chip-book-distill/npdp/) |
| Inside a Wireless Chip | 技术说明页 · 无线 SoC 内部结构 | [/wireless-soc/](https://svenkunkka.github.io/chip-book-distill/wireless-soc/) |
| 蓝牙的两套无线电 | 技术说明页 · 经典蓝牙 vs 低功耗蓝牙 | [/bluetooth/](https://svenkunkka.github.io/chip-book-distill/bluetooth/) |

## 目录结构

```
.
├── index.html          # 站点目录页（四页导航）
├── chip-book/          # 芯片通识课 读书蒸馏页
├── npdp/               # NPDP 知识体系指南 读书蒸馏页
├── wireless-soc/       # Inside a Wireless Chip
├── bluetooth/          # 蓝牙的两套无线电
└── .nojekyll           # 跳过 Jekyll 处理，按静态文件原样发布
```

每个子目录以 `index.html` 作为入口，因此链接可以省略文件名。

## 本地阅读

```bash
git clone https://github.com/SvenKunkka/chip-book-distill.git
cd chip-book-distill
open index.html
```

任一子目录里的 `index.html` 也可单独打开或分发。其中 `chip-book/`、`npdp/` 完全自包含；
`wireless-soc/` 与 `bluetooth/` 的排版字体从 Google Fonts 加载，离线环境下会回退到系统字体，内容不受影响。

## 内容来源与致谢

- 读书蒸馏页的页面骨架来自 **sansheng-distill** 蒸馏法（作者：叁笙）。
- 书籍内容的著作权归原作者与出版方所有，此处为个人读书笔记，仅供学习交流。
- 如需复现同款蒸馏页，见 [sansheng-distill-dsh-codex](https://github.com/SvenKunkka/sansheng-distill-dsh-codex)（DSH / Codex 移植版）。

## 许可

- 页面模板结构与排版代码：遵循 sansheng-distill 的原始授权。
- 读书笔记与技术说明正文：CC BY-NC-SA 4.0（署名 - 非商业性使用 - 相同方式共享）。

## 反馈

内容有误、链接失效或想补充新的一页，欢迎提 [Issue](https://github.com/SvenKunkka/chip-book-distill/issues)。
