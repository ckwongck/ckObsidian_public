---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-11-14 06:00:31 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-11-14 06:00:23

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 68,384
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 682,250 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 305,321 (約 HKD 2,381,501) [報表日 2026-11-12, 落後 2 日 ⚠️ 資料落後; 同步於 2026-11-14T05:50]
  * 現金結餘: HKD 0 / USD 7,218
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 106 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 36.062 USD | 21204 USD | 5.2% | 3444 USD | 19.4% | 6.5 | 0.86 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 278.72 USD | 9755 USD | 2.4% | 1325 USD | 15.7% | 27.8 | 0.9 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 342.75 USD | 17480 USD | 4.3% | -1408 USD | -7.4% | 26.1 | 1.24 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 355.429 USD | 19904 USD | 4.9% | 2778 USD | 16.2% | 5.8 | 0.88 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 161.39 USD | 35183 USD | 8.6% | - | - | 40.7 | 0.55 | - | Flex(2026-11-12) |
| IB | PLTR | 227.0 | 131.423413062 USD | 171.58 USD | 38949 USD | 9.6% | - | - | 14.1 | 0.6 | - | Flex(2026-11-12) |
| IB | QQQM | 434.0 | 249.066141779 USD | 283.39 USD | 122991 USD | 30.2% | - | - | 27.8 | 0.9 | - | Flex(2026-11-12) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.53 USD | 38905 USD | 9.5% | - | - | 12.3 | 0.92 | - | Flex(2026-11-12) |
| IB | SPCX | 122.0 | 140.002405574 USD | 139.94 USD | 17073 USD | 4.2% | - | - | 13.3 | 0.72 | - | Flex(2026-11-12) |
| IB | URA | 840.0 | 50.432105573 USD | 32.36 USD | 27182 USD | 6.7% | - | - | 24.3 | 0.83 | - | Flex(2026-11-12) |
| IB | VRT | 85.0 | 289.688176106 USD | 209.64 USD | 17819 USD | 4.4% | - | - | 32.5 | 0.7 | - | Flex(2026-11-12) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.9% | - | - | 40.6 | 0.53 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.2% | - | - | 34.3 | 0.82 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 6.0% | - | - | 27.8 | 0.9 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$407,441**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $368,536 = **90.5%** | 目標 90% | drift +0.5% ✅
  - 防禦 (defense: SGOV+現金): $46,578 = **11.4%** | 目標 10% | drift +1.4% ⚠️ 超配
  - 戶口現金: $7,673

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $139.11 | IV Rank: 13.3 | Vol/30dAvg: 0.72 | 下次財報: -
  * P: 最新價 $107.99 | IV Rank: 136.8 | Vol/30dAvg: 0.84 | 下次財報: -
  * AVGO: 最新價 $347.01 | IV Rank: 26.1 | Vol/30dAvg: 1.24 | 下次財報: -
  * QQQM: 最新價 $279.97 | IV Rank: 27.8 | Vol/30dAvg: 0.9 | 下次財報: -
  * URA: 最新價 $31.84 | IV Rank: 24.3 | Vol/30dAvg: 0.83 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 98.79 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 19.3 | VIX9D (9日短期): 17.82 | VIX9D/VIX Ratio: 0.92 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.2% (信用違約風險, >6%=壓力)
* FOMC 倒數: 24 天 (下次 2026-12-08)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| MU | $778.31 | 65 | 7.9 | 3.31% | 40.4 | 0.93x | -13.08% |
| TSM | $398.73 | 65 | 3.8 | 58.18% | 43.2 | 0.78x | -5.03% |
* 數據更新: 2026-11-14 05:34:02 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: MU (總分 65) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
