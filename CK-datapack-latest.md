---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-28 06:01:03 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-28 06:00:54

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 67,931
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 678,460 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 323,159 (約 HKD 2,520,643) [報表日 2026-10-26, 落後 2 日 ⚠️ 資料落後; 同步於 2026-10-28T05:51]
  * 現金結餘: HKD 56,457 / USD 5,242
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 89 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 35.13 USD | 20656 USD | 4.9% | 2895 USD | 16.3% | 13.2 | 0.94 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 296.98 USD | 10394 USD | 2.5% | 1964 USD | 23.3% | 23.2 | 0.75 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 341.5 USD | 17416 USD | 4.2% | -1471 USD | -7.8% | 34.9 | 1.13 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 347.16 USD | 19441 USD | 4.6% | 2314 USD | 13.5% | 18.7 | 1.0 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 163.04 USD | 35543 USD | 8.5% | - | - | 33.6 | 0.71 | - | Flex(2026-10-26) |
| IB | PLTR | 227.0 | 131.423413062 USD | 198.84 USD | 45137 USD | 10.8% | - | - | 45.9 | 0.84 | - | Flex(2026-10-26) |
| IB | QQQM | 434.0 | 249.066141779 USD | 293.26 USD | 127275 USD | 30.3% | - | - | 23.2 | 0.75 | - | Flex(2026-10-26) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.67 USD | 38959 USD | 9.3% | - | - | 2.8 | 0.67 | - | Flex(2026-10-26) |
| IB | SPCX | 122.0 | 140.002405574 USD | 146.9 USD | 17922 USD | 4.3% | - | - | 41.8 | 0.92 | - | Flex(2026-10-26) |
| IB | URA | 840.0 | 50.432105573 USD | 34.36 USD | 28862 USD | 6.9% | - | - | 53.2 | 1.52 | - | Flex(2026-10-26) |
| IB | VRT | 85.0 | 289.688176106 USD | 199.78 USD | 16981 USD | 4.0% | - | - | 121.7 | 1.57 | - | Flex(2026-10-26) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.8% | - | - | 50.4 | 0.79 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.1% | - | - | 74.0 | 1.34 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.8% | - | - | 23.2 | 0.75 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$419,582**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $380,623 = **90.7%** | 目標 90% | drift +0.7% ✅
  - 防禦 (defense: SGOV+現金): $51,895 = **12.4%** | 目標 10% | drift +2.4% ⚠️ 超配
  - 戶口現金: $12,935

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $148.58 | IV Rank: 41.8 | Vol/30dAvg: 0.92 | 下次財報: -
  * P: 最新價 $138.73 | IV Rank: 81.5 | Vol/30dAvg: 0.46 | 下次財報: -
  * AVGO: 最新價 $342.33 | IV Rank: 34.9 | Vol/30dAvg: 1.13 | 下次財報: -
  * QQQM: 最新價 $296.96 | IV Rank: 23.2 | Vol/30dAvg: 0.75 | 下次財報: -
  * URA: 最新價 $35.86 | IV Rank: 53.2 | Vol/30dAvg: 1.52 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 97.87 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 17.52 | VIX9D (9日短期): 16.65 | VIX9D/VIX Ratio: 0.95 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.3% (信用違約風險, >6%=壓力)
* FOMC 倒數: 41 天 (下次 2026-12-08)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| TSM | $436.87 | 75 | 4.0 | 53.10% | 35.8 | 0.82x | +0.73% |
| MU | $928.76 | 65 | 9.0 | 2.77% | 31.3 | 0.87x | -3.45% |
* 數據更新: 2026-10-28 05:34:32 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: TSM (總分 75) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
