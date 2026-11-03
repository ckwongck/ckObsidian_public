---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-11-04 06:00:27 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-11-04 06:00:19

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 66,466
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 665,177 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 305,496 (約 HKD 2,382,870) [報表日 2026-11-02, 落後 2 日 ⚠️ 資料落後; 同步於 2026-11-04T05:50]
  * 現金結餘: HKD 0 / USD 5,242
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 96 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 35.51 USD | 20880 USD | 5.1% | 3119 USD | 17.6% | 23.6 | 0.94 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 283.38 USD | 9918 USD | 2.4% | 1488 USD | 17.6% | 30.9 | 1.42 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 336.43 USD | 17158 USD | 4.2% | -1730 USD | -9.2% | 50.2 | 0.77 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 330.44 USD | 18505 USD | 4.5% | 1378 USD | 8.1% | 27.3 | 1.55 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 164.28 USD | 35813 USD | 8.8% | - | - | 42.0 | 0.73 | - | Flex(2026-11-02) |
| IB | PLTR | 227.0 | 131.423413062 USD | 178.34 USD | 40483 USD | 9.9% | - | - | 63.9 | 2.31 | - | Flex(2026-11-02) |
| IB | QQQM | 434.0 | 249.066141779 USD | 280.49 USD | 121733 USD | 29.9% | - | - | 30.9 | 1.42 | - | Flex(2026-11-02) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.43 USD | 38866 USD | 9.5% | - | - | 9.4 | 0.86 | - | Flex(2026-11-02) |
| IB | SPCX | 122.0 | 140.002405574 USD | 136.37 USD | 16637 USD | 4.1% | - | - | 70.6 | 0.74 | - | Flex(2026-11-02) |
| IB | URA | 840.0 | 50.432105573 USD | 32.93 USD | 27661 USD | 6.8% | - | - | 56.2 | 0.73 | - | Flex(2026-11-02) |
| IB | VRT | 85.0 | 289.688176106 USD | 224.24 USD | 19060 USD | 4.7% | - | - | 78.5 | 0.82 | - | Flex(2026-11-02) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.9% | - | - | 63.2 | 0.75 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.2% | - | - | 67.3 | 1.14 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 6.0% | - | - | 30.9 | 1.42 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$407,710**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $368,843 = **90.5%** | 目標 90% | drift +0.5% ✅
  - 防禦 (defense: SGOV+現金): $44,564 = **10.9%** | 目標 10% | drift +0.9% ✅
  - 戶口現金: $5,697

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $141.31 | IV Rank: 70.6 | Vol/30dAvg: 0.74 | 下次財報: -
  * P: 最新價 $117.65 | IV Rank: 101.2 | Vol/30dAvg: 0.5 | 下次財報: -
  * AVGO: 最新價 $332.13 | IV Rank: 50.2 | Vol/30dAvg: 0.77 | 下次財報: -
  * QQQM: 最新價 $282.23 | IV Rank: 30.9 | Vol/30dAvg: 1.42 | 下次財報: -
  * URA: 最新價 $33.05 | IV Rank: 56.2 | Vol/30dAvg: 0.73 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 99.97 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 20.83 | VIX9D (9日短期): 21.96 | VIX9D/VIX Ratio: 1.05 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.43% (信用違約風險, >6%=壓力)
* FOMC 倒數: 34 天 (下次 2026-12-08)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| FOXA | $67.10 | 65 | 6.4 | 4.39% | 61.9 | 1.91x | +4.69% |
* 數據更新: 2026-11-04 05:34:09 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: FOXA (總分 65) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
