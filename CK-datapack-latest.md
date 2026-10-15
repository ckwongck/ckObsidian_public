---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-16 06:00:10 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-16 06:00:01

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 67,251
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 672,912 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 325,424 (約 HKD 2,538,308) [報表日 2026-10-14, 落後 2 日 ⚠️ 資料落後; 同步於 2026-10-16T05:50]
  * 現金結餘: HKD -0 / USD 5,244
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 77 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 34.11 USD | 20057 USD | 4.7% | 2296 USD | 12.9% | 14.5 | 1.27 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 299.4 USD | 10479 USD | 2.4% | 2048 USD | 24.3% | 16.3 | 1.33 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 343.6 USD | 17524 USD | 4.1% | -1364 USD | -7.2% | 34.8 | 1.12 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 342.01 USD | 19153 USD | 4.5% | 2026 USD | 11.8% | 22.4 | 0.98 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 174.48 USD | 38037 USD | 8.9% | - | - | 24.2 | 1.32 | - | Flex(2026-10-14) |
| IB | PLTR | 227.0 | 131.423413062 USD | 200.97 USD | 45620 USD | 10.6% | - | - | 39.8 | 1.03 | - | Flex(2026-10-14) |
| IB | QQQM | 434.0 | 249.066141779 USD | 300.13 USD | 130256 USD | 30.4% | - | - | 16.3 | 1.33 | - | Flex(2026-10-14) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.54 USD | 38909 USD | 9.1% | - | - | 7.8 | 1.12 | - | Flex(2026-10-14) |
| IB | SPCX | 122.0 | 140.002405574 USD | 152.16 USD | 18564 USD | 4.3% | - | - | 45.0 | 1.05 | - | Flex(2026-10-14) |
| IB | URA | 840.0 | 50.432105573 USD | 35.54 USD | 29854 USD | 7.0% | - | - | 46.8 | 2.01 | - | Flex(2026-10-14) |
| IB | VRT | 85.0 | 289.688176106 USD | 222.83 USD | 18941 USD | 4.4% | - | - | 53.7 | 2.49 | - | Flex(2026-10-14) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.8% | - | - | 53.0 | 1.18 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.1% | - | - | 44.9 | 1.8 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.7% | - | - | 16.3 | 1.33 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$428,387**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $389,478 = **90.9%** | 目標 90% | drift +0.9% ✅
  - 防禦 (defense: SGOV+現金): $44,608 = **10.4%** | 目標 10% | drift +0.4% ✅
  - 戶口現金: $5,699

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $148.62 | IV Rank: 45.0 | Vol/30dAvg: 1.05 | 下次財報: -
  * P: 最新價 $133.40 | IV Rank: 58.0 | Vol/30dAvg: 0.94 | 下次財報: -
  * AVGO: 最新價 $344.33 | IV Rank: 34.8 | Vol/30dAvg: 1.12 | 下次財報: -
  * QQQM: 最新價 $299.79 | IV Rank: 16.3 | Vol/30dAvg: 1.33 | 下次財報: -
  * URA: 最新價 $36.12 | IV Rank: 46.8 | Vol/30dAvg: 2.01 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 102.49 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 16.46 | VIX9D (9日短期): 13.97 | VIX9D/VIX Ratio: 0.85 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.25% (信用違約風險, >6%=壓力)
* FOMC 倒數: 11 天 (下次 2026-10-27)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| TSM | $422.25 | 80 | 4.9 | 33.37% | 36.1 | 2.12x | -3.53% |
| TXN | $279.12 | 65 | 27.7 | 1.39% | 51.0 | 1.23x | +0.74% |
* 數據更新: 2026-10-16 05:33:50 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: TSM (總分 80) — 考慮研究後分批建倉
3. 📊 **URA 成交異動** (Vol/Avg=2.0x) → 關注新聞/財報

=== [END OF MAX DATA PACK v4.1] ===
