# 鼎革千年 · 中国历代权力更迭脉络

以长卷轴形式呈现从夏商周到共和国五千年的朝代更迭，聚焦权力结构的演变、制度的兴废与历史周期的回响。

## 预览

直接在浏览器中打开 `index.html` 即可浏览完整内容。

## 内容涵盖


| 时期    | 朝代              |
| ----- | --------------- |
| 先秦    | 夏、商、西周、东周（春秋战国） |
| 大一统帝国 | 秦、西汉、东汉         |
| 分裂与融合 | 三国、西晋、东晋、南北朝    |
| 隋唐盛世  | 隋、唐（含安史之乱专题）    |
| 过渡动荡  | 五代十国            |
| 文治与铁骑 | 北宋、南宋、元         |
| 最后的帝国 | 明、清             |
| 走向共和  | 中华民国、中华人民共和国    |


每个朝代包含：

- **开国叙事** — 王朝建立的关键路径
- **皇帝列表** — 含在位年份、继位方式、结局标签
- **权力洞察** — 制度变迁、灭亡规律、历史启示

## 技术栈

- 纯 HTML + CSS + JavaScript，单文件架构
- 零依赖、零构建工具
- 字体：[Ma Shan Zheng](https://fonts.google.com/specimen/Ma+Shan+Zheng)（书法）、[ZCOOL XiaoWei](https://fonts.google.com/specimen/ZCOOL+XiaoWei)（标题）、[Noto Serif SC](https://fonts.google.com/specimen/Noto+Serif+SC)（正文）
- 滚动驱动动画（IntersectionObserver）
- 响应式设计，适配桌面与移动端

## 设计风格

「墨卷长轴」— 深色墨底 + 金石点缀 + 宣纸韵味，模拟历史长卷的阅读体验。

详细设计体系参见 [.cursor/rules/design-system.mdc](.cursor/rules/design-system.mdc)。

## 本地运行

无需安装任何依赖，任选一种方式：

```bash
# 方式一：直接打开
open index.html

# 方式二：本地服务器（推荐，避免字体加载问题）
python3 -m http.server 8000
# 然后访问 http://localhost:8000
```

## 项目结构

```
dinge-qiannian/
├── index.html              # 全部内容（HTML + CSS + JS）
├── README.md               # 项目说明
└── .cursor/
    └── rules/
        ├── project.mdc     # 项目编码规范
        └── design-system.mdc  # 视觉设计体系约束
```

## License

MIT