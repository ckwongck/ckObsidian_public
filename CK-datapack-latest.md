---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-11-06 06:00:57 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-11-06 06:00:48

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 64,231
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 646,288 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 305,525 (約 HKD 2,383,093) [報表日 2026-11-04, 落後 2 日 ⚠️ 資料落後; 同步於 2026-11-06T05:50]
  * 現金結餘: HKD 0 / USD 7,129
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 98 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 35.33 USD | 20774 USD | 5.1% | 3013 USD | 17.0% | 26.1 | 1.74 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 265.55 USD | 9294 USD | 2.3% | 864 USD | 10.2% | 39.7 | 5.02 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 293.66 USD | 14977 USD | 3.7% | -3911 USD | -20.7% | 70.4 | 2.45 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 341.94 USD | 19149 USD | 4.7% | 2022 USD | 11.8% | 32.1 | 1.73 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 162.24 USD | 35368 USD | 8.8% | - | - | 50.3 | 3.26 | - | Flex(2026-11-04) |
| IB | PLTR | 227.0 | 131.423413062 USD | 171.7 USD | 38976 USD | 9.7% | - | - | 71.8 | 2.08 | - | Flex(2026-11-04) |
| IB | QQQM | 434.0 | 249.066141779 USD | 284.92 USD | 123655 USD | 30.6% | - | - | 39.7 | 5.02 | - | Flex(2026-11-04) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.45 USD | 38874 USD | 9.6% | - | - | 4.1 | 1.74 | - | Flex(2026-11-04) |
| IB | SPCX | 122.0 | 140.002405574 USD | 135.92 USD | 16582 USD | 4.1% | - | - | 86.1 | 1.7 | - | Flex(2026-11-04) |
| IB | URA | 840.0 | 50.432105573 USD | 32.7 USD | 27468 USD | 6.8% | - | - | 57.4 | 2.21 | - | Flex(2026-11-04) |
| IB | VRT | 85.0 | 289.688176106 USD | 205.55 USD | 17472 USD | 4.3% | - | - | 103.4 | 2.94 | - | Flex(2026-11-04) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.9% | - | - | 59.8 | 1.76 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.2% | - | - | 90.7 | 2.59 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 6.1% | - | - | 39.7 | 5.02 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$403,584**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $364,710 = **90.4%** | 目標 90% | drift +0.4% ✅
  - 防禦 (defense: SGOV+現金): $46,458 = **11.5%** | 目標 10% | drift +1.5% ⚠️ 超配
  - 戶口現金: $7,584

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $123.62 | IV Rank: 86.1 | Vol/30dAvg: 1.7 | 下次財報: -
  * P: 最新價 $93.44 | IV Rank: 118.5 | Vol/30dAvg: 1.5 | 下次財報: -
  * AVGO: 最新價 $291.53 | IV Rank: 70.4 | Vol/30dAvg: 2.45 | 下次財報: -
  * QQQM: 最新價 $266.85 | IV Rank: 39.7 | Vol/30dAvg: 5.02 | 下次財報: -
  * URA: 最新價 $30.98 | IV Rank: 57.4 | Vol/30dAvg: 2.21 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 97.92 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 28.18 | VIX9D (9日短期): 32.66 | VIX9D/VIX Ratio: 1.16 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.32% (信用違約風險, >6%=壓力)
* FOMC 倒數: 32 天 (下次 2026-12-08)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| TXN | $278.15 | 65 | 27.1 | 1.88% | 51.5 | 2.56x | -2.19% |
| FOXA | $67.67 | 65 | 7.4 | 4.19% | 57.6 | 1.58x | +5.01% |
* 數據更新: 2026-11-06 05:34:24 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: TXN (總分 65) — 考慮研究後分批建倉
3. ⚠️ **VIX 高企 (28.18)** → 市場恐慌，短期波動加劇，避免追高
4. 📊 **AVGO 成交異動** (Vol/Avg=2.5x) → 關注新聞/財報
5. 📊 **QQQM 成交異動** (Vol/Avg=5.0x) → 關注新聞/財報
6. 📊 **URA 成交異動** (Vol/Avg=2.2x) → 關注新聞/財報

=== [END OF MAX DATA PACK v4.1] ===
