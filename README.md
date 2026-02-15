# Overnight-Hold-Indicator-Webull
#Does not work for backtesting due to Webull Scripting GAP missing a command like lookahead=barmerge.lookahead_off : This is a strict rule that prevents the code from "cheating" or looking into the future. It ensures that if you are looking at historical data, the script only uses the daily volume data that was actually available at that exact moment in time, keeping your backtesting accurate. Webull Script is missing this feature therefore backtesting is not possible.

Overnight Hold Indicator in Webull Script for Webull Desktop
Daily Timeframe Use Only
Based on Irish Born Ivestor's indicator for TradingView https://www.tradingview.com/script/Ygz1n8bc-Over-Night-Hold-Scanner-Born-Investor/
This Webull Script indicator is built to isolate high-probability overnight hold (ONH) setups, strictly adapting IrishBornIVestor code for TradingView. Scans for explosive volume (2x+ average), strong closes in the top 15% of the range, and momentum context—MUST onlye be used on DAILY chart timeframe.

Key Features
Strict Daily Context: Runs on any chart due to Webull functions but should only be used looking at the daily chart.

Setup Scoring: Automatically evaluates and scores both relative volume (RVOL) and closing strength.

Baseline Liquidity Filters: Configured to weed out the noise (requires a minimum $3 price and 1M+ average daily volume).

Actionable Context: Detects trend continuation and reversal setups based on the day's price action.
