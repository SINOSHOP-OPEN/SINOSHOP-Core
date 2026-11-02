# 🌊 SINOSHOP-Core (Pre-Alpha)

> **觀天之道，執天之行。造福人民。**
> *Observe Nature’s Order, Align with Ocean’s Rhythm, Advance the People’s Welfare.*

**海生電，電養橋，橋造城，城惠民。**
**各美其美，美美與共。**
*Ocean breeds energy, energy sustains the corridors, corridors build cities, and cities benefit the people.*
*Each cherishes its own beauty, and all share in the harmony of common beauty.*

## 🛠️ 1. 物理工程藍圖 | Engineering Blueprint
SINOSHOP 是一套開源的超大型海洋自維持穩定平台協議。我們以實事求是的工程數據，構建海洋文明的基石。
### A. 核心規格 | Core Specifications
 * **構型 (Hull)**：138m 寬 × 27m 高 扁橢圓柱體。
 * **結構 (Structure)**：竹塑玄武岩纖維複合外殼 + 密封中空鋼管桁架一體化。
 * **內部集成 (Internal Integration)**：6 條 Φ21m 並排功能管廊。
   * **底層 (Equipment)**：中心線下 **3.9m** (模數化設備與能源層)。
   * **頂層 (Safety)**：中心線上 **6.1m** (獨立救生平台層)。
 * **補償 (Dynamics)**：殼壁間 **1.7m** 夾層發電水艙。

## 🎯 2. 技術挑戰 | Hero Tasks
物理硬件已具備“毫米級穩定”的潛能，現在需要算法賦予其靈魂。我們開放 **雙軌制考驗**：

| 賽道 | 環境 | 目標 | 狀態 |
| :--- | :--- | :--- | :--- |
| **🏆 鏈上 L1 (已就緒)** | Solidity + Foundry CI | 平均誤差 < 100mm，穩定通過 30s 動態 | 參見 Issue #1 |
| **🔬 物理仿真 (Python)** | `run_demo.py` 非線性模型 | RMSD < 50mm (基線 68mm) | 用於本地調優 |

**共同約束**：30s 慣性時滯，±30mm 執行器死區。
> 鏈上賽道為主要評判標準，通過 CI 自動驗證即為有效貢獻。

## 📜 3. 精神與願景 | Philosophy & Vision

**貞忠昭日月，惠民播春秋。**
**Steadfast Loyalty glowing like the sun and moon;**
**Benevolence nourishing the tide of time.**

**實事求是聲明 (Sincerity Statement)**：
本项目目前由 SINOSHOP 技术委员会自费推进，处于极早期阶段。我们不提供即時現金激励，转而提供基于代码贡献的**长期资产确权**。具体贡献者经济模型、法律文件及合规要求，请务必阅读以下核心文档：

 * 📄 **[ECONOMICS.md](./ECONOMICS.md)** — TigerToken 释放规则、RWA 分红计算公式、权益层级表。
 * 📄 **[CONTRIBUTING.md](./CONTRIBUTING.md)** — 贡献指南与行为准则。
 * 📄 **[CLA.pdf](./CLA.pdf)** — 贡献者许可协议（知识产权归属）。
 * 📄 **[docs/COMPLIANCE.md](./docs/COMPLIANCE.md)** — ERC-3643 合格貢獻者验证流程。

### 貢獻者權益 (Contributor Rights)：
 1. **技術確權**：你的 Commit 是未來權益分配與資產代幣化的唯一審計依據。
 2. **名譽永久**：合併 PR 的貢獻者將永久載入 [HALL_OF_FAME.md](./HALL_OF_FAME.md) 架构师名录。
 3. **鏈上透明**：悬赏池代码公开在 `contracts/governance/Bounty.sol`，分红逻辑演示在 `contracts/governance/RevenueDistributor.sol`。
🛡️ 知識產權與法律聲明 | IP & Legal Notice

本項目核心技術受國際專利條約保護。

已申請專利 (Patents Pending)：

🇨🇳 中國發明專利：202411818684.6 — 已進入實質審查階段。

🌐 PCT 國際專利：PCT/CN2025/139199 — 優先權日：2024年12月11日。

貢獻者承諾：你的任何改進，將自動授予項目永久免費使用許可。你保留署名權，並承諾不發起專利訴訟。這不是限制，是對所有人的保護。

詳細條款：請務必閱讀 CLA.pdf 及 CONTRIBUTING.md。
## 🚀 4. 快速開始 | Quick Start

```bash
# 1. 克隆倉庫
git clone https://github.com/SinoSir/SINOSHOP-Core.git

# 2. 物理仿真環境 (Python)
pip install -r requirements.txt
python run_demo.py

# 3. 鏈上測試環境 (Foundry)
forge install
forge test --match-path test/HeroTask.t.sol
