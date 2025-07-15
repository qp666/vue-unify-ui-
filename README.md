# vue-unify-ui  
> **One Design, Everywhere.**  
> **一套设计，统治所有 Vue & uni-app 场景。**

[![npm](https://img.shields.io/npm/v/vue-unify-ui?style=flat-square&colorA=000&colorB=31c27c)](https://npm.im/vue-unify-ui)
[![downloads](https://img.shields.io/npm/dm/vue-unify-ui?style=flat-square&colorA=000&colorB=ff4757)](https://npm.im/vue-unify-ui)
[![coverage](https://img.shields.io/codecov/c/github/qp666/vue-unify-ui?style=flat-square&colorA=000&colorB=5f27cd)](https://codecov.io/gh/qp666/vue-unify-ui)
[![license](https://img.shields.io/github/license/qp666/vue-unify-ui?style=flat-square&colorA=000&colorB=00d2d3)](https://github.com/qp666/vue-unify-ui/blob/main/LICENSE)

---

## 前言 · Preface

> “PC 用 Element，H5 用 Vant，小程序用 Wot？  
>  抱歉，2025 年了，我们只做一件事：  
>  **让一套代码在所有端都能优雅地呼吸。**”

**vue-unify-ui** 是首个、也是唯一一个同时面向  
**Web(PC & Mobile)** + **微信小程序** + **支付宝小程序** + **App(H5+Native)**  
的 **泛 Vue 统一设计体系**。

我们站在 Element-Plus、Ant-Design-Vue、Vant、Taro-UI、Wot-UI、Naive-UI 等巨人的肩膀上，  
将“百家之所长”熔于一炉，铸成一把足以劈开多端混沌的利剑。

---

## 设计哲学 · Design Philosophy

| 维度 | 传统方案 | vue-unify-ui |
|---|---|---|
| **Design Token** | 多端各自为政 | 原子级变量，一键全局换肤 |
| **API 语义** | PC / Mobile / 小程序 三套心智 | 100% 统一，零心智切换 |
| **组件粒度** | 要么过于抽象，要么过于具体 | 分层设计：原子 → 基础 → 业务 |
| **构建产物** | 多套仓库，重复 CI/CD | 单仓 monorepo，一键发布 6 端 |
| **TypeScript** | 部分支持 | 100% 类型安全，自动推断 |

> “真正的统一不是妥协，而是更高维度的抽象。”  
> —— vue-unify-ui 作者 @qp666

---

## 能力矩阵 · Capability Matrix

| 场景 | 渲染引擎 | 组件完成度 | 主题系统 | SSR | 自动化测试 |
|---|---|---|---|---|---|
| **PC Web** | Vue3 / Vite | ✅ 100% | ✅ Design Token | ✅ | ✅ e2e + screenshot |
| **Mobile Web** | Vue3 / Vite | ✅ 100% | ✅ Design Token | ✅ | ✅ e2e + screenshot |
| **微信小程序** | uni-app | ✅ 100% | ✅ Design Token | ❌ | ✅ miniprogram-sim |
| **支付宝小程序** | uni-app | ✅ 100% | ✅ Design Token | ❌ | ✅ miniprogram-sim |
| **App(原生)** | uni-app | ✅ 100% | ✅ Design Token | ❌ | ✅ appium |
| **SSR / SSG** | Nuxt3 | ✅ 100% | ✅ Design Token | ✅ | ✅ playwright |

---

## 30 秒快速开始 · Quick Start

```bash
# 全局安装 CLI（推荐）
npm i -g @vue-unify/cli

# 创建多端项目
vue-unify create my-project
cd my-project

# 一键运行所有端
pnpm dev:all
