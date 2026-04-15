<div align="center">

# ⚗️ MBTI分子 — 人际化学反应预测器

> *"每个人都是一种独特的元素，当两种元素相遇，便产生一场化学反应。"*

[![纯前端](https://img.shields.io/badge/%E7%BA%AF%E5%89%8D%E7%AB%AF-%E9%9B%B6%E4%BE%9D%E8%B5%96-brightgreen)](https://github.com/haizhongjin100-source/mbti-molecule)
[![页面数](https://img.shields.io/badge/%E9%A1%B5%E9%9D%A2-9-blue)](https://github.com/haizhongjin100-source/mbti-molecule)
[![反应数据](https://img.shields.io/badge/%E5%8F%8D%E5%BA%94%E6%95%B0%E6%8D%AE-408%E6%9D%A1-orange)](https://github.com/haizhongjin100-source/mbti-molecule)

**选两个 MBTI 人格，生成一场专属的「人际化学反应」分析。**

以化学实验报告的形式呈现——反应方程式、温度计、剧烈程度、沟通模式、相处建议……
把严肃的人格分析变成一次有趣的实验。

**→ [立即体验：mbti.haizhongjin.space](https://mbti.haizhongjin.space)**
**→ [或双击 index.html 本地打开](#-本地部署)**

</div>

---

## 🧪 这是什么？

MBTI分子 是一个纯前端趣味项目，把 **16 种 MBTI 人格之间的化学反应** 以化学实验报告的风格展示出来。

比如：**INTJ + ENFP** 产生什么反应？**INFP 和 ISTJ** 在职场能合得来吗？

项目覆盖全部 **136 种人格组合 × 3 个维度（友谊 / 恋爱 / 职场）= 408 条化学反应数据**，每条包含：

- 🧪 伪化学方程式（产物、催化剂、反应热）
- 🌡️ 最佳相处温度计（match% 液柱动画）
- 💬 沟通模式 & 信任建立分析
- ⚡ 冲突预警 & 典型场景
- 📋 相处建议

---

## ✨ 功能一览

### 核心功能

| 功能 | 页面 | 说明 |
|------|------|------|
| ⚗️ **化学反应预测** | [index.html](index.html) | 选择两个 MBTI 人格，生成化学反应报告，支持友谊/恋爱/职场三维度 |
| 🔬 **反应方程式** | index.html | 自动生成伪化学方程式（产物、催化剂、温度、反应热） |
| 🌡️ **温度计** | index.html | match% 映射为温度读数，液柱动画直观展示契合度 |

### 探索工具

| 功能 | 页面 | 说明 |
|------|------|------|
| 📊 **人格详情** | [personality.html](personality.html) | 16 种 MBTI 完整档案：特质、沟通、情感、职业、成长指南 |
| 🔗 **组合全览** | [combos.html](combos.html) | 选择一个人格，一览与所有 15 种类型的化学反应 |
| 🏆 **CP 排行榜** | [ranking.html](ranking.html) | 全部 136 组组合按匹配度排名，支持按强度筛选 |
| 🕸️ **分子图谱** | [molecule.html](molecule.html) | Canvas 力导向关系网络图，可视化 16 种人格的关系 |
| 🧬 **16型周期表** | [periodic.html](periodic.html) | MBTI 人格以化学元素周期表形式排列，四大气质分组 |

### 趣味互动

| 功能 | 页面 | 说明 |
|------|------|------|
| 🧪 **快速测试** | [quiz.html](quiz.html) | 4 道趣味选择题，快速测出你的 MBTI |
| 🖼️ **人格画像** | [portrait.html](portrait.html) | 输入名字生成专属人格标签卡，支持保存为图片 |
| 🏠 **宿舍兼容性** | [dorm.html](dorm.html) | 2-8 人宿舍分析：氛围判定、冲突预警、作息兼容 |

---

## 📸 项目截图

> 主页 — 化学反应预测器，选择两个 MBTI 人格后生成实验报告风格的分析结果

> 人格详情页 — 完整的人格档案卡片，包含特质、沟通方式、代表人物等

> 16型周期表 — 以化学元素周期表形式展示 MBTI 十六型人格

---

## 🗂️ 项目结构

```
MBTI分子/
├── index.html          ⚗️  主页 — 化学反应预测器
├── personality.html    🔬  人格详情 — 16种人格完整档案
├── combos.html         🔗  组合全览 — 一个MBTI × 所有组合
├── quiz.html           🧪  快速测试 — 4题测出MBTI
├── ranking.html        🏆  CP排行榜 — 按匹配度排名
├── molecule.html       🕸️  分子图谱 — 关系网络可视化
├── periodic.html       🧬  16型周期表
├── portrait.html       🖼️  人格画像 — 专属标签卡
├── dorm.html           🏠  宿舍兼容性测试
├── images/             🖼️  16种人格头像 (PNG)
└── scripts/
    └── data.js         📊  共享数据（3×136组反应 + 人格档案）
```

### 页面导航关系

```
index.html（主页入口）
  ├→ personality.html?type=XX    人格详情
  ├→ combos.html                 组合全览
  ├→ ranking.html                CP排行榜
  ├→ molecule.html               分子图谱
  ├→ portrait.html               人格画像
  ├→ quiz.html                   快速测试
  └→ 支持 URL 参数 ?mbti1=XX&mbti2=YY 预选人格

所有页面之间可通过导航栏互相跳转
```

---

## 🎨 设计风格

**复古科学实验室 × 化学分子美学 × 学院派复古风**

理性、克制、带着神秘感的维多利亚实验记录风格。泛黄的纸张背景，配合红铜色和松绿色的点缀，营造出实验室记录本的质感。

**色彩系统**：

| 用途 | 色值 | 说明 |
|------|------|------|
| 背景主色 | `#F5F0E8` | 泛黄纸张色 |
| 强调色 | `#C45C3E` | 复古红铜色 |
| 辅助色 | `#3D5A4C` | 深松绿 |
| 文字主色 | `#2D2A26` | 深棕黑 |

**反应强度配色**：

| 强度 | 色值 | 视觉 |
|------|------|------|
| 💥 爆炸 | `#D64933` | 烈焰红 |
| 🔥 剧烈 | `#C45C3E` | 红铜色 |
| 🌿 温和 | `#7A8B6E` | 苔藓绿 |
| 🌊 平静 | `#5B7A8C` | 灰蓝色 |
| ❄️ 冰封 | `#4A4A4A` | 炭灰色 |

---

## 🔬 数据说明

| 数据类型 | 数量 | 说明 |
|----------|------|------|
| 化学反应组合 | 136 组 | 覆盖全部 C(16,2) + 16 种同类型组合 |
| 反应维度 | ×3 | 友谊版 / 恋爱版 / 职场版 |
| **反应数据总计** | **408 条** | 每条含 intensity、title、desc、match、comm、trust、conflict 等字段 |
| 人格档案 | 16 份 | 每种人格含概述、特质、沟通、情感、职业、成长、代表人物 |

---

## 🚀 本地部署

```bash
# 克隆仓库
git clone https://github.com/haizhongjin100-source/mbti-molecule.git

# 进入目录
cd mbti-molecule

# 双击 index.html 直接在浏览器中打开即可
```

**零依赖、零配置、零构建。** 纯前端静态页面，不需要安装任何东西，不需要启动服务器。

> 也可以用 VS Code 的 Live Server 插件打开，体验更佳。

---

## 🛠️ 技术栈

| 技术 | 用途 |
|------|------|
| HTML / CSS / JavaScript | 纯原生，无框架依赖 |
| [html2canvas](https://github.com/niklasvh/html2canvas) | 人格画像保存为图片 |
| Canvas API | 分子图谱力导向图 |
| Google Fonts | Playfair Display + Noto Serif SC |

---

## ⚠️ 声明

MBTI 人格测试仅供娱乐和社交参考，人格无好坏之分。所有化学反应分析均为趣味性解读，请以娱乐心态对待。

---

<div align="center">

*MBTI分子实验室 · 仅供娱乐 · 人格无好坏*

</div>
