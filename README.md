# 三餐有意思 | What To Eat Today

> 每天不知道吃什么？拍一张冰箱照片，AI 帮你规划今天吃什么。

[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)
[![Taro](https://img.shields.io/badge/Taro-4.x-007FFF?style=flat)](https://taro.zone/)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=flat&logo=react)](https://react.dev)

---

## 目录

- [截图](#截图)
- [它是什么](#它是什么)
- [为什么做](#为什么做)
- [核心功能](#核心功能)
- [快速开始](#快速开始)
- [技术架构](#技术架构)
- [Roadmap](#roadmap)
- [FAQ](#faq)
- [谁适合用](#谁适合用)
- [关于我](#关于我)

---

## 截图

<img width="2560" height="922" alt="三餐有意思界面" src="https://github.com/user-attachments/assets/5bcb3c7a-6939-4720-bb56-9a1640f97e43" />

---

## 它是什么

一个**微信小程序**，帮你解决"今天吃什么"这个世纪难题。

**你可以用它来：**
- 拍一张冰箱照片，AI 自动识别食材，推荐你今天做什么菜
- 发现新菜谱，AI 自动生成精美封面图
- 管理你的个人菜谱库，收藏喜欢的菜谱

所有 AI 能力通过云函数调用，不需要你配置任何 API Key。

---

## 为什么做

每天下班回家，打开冰箱，面对一堆食材发呆——"今天吃什么？"

试过很多菜谱 App，要么推荐的菜太复杂，要么家里根本没有那些食材。

这个小程序的思路：**直接拍冰箱，AI 看看你有什么，然后告诉你能做什么**。不需要你手动输入食材，拍照就行。

---

## 核心功能

| 你能做什么 | 说明 |
|-----------|------|
| **拍照识菜** | 拍冰箱照片，AI 自动识别食材并推荐菜谱 |
| **AI 生图** | 菜谱详情页自动生成精美封面图 |
| **个人菜谱库** | 收藏、管理你喜欢的菜谱 |
| **AI 对话** | 和 AI 聊天，问它怎么做菜、营养搭配等 |
| **云函数集成** | 所有 AI 能力走云函数，安全可靠 |

---

## 快速开始

```bash
# 1. 进入小程序目录
cd miniprogram

# 2. 安装依赖
npm install

# 3. 启动开发模式
npm run dev:weapp
```

然后用微信开发者工具导入 `miniprogram/` 目录，开启云开发即可。

### 云函数部署

AI 能力通过 `aiService` 云函数提供：

```bash
cd miniprogram/cloudfunctions/aiService
npm install
```

在 CloudBase 控制台确认以下能力已启用：
- 文本生成：`hunyuan-exp`
- 图生文：`dashscope-custom / qwen3.5-omni-flash`
- 生图：`hunyuan-image`

---

## 技术架构

```
┌────────────────────────────────────────┐
│     微信小程序 (Taro 4.x + React)      │
│  拍照识别 · 菜谱浏览 · AI 对话          │
├────────────────────────────────────────┤
│     CloudBase 云函数 (aiService)       │
│  文本生成 · 图片识别 · AI 生图          │
├────────────────────────────────────────┤
│     AI 模型层                          │
│  混元大模型 · DashScope Qwen            │
├────────────────────────────────────────┤
│     CloudBase 云开发                    │
│  云数据库 · 云存储 · 用户鉴权           │
└────────────────────────────────────────┘
```

---

## Roadmap

- [x] AI 图片识别导入菜谱
- [x] AI 自动生成菜谱封面
- [x] 云函数统一 AI 调用
- [ ] 菜谱营养分析
- [ ] 个人饮食记录
- [ ] 社区分享菜谱
- [ ] 智能周菜谱规划

---

## FAQ

**Q: 需要自己配置 API Key 吗？**
A: 不需要。所有 AI 能力通过 CloudBase 云函数调用，API Key 配置在云开发控制台，不在代码中。

**Q: 支持哪些 AI 模型？**
A: 文本生成用混元大模型，图片识别用 DashScope Qwen，生图用混元生图模型。

**Q: 云函数超时怎么办？**
A: 在 CloudBase 控制台把 `aiService` 云函数的超时时间调大，视觉/生图建议 ≥ 60 秒。

**Q: 只能用微信吗？**
A: 当前版本是微信小程序。Taro 框架支持多端编译，理论上可以扩展到 H5 和 App。

---

## 谁适合用

- **不知道吃什么的打工人**：拍照冰箱，AI 帮你决定
- **喜欢做饭但没灵感的人**：AI 推荐新菜谱，自动生成封面
- **小程序开发者**：参考 Taro + CloudBase + AI 的集成方案
- **对 AI 应用感兴趣的人**：云函数调用大模型的完整案例

---

## 关于我

我是**肖恩沃尔特**（Sean Walter），一个从测试工程师正在转型为 AI 独立开发者的程序员。

"三餐有意思"是我把 AI 和日常生活结合的一个尝试——用技术解决"今天吃什么"这个小问题。

- GitHub: [Dream22180971](https://github.com/Dream22180971)
- Twitter/X: [@sean_walter0717](https://x.com/sean_walter0717)
- 博客: [seanwalter.top](https://seanwalter.top)

---

## License

[MIT](./LICENSE)
