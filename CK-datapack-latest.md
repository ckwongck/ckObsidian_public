---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-11-21 06:08:22 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-11-21 06:00:10

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: [OpenD accinfo 未授權 - 需 Futu 交易權限]
  * 現金結餘: [OpenD accinfo 未授權]
  * 剩餘購買力: [OpenD accinfo 未授權]
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 286,248 (約 HKD 2,232,736) [報表日 2026-11-19, 落後 2 日 ⚠️ 資料落後; 同步於 2026-11-21T05:50]
  * 現金結餘: HKD -0 / USD 7,216
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 113 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| IB | GRID | 218.0 | 196.402405573 USD | 152.42 USD | 33228 USD | 10.4% | - | - | - | - | - | Flex(2026-11-19) |
| IB | PLTR | 227.0 | 131.423413062 USD | 153.68 USD | 34885 USD | 10.9% | - | - | - | - | - | Flex(2026-11-19) |
| IB | QQQM | 434.0 | 249.066141779 USD | 265.64 USD | 115288 USD | 36.0% | - | - | 17.6 | 3.12 | - | Flex(2026-11-19) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.61 USD | 38936 USD | 12.2% | - | - | - | - | - | Flex(2026-11-19) |
| IB | SPCX | 122.0 | 140.002405574 USD | 138.43 USD | 16888 USD | 5.3% | - | - | 14.6 | 1.17 | - | Flex(2026-11-19) |
| IB | URA | 840.0 | 50.432105573 USD | 28.67 USD | 24083 USD | 7.5% | - | - | - | - | - | Flex(2026-11-19) |
| IB | VRT | 85.0 | 289.688176106 USD | 184.99 USD | 15724 USD | 4.9% | - | - | - | - | - | Flex(2026-11-19) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 2.4% | - | - | - | - | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.8% | - | - | 21.5 | 1.58 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 7.6% | - | - | 17.6 | 3.12 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$320,027**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $281,091 = **87.8%** | 目標 90% | drift -2.2% ⚠️ 不足
  - 防禦 (defense: SGOV+現金): $46,607 = **14.6%** | 目標 10% | drift +4.6% ⚠️ 超配
  - 戶口現金: $7,671

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: [需 Futu Basic 訂閱 / yfinance 離線] | IV Rank: 14.6 | Vol/30dAvg: 1.17 | 下次財報: -
  * P: [需 Futu Basic 訂閱 / yfinance 離線] | IV Rank: 68.4 | Vol/30dAvg: 1.26 | 下次財報: -
  * AVGO: [需 Futu Basic 訂閱 / yfinance 離線] | IV Rank: 24.7 | Vol/30dAvg: 2.27 | 下次財報: -
  * QQQM: [需 Futu Basic 訂閱 / yfinance 離線] | IV Rank: 17.6 | Vol/30dAvg: 3.12 | 下次財報: -
  * URA: [需 Futu Basic 訂閱 / yfinance 離線] | IV Rank: - | Vol/30dAvg: - | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: None (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): None | VIX9D (9日短期): None | VIX9D/VIX Ratio: - (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.52% (信用違約風險, >6%=壓力)
* FOMC 倒數: 17 天 (下次 2026-12-08)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| MSFT | $484.52 | 65 | 18.3 | 0.08% | 43.1 | 1.64x | -5.48% |
* 數據更新: 2026-11-21 05:33:31 HKT

## 六、建議行動 (Actionable Insights)
1. 💰 **現金/SGOV 過多 4.6%** → 錯失增長機會，考慮分批轉增長倉
2. 🎯 **Alpha 機會**: MSFT (總分 65) — 考慮研究後分批建倉
3. 📊 **AVGO 成交異動** (Vol/Avg=2.3x) → 關注新聞/財報
4. 📊 **QQQM 成交異動** (Vol/Avg=3.1x) → 關注新聞/財報

=== [END OF MAX DATA PACK v4.1] ===
