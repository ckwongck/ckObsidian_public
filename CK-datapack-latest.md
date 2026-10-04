---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-05 06:00:15 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-05 06:00:07

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 49,975 / USD 66,842
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 653,136 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 334,976 (約 HKD 2,612,812) [報表日 2026-10-02, 落後 3 日 ⚠️ 資料落後; 同步於 2026-10-05T05:50]
  * 現金結餘: HKD -0 / USD 5,162
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 66 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 32.72 USD | 19239 USD | 4.4% | 1479 USD | 8.3% | 17.2 | 0.89 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 308.69 USD | 10804 USD | 2.5% | 2374 USD | 28.1% | 17.5 | 1.16 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 355.14 USD | 18112 USD | 4.1% | -776 USD | -4.1% | 30.0 | 0.98 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 333.69 USD | 18687 USD | 4.3% | 1560 USD | 9.1% | 19.3 | 0.81 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 182.91 USD | 39874 USD | 9.1% | - | - | 31.9 | 2.17 | - | Flex(2026-10-02) |
| IB | PLTR | 227.0 | 131.423413062 USD | 188.75 USD | 42846 USD | 9.8% | - | - | 42.6 | 0.68 | - | Flex(2026-10-02) |
| IB | QQQM | 434.0 | 249.066141779 USD | 308.69 USD | 133971 USD | 30.6% | - | - | 17.5 | 1.16 | - | Flex(2026-10-02) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.44 USD | 38870 USD | 8.9% | - | - | 3.9 | 1.12 | - | Flex(2026-10-02) |
| IB | SPCX | 122.0 | 140.002405574 USD | 158.96 USD | 19393 USD | 4.4% | - | - | 44.5 | 1.43 | - | Flex(2026-10-02) |
| IB | URA | 840.0 | 50.432105573 USD | 39.79 USD | 33424 USD | 7.6% | - | - | 48.9 | 0.6 | - | Flex(2026-10-02) |
| IB | VRT | 85.0 | 289.688176106 USD | 252.18 USD | 21435 USD | 4.9% | - | - | 52.6 | 0.68 | - | Flex(2026-10-02) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.7% | - | - | 51.3 | 1.31 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.0% | - | - | 51.1 | 1.0 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.6% | - | - | 17.5 | 1.16 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$437,652**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $398,781 = **91.1%** | 目標 90% | drift +1.1% ⚠️ 超配
  - 防禦 (defense: SGOV+現金): $44,487 = **10.2%** | 目標 10% | drift +0.2% ✅
  - 戶口現金: $5,616

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $158.96 | IV Rank: 44.5 | Vol/30dAvg: 1.43 | 下次財報: -
  * P: 最新價 $140.14 | IV Rank: 61.0 | Vol/30dAvg: 0.76 | 下次財報: -
  * AVGO: 最新價 $355.14 | IV Rank: 30.0 | Vol/30dAvg: 0.98 | 下次財報: -
  * QQQM: 最新價 $308.69 | IV Rank: 17.5 | Vol/30dAvg: 1.16 | 下次財報: -
  * URA: 最新價 $39.79 | IV Rank: 48.9 | Vol/30dAvg: 0.6 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 107.29 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 15.31 | VIX9D (9日短期): 12.06 | VIX9D/VIX Ratio: 0.79 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.24% (信用違約風險, >6%=壓力)
* FOMC 倒數: 22 天 (下次 2026-10-27)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
*今日無標的達標，AI 陣營缺乏黃金坑，維持戰略靜默。*

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀

=== [END OF MAX DATA PACK v4.1] ===
