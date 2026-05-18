# 📊 量化交易 × Web3 学习手册

> **从入门到就业 · 全程可运行代码**
>
> A complete, hands-on learning path for Quantitative Finance & Web3, with executable Jupyter Notebooks at every step.

---

## 🗺️ 这是什么

这是一份**可以边读边跑**的量化 + Web3 学习手册，共 14 个 Jupyter Notebook，覆盖从数学基础到前沿 ZKML 的完整路径。

**适合谁：**
- 金融 / 数学 / 计算机背景的学生，想进量化行业
- 主观投资者，想转量化
- 传统金融从业者，想进 Web3
- 任何对「用代码做投资」感兴趣的人

**不适合谁：**
- 寻找"圣杯策略"的人（这份手册不会让你一夜暴富）
- 完全不愿意写代码的人

---

## 📚 目录

### 🔰 模块一：量化交易基础

| Notebook | 主题 | 预计时间 | 核心内容 |
|----------|------|----------|---------|
| [00](./00_学习地图.ipynb) | 学习地图 & 环境配置 | 1h | 整体路径规划，一键安装所有依赖 |
| [01](./01_量化入门_多因子模型.ipynb) | 量化入门 + 多因子模型 | 8–12h | Sharpe/最大回撤/IC/ICIR，单因子检验，组合优化 |
| [02](./02_量化策略_回测实战.ipynb) | 量化策略 + 回测实战 | 10–15h | CTA 趋势跟踪，统计套利，LightGBM 选股，样本外检验 |
| [03](./03_量化企业实务_求职.ipynb) | 企业实务 + 求职 | 4–6h | 量化私募/公募结构，岗位薪资，简历/笔试/面试 |

### 🌐 模块二：Web3 全栈

| Notebook | 主题 | 预计时间 | 核心内容 |
|----------|------|----------|---------|
| [04](./04_Web3入门_区块链原理.ipynb) | Web3 入门 + 区块链原理 | 6–8h | 手写区块链，哈希/签名/共识，Merkle 树，EVM 原理 |
| [05](./05_Web3_Solidity_智能合约.ipynb) | Solidity + 智能合约 | 8–12h | ERC20/NFT 开发，web3.py 部署，6 大安全漏洞 |
| [06](./06_Web3_DeFi_链上数据.ipynb) | DeFi + 链上数据分析 | 10–12h | 复刻 Uniswap V2，Aave 借贷，Dune Analytics |
| [07](./07_链上量化_MEV与套利.ipynb) | 链上量化 + MEV + 求职 | 8–10h | 跨 DEX 套利，三明治攻击，Flashbots，Crypto Quant 求职 |

### 🤖 模块三：AI × 量化前沿

| Notebook | 主题 | 预计时间 | 核心内容 |
|----------|------|----------|---------|
| [08](./08_数学统计基础.ipynb) | 数学统计基础 | 6–8h | 概率论、线性代数、时间序列、随机过程、因果推断 |
| [09](./09_ML深度学习_因子挖掘.ipynb) | ML/深度学习挖掘 Alpha | 10–15h | LSTM/Transformer/GNN 选股，AutoEncoder 因子，SHAP |
| [10](./10_强化学习交易.ipynb) | 强化学习交易 | 8–12h | DQN 择时，PPO 仓位管理，金融 RL 三大陷阱 |
| [11](./11_LLM大模型与另类数据.ipynb) | 大模型 + 另类数据 | 6–8h | GPT/Claude 情绪分析，FinGPT，卫星/信用卡另类数据 |

### 🚀 模块四：Web3 前沿 + AI on-chain

| Notebook | 主题 | 预计时间 | 核心内容 |
|----------|------|----------|---------|
| [12](./12_Web3最新生态.ipynb) | Web3 最新生态（2024–2026） | 6–8h | L2/Account Abstraction/EigenLayer/永续 DEX |
| [13](./13_链上AI_ZKML.ipynb) | 链上 AI + ZKML | 5–7h | ZK 证明，ZKML vs OPML vs TEE，链上 AI Agent |

**总计：约 100–140 小时**（可按模块拆分，分 3–6 个月完成）

---

## 🛠️ 环境配置

```bash
# 1. 创建虚拟环境
conda create -n quant python=3.11 -y
conda activate quant

# 2. 安装核心依赖
pip install -r requirements.txt

# 3. 启动 Jupyter
jupyter lab
```

> 详细说明见 [00_学习地图.ipynb](./00_学习地图.ipynb)

---

## 📦 依赖概览

| 类别 | 主要库 |
|------|--------|
| 数据处理 | `numpy` `pandas` `scipy` |
| 机器学习 | `scikit-learn` `lightgbm` `xgboost` |
| 深度学习 | `torch` `torchvision` |
| 金融数据 | `yfinance` `akshare` `tushare` |
| 回测 | `backtrader` `bt` |
| 组合优化 | `cvxpy` |
| 可视化 | `matplotlib` `seaborn` `plotly` |
| Web3 | `web3` `eth-brownie` |
| 时间序列 | `statsmodels` `arch` |
| NLP / LLM | `transformers` `openai` `anthropic` |
| 强化学习 | `gymnasium` `stable-baselines3` |

---

## 🗂️ 推荐学习路径

```
                  ┌──────────────────┐
                  │  00 学习地图     │  ← 从这里开始
                  └────────┬─────────┘
              ┌────────────┴────────────┐
              ↓                         ↓
   ┌──────────────────┐      ┌──────────────────┐
   │  量化路线        │      │  Web3 路线       │
   │  01 → 02 → 03   │      │  04 → 05 → 06 → 07│
   └────────┬─────────┘      └─────────┬────────┘
            │                          │
            └──────────┬───────────────┘
                       ↓
            ┌──────────────────────┐
            │   AI × 量化前沿      │
            │   08 → 09 → 10 → 11  │
            └──────────┬───────────┘
                       ↓
            ┌──────────────────────┐
            │   Web3 前沿 + 链上AI │
            │       12 → 13        │
            └──────────────────────┘
```

---

## 📝 License

[MIT License](./LICENSE) — 欢迎 fork、star、提 issue 和 PR 🎉

---

## 🙏 贡献 & 反馈

如果你发现代码错误、数据链接失效，或者有更好的教学示例，欢迎提 [Issue](../../issues) 或 [Pull Request](../../pulls)。

---

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11-blue?logo=python" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter" />
  <img src="https://img.shields.io/badge/License-MIT-green" />
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen" />
</p>
