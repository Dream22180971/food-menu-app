<div align="center">

# 三餐有意思 · What To Eat Today

**一个围绕“今天吃什么”的 AI 饮食小助手：推荐、菜谱、饮食记录和购物清单。**

[English](./README.md) | [简体中文](./README.zh-CN.md)

[![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev)
[![Vite](https://img.shields.io/badge/Vite-6-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vite.dev)
[![AI](https://img.shields.io/badge/AI-Gemini-F97316?style=for-the-badge)](#ai-能力)
[![License](https://img.shields.io/badge/LICENSE-MIT-10B981?style=for-the-badge)](./LICENSE)

</div>

---

## 它是什么

当前版本已经是 React Web 应用，重点解决每天真实的吃饭决策。

它把这些能力放到一个流程里：

- AI 推荐今天吃什么
- 管理个人菜谱
- 记录每天吃了什么
- 维护购物清单
- 收藏喜欢的菜
- 从内容 / 图片辅助解析菜谱
- 本地数据兜底

---

## 演示

<div align="center">

<img width="92%" alt="三餐有意思" src="https://github.com/user-attachments/assets/5bcb3c7a-6939-4720-bb56-9a1640f97e43" />

</div>

> 这个仓库早期 README 还是“小程序 / Taro”定位，但当前代码已经是 React 19 + Vite，本版文档以当前代码为准。

---

## 5 分钟快速开始

```bash
git clone https://github.com/Dream22180971/food-menu-app.git
cd food-menu-app

npm install
npm run dev
```

访问 `http://localhost:3000`。

---

## 核心体验

| 区域 | 作用 |
|---|---|
| 首页 | AI 推荐 + 当日饮食记录 |
| 发现 | 浏览 / 搜索菜谱 |
| 清单 | 管理食材和购物项 |
| 收藏 | 保存以后还想做的菜 |
| AI 解析 | 从提供的内容里提取菜谱信息 |
| 本地兜底 | 需要时使用 `localStorage` 保留基础数据 |

---

## AI 能力

当前代码包含：

- 菜品推荐
- 菜谱解析
- 内容辅助生成菜谱

具体 AI 效果取决于本地环境中配置的模型和服务。

---

## 产品方向

它不只是“菜谱列表”，更适合往一个轻量日常饮食工作流发展：

```text
我有什么？
   ↓
能做什么？
   ↓
今天吃了什么？
   ↓
下一次该买什么？
```

---

## 技术栈

```text
React 19
Vite 6
TypeScript
Motion
Firebase
Google GenAI
localStorage fallback
```

---

## 路线图

- [x] 菜谱卡片与发现
- [x] 每日饮食记录
- [x] 收藏
- [x] 购物清单
- [x] AI 推荐
- [ ] 更完整的食材识别流程
- [ ] 周菜谱规划
- [ ] 营养总结
- [ ] 更完善的同步 / 账号方案
- [ ] 可分享菜谱卡

---

## 当前限制

- AI 能力依赖环境配置
- 本地兜底数据只属于当前设备
- 旧 README 中部分“小程序”说明已经不适用于当前代码

---

## License

[MIT](./LICENSE)

<div align="center">

**少一点站在冰箱前发呆，多一点好好吃饭。**

</div>
