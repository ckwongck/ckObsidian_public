---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-29 10:10:42 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-29 10:10:34

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 67,956
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 677,922 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 327,829 (約 HKD 2,557,070) [報表日 2026-10-27, 落後 2 日 ⚠️ 資料落後; 同步於 2026-10-29T10:10]
  * 現金結餘: HKD 56,457 / USD 5,242
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 90 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 35.34 USD | 20780 USD | 4.9% | 3019 USD | 17.0% | 21.5 | 0.93 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 294.19 USD | 10297 USD | 2.4% | 1866 USD | 22.1% | 21.4 | 0.85 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 341.21 USD | 17402 USD | 4.1% | -1486 USD | -7.9% | 58.8 | 1.0 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 346.55 USD | 19407 USD | 4.6% | 2280 USD | 13.3% | 24.0 | 0.91 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 167.05 USD | 36417 USD | 8.6% | - | - | 32.1 | 0.76 | - | Flex(2026-10-27) |
| IB | PLTR | 227.0 | 131.423413062 USD | 198.73 USD | 45112 USD | 10.6% | - | - | 53.5 | 0.91 | - | Flex(2026-10-27) |
| IB | QQQM | 434.0 | 249.066141779 USD | 296.96 USD | 128881 USD | 30.4% | - | - | 21.4 | 0.85 | - | Flex(2026-10-27) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.68 USD | 38963 USD | 9.2% | - | - | 2.9 | 0.69 | - | Flex(2026-10-27) |
| IB | SPCX | 122.0 | 140.002405574 USD | 148.58 USD | 18127 USD | 4.3% | - | - | 59.8 | 0.96 | - | Flex(2026-10-27) |
| IB | URA | 840.0 | 50.432105573 USD | 35.86 USD | 30122 USD | 7.1% | - | - | 54.5 | 1.08 | - | Flex(2026-10-27) |
| IB | VRT | 85.0 | 289.688176106 USD | 208.56 USD | 17728 USD | 4.2% | - | - | 86.5 | 3.58 | - | Flex(2026-10-27) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.8% | - | - | 61.0 | 0.65 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.1% | - | - | 66.6 | 2.43 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.8% | - | - | 21.4 | 0.85 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$424,229**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $385,266 = **90.8%** | 目標 90% | drift +0.8% ✅
  - 防禦 (defense: SGOV+現金): $51,898 = **12.2%** | 目標 10% | drift +2.2% ⚠️ 超配
  - 戶口現金: $12,935

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $145.23 | IV Rank: 59.8 | Vol/30dAvg: 0.96 | 下次財報: -
  * P: 最新價 $138.60 | IV Rank: 82.3 | Vol/30dAvg: 0.4 | 下次財報: -
  * AVGO: 最新價 $351.81 | IV Rank: 58.8 | Vol/30dAvg: 1.0 | 下次財報: -
  * QQQM: 最新價 $298.71 | IV Rank: 21.4 | Vol/30dAvg: 0.85 | 下次財報: -
  * URA: 最新價 $36.55 | IV Rank: 54.5 | Vol/30dAvg: 1.08 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 94.55 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 16.91 | VIX9D (9日短期): 15.6 | VIX9D/VIX Ratio: 0.92 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): None ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 0.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 3.18% (信用違約風險, >6%=壓力)
* FOMC 倒數: 40 天 (下次 2026-12-08)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| MU | $983.23 | 75 | 9.3 | 2.62% | 43.9 | 1.14x | +2.12% |
| TSM | $439.51 | 75 | 4.1 | 52.78% | 41.8 | 0.73x | +1.28% |
| FOXA | $63.39 | 75 | 7.9 | 2.08% | 49.4 | 1.30x | -1.00% |
* 數據更新: 2026-10-29 05:34:26 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: MU (總分 75) — 考慮研究後分批建倉

=== [END OF MAX DATA PACK v4.1] ===
