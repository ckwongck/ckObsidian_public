---
title: CK 投資組合最新數據包 (自動每日更新)
updated: 2026-10-22 06:00:56 HKT
source: portfolio_datapack.py (cron 06:00)
auto: true
note: 此檔由腳本自動生成，策略筆記請改 CK.md
---

=== [CK PORTFOLIO MAX DATA PACK v4.1] ===
* 數據提取時間 (HKT): 2026-10-22 06:00:48

## 一、 賬戶資金與流動性全景 (Liquidity & Buying Power) *v4.1 修復版*
* Futu 賬戶 (HKD/USD) — OpenD 即時:
  * 總資產估值: HKD 0 / USD 67,206
  * **實時現金結餘: USD 0 / HKD 0**
  * 剩餘購買力: 672,631 HKD+USD
* IB 賬戶 (HKD/USD) — Flex Web Service (每日 02:10 HKT snapshot):
  * 總資產估值: USD 317,675 (約 HKD 2,477,865) [報表日 2026-10-20, 落後 2 日 ⚠️ 資料落後; 同步於 2026-10-22T05:50]
  * 現金結餘: HKD -0 / USD 5,244
  * 剩餘購買力 / 可用保證金: [Flex 無此欄位 - 不適用]
  * 註: IB 使用 Flex Web Service (每日 02:10 HKT snapshot), 非即時. 即時需另起 IB Gateway.

* Firstrade 賬戶 (USD) — Apex Clearing 月結單 (manual copy, 無 API):
  * 總資產估值: USD 41,450 (約 HKD 323,309) [報表日 20260731, 落後 83 日 ⚠️ 資料落後]
  * 現金結餘: USD 455
  * 剩餘購買力 / 可用保證金: [月結單無此欄位 - 不適用]
  * 註: Firstrade 無公開 API, 月結單人手抄入 holdings_firstrade.json.

## 二、 實時持倉深度透視 + 微觀結構 X 光 (Full Positions + Micro-Structure) *v4.1*
| 賬戶 | 代號 | 股數 | 平均成本 | 最新市價 | 市值 | 佔總資產% | 累計P&L | 累計P&L% | IV Rank | Vol/30dAvg | 下次財報 | 數據來源 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Futu | US.SCHD | 588.0 | 30.206 USD | 34.66 USD | 20380 USD | 4.8% | 2619 USD | 14.8% | 15.1 | 0.86 | - | live-OpenD |
| Futu | US.QQQM | 35.0 | 240.873 USD | 298.22 USD | 10438 USD | 2.5% | 2007 USD | 23.8% | 21.2 | 0.87 | - | live-OpenD |
| Futu | US.AVGO | 51.0 | 370.35 USD | 335.67 USD | 17119 USD | 4.1% | -1769 USD | -9.4% | 16.6 | 0.73 | - | live-OpenD |
| Futu | US.AAPL | 56.0 | 305.83 USD | 343.99 USD | 19263 USD | 4.6% | 2137 USD | 12.5% | 7.0 | 0.88 | - | live-OpenD |
| IB | GRID | 218.0 | 196.402405573 USD | 167.91 USD | 36604 USD | 8.7% | - | - | 30.7 | 0.77 | - | Flex(2026-10-20) |
| IB | PLTR | 227.0 | 131.423413062 USD | 192.6 USD | 43720 USD | 10.4% | - | - | 42.6 | 0.9 | - | Flex(2026-10-20) |
| IB | QQQM | 434.0 | 249.066141779 USD | 295.59 USD | 128286 USD | 30.5% | - | - | 21.2 | 0.87 | - | Flex(2026-10-20) |
| IB | SGOV | 387.0 | 100.683505574 USD | 100.61 USD | 38936 USD | 9.3% | - | - | 2.6 | 0.97 | - | Flex(2026-10-20) |
| IB | SPCX | 122.0 | 140.002405574 USD | 147.79 USD | 18030 USD | 4.3% | - | - | 12.9 | 2.35 | - | Flex(2026-10-20) |
| IB | URA | 840.0 | 50.432105573 USD | 35.18 USD | 29551 USD | 7.0% | - | - | 46.7 | 0.76 | - | Flex(2026-10-20) |
| IB | VRT | 85.0 | 289.688176106 USD | 203.56 USD | 17303 USD | 4.1% | - | - | 55.8 | 1.17 | - | Flex(2026-10-20) |
| Firstrade | CEG | 29.0 | 272.2 USD | 262.75 USD | 7620 USD | 1.8% | - | - | 56.7 | 0.73 | - | Stmt(20260731) |
| Firstrade | GEV | 9.0 | 945.0 USD | 990.29 USD | 8913 USD | 2.1% | - | - | 48.4 | 1.32 | - | Stmt(20260731) |
| Firstrade | QQQM | 86.3518 | 299.4 USD | 283.29 USD | 24463 USD | 5.8% | - | - | 21.2 | 0.87 | - | Stmt(20260731) |

* 📊 總資產估值 (FX→USD, 已 exclude 媽媽資產): **$420,626**
* 🎯 90/10 陣型評估 (CK auth 2026-07-14):
  - 增長 (growth): $381,690 = **90.7%** | 目標 90% | drift +0.7% ✅
  - 防禦 (defense: SGOV+現金): $44,635 = **10.6%** | 目標 10% | drift +0.6% ✅
  - 戶口現金: $5,699

## 三、 觀察名單與掛單深度 (Watchlist & Order Book) + 微觀結構 *v4.1*
* 活動掛單 (Active Orders):
  1. [IB 掛單需 IB Gateway 先讀到; Flex read-only 讀唔到掛單. CK 喺 IB 落單]
* 觀察名單技術快照 + 微觀結構 X 光 (報價: Futu OpenD → yfinance fallback):
  * SPCX: 最新價 $159.31 | IV Rank: 12.9 | Vol/30dAvg: 2.35 | 下次財報: -
  * P: 最新價 $130.93 | IV Rank: 75.4 | Vol/30dAvg: 0.37 | 下次財報: -
  * AVGO: 最新價 $337.80 | IV Rank: 16.6 | Vol/30dAvg: 0.73 | 下次財報: -
  * QQQM: 最新價 $298.64 | IV Rank: 21.2 | Vol/30dAvg: 0.87 | 下次財報: -
  * URA: 最新價 $35.55 | IV Rank: 46.7 | Vol/30dAvg: 0.76 | 下次財報: -

## 四、 宏觀與風險雷達 (Macro Risk Radar) *v4.1 升級*
* MOVE Index: 95.94 (債市恐慌指標, >100=緊張)
* VIX (標普恐慌指數): 16.68 | VIX9D (9日短期): 15.49 | VIX9D/VIX Ratio: 0.93 (Ratio>1=短期恐慌升溫)
* PCC (Put/Call Ratio 全市場): 400.0 ( >1.2=極端恐慌/超賣反彈機會; <0.7=極端貪婪/頂部風險 )
* Sahm Rule: 400.0% (衰退指標, >0.5%=衰退信號)
* High-Yield Spread: 400.0% (信用違約風險, >6%=壓力)
* FOMC 倒數: 5 天 (下次 2026-10-27)

## 五、 Alpha 獵物名單 (Quant Screener) *v4.1 動態 AI 生態圈版*
* 掃描 [納斯達克 100 / 標普 500] 成份股 — 第0層硬門檻(市值>100億/30日均量>200萬/價>EMA200) + 第1層多因子計分(滿分100) — 僅列 總分>=65 前 3-5 隻
* 計分: 估值現金流(ROIC>15%+15/FCF>2%+15/EV-EBITDA<35+10) | 錯殺支撐(RSI30-52+15/價入EMA50±3%+10/12-1動能>0+10) | 微觀(Vol比>1.2+15/IV Rank<50+10)
| 代號 | 最新價 | 總分 | EV/EBITDA | FCF% | RSI | Vol比 | 距離 EMA50 % |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| TSM | $431.89 | 75 | 4.0 | 53.71% | 38.7 | 0.98x | -0.83% |
| META | $697.52 | 65 | 16.3 | 1.21% | 40.8 | 1.25x | +2.41% |
* 數據更新: 2026-10-22 05:34:21 HKT

## 六、建議行動 (Actionable Insights)
1. ✅ **陣型健康** — 90/10 drift 在 ±3% 內，保持現狀
2. 🎯 **Alpha 機會**: TSM (總分 75) — 考慮研究後分批建倉
3. 🐻 **極端恐慌 (PCC=400.0)** → 超賣反彈機會，考慮逢低分批吸納
4. 🚨 **Sahm Rule 觸發 (400.0%)** → 衰退信號，防禦為主
5. 📅 **FOMC 倒數 5 天** → 議息前市場波動加劇，避免重倉操作
6. 📊 **SPCX 成交異動** (Vol/Avg=2.4x) → 關注新聞/財報

=== [END OF MAX DATA PACK v4.1] ===
