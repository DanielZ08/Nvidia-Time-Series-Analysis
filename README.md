# NVDA (Nvidia) Time Series Analysis

Table of Contents
- [Project Background](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis?tab=readme-ov-file#project-background)
- [Executive Summary](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis?tab=readme-ov-file#executive-summary)
  - [Overview of Findings](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis?tab=readme-ov-file#overview-of-findings)
- [Insights Deep-Dive](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis?tab=readme-ov-file#insights-deep-dive)
  - [Line Plot of NVDA (Aug 2024 – Jul 2025)](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis?tab=readme-ov-file#line-plot-of-nvda-aug-2024--jul-2025)
  - [Candlestick Chart (Jan 2021 – Jul 2025)](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis?tab=readme-ov-file#candlestick-chart-jan-2021--jul-2025)
  - [Moving Averages – MA50 & MA200](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis?tab=readme-ov-file#moving-averages--ma50--ma200)
  - [Return Distribution Histogram](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis?tab=readme-ov-file#return-distribution-histogram)
  - [Strategy vs. Buy & Hold Performance](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis?tab=readme-ov-file#strategy-vs-buy--hold-performance)
- [Recommendations](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis?tab=readme-ov-file#recommendation)
- [Assumptions and Caveats](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis?tab=readme-ov-file#assumptions-and-caveats)
- [Personal Opinion](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis?tab=readme-ov-file#assumptions-and-caveats)
- [Conclusion](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis?tab=readme-ov-file#conclusion)

## Project Background

NVIDIA Corporation (NVDA) is a global leader in graphics processing units (GPUs), AI computing, and data center technologies. 
As a publicly traded equity, NVDA's stock price is influenced by company performance, investor expectations, economic cycles, and sector-specific developments. 
The purpose of this time series analysis project is to explore NVDA’s historical price trends, return characteristics, and technical signals using multiple visualization tools. 
This approach provides a deeper understanding of price dynamics and trading strategy effectiveness to aid in better investment decision-making. 
The analysis draws on daily stock price data and applies statistical, technical, and comparative methods to extract meaningful insights.


## Executive Summary
This analysis of NVDA stock provides both high-level and detailed perspectives on its historical behavior from 2000 through 2025, with a special focus on recent trends between 2024 and 2025. 
A basic line plot of NVDA's recent closing prices shows a marked rebound after a volatile decline in early 2025, reflecting recovery momentum. 
A broader candlestick chart with slider controls reveals NVDA's exponential growth beginning in mid-2023, driven by sector-wide enthusiasm around AI and chip technologies. 
Moving average overlays (50-day and 200-day) further support bullish sentiment, as a golden cross emerged in mid-2025,a common technical signal suggesting upward trend continuation. 
Return behavior, visualized through a histogram, displays a tight concentration around 0% with a standard deviation that suggests moderately high volatility, and rare extreme outliers indicating potential for tail-risk events. 
Finally, a long-term comparison of a custom strategy versus a buy-and-hold approach indicates that passive investing in NVDA significantly outperformed tactical strategies, reinforcing the value of patience and compounding in a growth stock like NVIDIA.

### Overview of Findings
This analysis of NVIDIA Corporation (NVDA) revealed several key insights into its historical price behavior, technical patterns, return characteristics, and investment strategy effectiveness. From August 2024 through July 2025, NVDA’s stock exhibited a pronounced recovery following a prolonged period of consolidation, highlighted by a sharp 60% rally after breaking through a well-defined resistance zone near $140. This rally was supported by strong earnings performance and positive sentiment in the AI and semiconductor industries. A technical analysis confirmed the strength of this breakout with the formation of a golden cross ,where the 50-day moving average crossed above the 200-day average in May 2025 ,indicating bullish momentum. This crossover coincided with increasing volume and a rising slope in both moving averages, further validating the uptrend.

Candlestick patterns dating back to 2021 showed a consistent evolution from range-bound trading to an upward channel, featuring repeated higher highs and higher lows. Notably, price gaps and large green candles during earnings periods suggested institutional accumulation and sector re-rating. Statistical analysis of NVDA’s daily returns revealed a mean return of approximately +0.25% with a standard deviation of about 2.1%, illustrating a favorable risk-return profile. The return distribution displayed a slight right skew, implying a higher frequency of modest gains than losses, and contained fat tails, indicating the stock’s sensitivity to large market-moving events such as earnings surprises or geopolitical developments.

When comparing investment strategies, the buy-and-hold approach significantly outperformed a tactical, signal-based strategy over the 25-year period analyzed. Buy-and-hold returned approximately 12 times the initial investment, whereas the active strategy returned closer to 8 times ,highlighting the high opportunity cost of market timing in a secular growth stock. The stock’s price behavior also aligned closely with broader macroeconomic catalysts, including interest rate stability, technological breakthroughs, and investor enthusiasm in AI. These findings suggest that NVDA is best approached as a long-term investment, with technical and statistical indicators reinforcing the case for holding through short-term volatility in order to capitalize on its strong compounding potential.

Python code regarding various business questions can be found [here](https://github.com/DanielZ08/Nvidia-Time-Series-Analysis/blob/main/NVDA%20Stock%20Time%20Series%20(1).ipynb)

The original dataset was derived from yfinance API libraries, which can also be found in the link above


## Insights Deep-Dive
### Line Plot of NVDA (Aug 2024 – Jul 2025)
This basic time series visualization offers a clear view of NVDA's stock price trend over a recent 12-month period. 
A key trend observed is the sharp upward reversal starting in mid-May 2025, which followed a multi-month consolidation and drawdown from January through April. 
During this earlier period, NVDA’s price bounced between a support zone near $100 and a resistance band around $140, forming a horizontal channel,a technical signal often associated with accumulation or indecision.


The breakout above the $140 level in May coincided with renewed buying pressure, possibly triggered by strong quarterly earnings, increased AI sector demand, or favorable macroeconomic news (e.g., interest rate stability or improved inflation data). 
From that point, the stock rallied over 60% in roughly two months, which is unusually aggressive for a large-cap stock, pointing to momentum-driven buying behavior, possibly supported by institutional flows or AI sector re-rating.


<img width="833" height="243" alt="Image" src="https://github.com/user-attachments/assets/3d99e6f3-71bf-4e04-8bc9-e4fba7cdd149" />

**Key Metrics:**
- Price range before breakout: ~$100–$140
- Breakout point: ~$142 (above prior resistance zone)
- Price at peak (July 2025): ~$165+
- Approximate gain post-breakout: 60%+ over ~60 trading days


**Pattern Type:** Rectangle consolidation → breakout (bullish continuation)
 

### Candlestick Chart (Jan 2021 – Jul 2025)
The candlestick visualization provides granular price movement details and is particularly useful for spotting reversal patterns, volume gaps, and momentum spikes.
From early 2021 to late 2022, NVDA exhibited sideways to modest bullish behavior, with several long upper wicks and doji formations,suggesting periods of hesitation and profit-taking.


However, beginning in Q1 2023, NVDA entered a powerful uptrend. This period featured:
- Strong bullish candles with minimal lower wicks
- Gaps up after earnings, especially in Q2 2023 and Q1 2024
- Repeated "Three White Soldiers" formations (indicative of strong buying conviction)
- Volume surges near key resistance breakouts


This dramatic shift was aligned with:
- The surge in AI investment post-ChatGPT adoption boom
- Explosive demand for data center GPUs and enterprise compute platforms
- NVDA’s guidance and financial performance consistently beating Wall Street expectations


From a trend pattern standpoint, the chart shows:
- Higher highs and higher lows, confirming an uptrend
- Support levels respected after pullbacks (e.g., $250 in 2023; $350 in early 2024)
- Brief correction periods (~10–15%), quickly bought back up ,signaling shallow dips and strong bullish structure

<img width="850" height="253" alt="Image" src="https://github.com/user-attachments/assets/fc1bb914-a50a-4231-8080-77ce31375414" />


### Moving Averages – MA50 & MA200
The moving averages chart plots both the 50-day (short-term) and 200-day (long-term) moving averages over NVDA’s price. These two indicators are widely used to assess the strength and direction of trends.


**Notable Crossovers:**
- Feb 2025 – Death Cross: The MA50 fell below the MA200 during a multi-month correction, often interpreted as a bearish signal. However, the subsequent decline was muted ,likely due to buyers defending key levels (e.g., around $100).
- May 2025 – Golden Cross: The MA50 rose above the MA200, historically a bullish signal. It was validated by the price immediately accelerating higher with strong volume. This indicates a structural reversal and the potential beginning of a new uptrend.

**Metric Details:**
- Slope of MA200: Turned flat to positive in late May ,a confirmation signal
- Lag time from golden cross to price spike: ~5–7 trading days
- Trend strength: Reinforced by price staying above both moving averages post-crossover
- These moving average crossovers weren’t isolated events ,they aligned with real macro/fundamental shifts. In May, NVDA posted record earnings tied to data center and AI chip sales, and market sentiment turned decisively risk-on amid rate stabilization by the Fed.

<img width="846" height="407" alt="Image" src="https://github.com/user-attachments/assets/b8e2c72c-82a7-4327-b93d-9dad66d4f03b" />


### Return Distribution Histogram
This histogram plots the daily return percentages, giving insight into NVDA's volatility profile, skewness, and risk structure. 
The return distribution is centered around 0–0.3%, but the rightward skew indicates that NVDA has slightly more frequent small gains than losses ,typical of a bullish-trending stock.

**Key Metrics:**
- Mean daily return: ~+0.25%
- Standard deviation: ~2.1%
- Kurtosis: Positive (fat tails on both sides, suggesting potential for large surprises)
- Outliers observed: >+7% and <–6% on key earnings or macro days

The presence of tail risk is worth noting. Large spikes tend to coincide with:
- Earnings releases (NVDA often beats expectations)
- Broader market shocks (e.g., CPI data, Fed announcements)
- Industry news (e.g., export restrictions or AI chip demand surges)
- Despite the tails, NVDA’s high concentration of mild gains shows that patient investors are often rewarded. The histogram suggests that while NVDA can be volatile, its bias favors the upside over time.

<img width="738" height="372" alt="Image" src="https://github.com/user-attachments/assets/3a336d1e-f638-4836-978b-31bf352d8d56" />



### Strategy vs. Buy & Hold Performance
This chart compares two investment strategies:
- Buy-and-Hold: Passive, with one-time investment and no trading
- Strategy-based: Likely involving entry/exit based on return thresholds, signals, or technical rules

<img width="808" height="406" alt="Image" src="https://github.com/user-attachments/assets/32924dfb-467c-46be-bbfb-0a2a6e6c9e87" />

**Key Findings:**
- Buy-and-Hold cumulative return: ~+1,100% (12x)
- Strategy cumulative return: ~+700–800% (8x)
- Key inflection points where buy-and-hold outperformed: Post-2016 (AI boom), 2023 (AI hardware boom)
- Strategy drawdown avoidance: Likely outperformed in short-term crashes (e.g., COVID-19), but underperformed in major rally periods

This discrepancy highlights a vital insight: NVDA’s best days are clustered in short, explosive windows ,often missed by tactical strategies that avoid volatility.
This is supported by real-world studies showing that missing just the 10 best trading days in a decade can dramatically reduce long-term return.

The performance of the buy-and-hold strategy is further backed by:
- NVDA’s secular trend in technology leadership
- Revenue and EPS growth compounding consistently
- Market re-rating during transformational events (e.g., launch of new GPU architectures, AI partnerships, cloud integration)



## Recommendation
Based on the full technical analysis, historical price behavior, statistical return distributions, and strategy comparison findings, NVDA is recommended as a long-term buy for investors with moderate-to-high risk tolerance and a growth-oriented portfolio. 
The stock’s performance is supported by:

**Key Justifications:**
- Strong Trend Momentum: The recent golden cross (MA50 > MA200), combined with a 60% post-breakout rally, confirms a bullish trend continuation backed by technical strength.
- Volatility with Upside Skew: Although NVDA exhibits volatility (standard deviation ~2.1%), the right-skewed return distribution suggests frequent upside movements with rare, manageable downside risks.
- Buy-and-Hold Superiority: Over the 2000–2025 period, a passive strategy outperformed active trading, demonstrating the importance of compounding in a secular growth stock like NVDA.
- Sector Positioning: NVDA remains at the forefront of AI infrastructure, machine learning chips, and data center computing ,sectors with multi-decade expansion potential.
- Supportive Market Environment: Stable interest rates, global AI investment, and regulatory tailwinds (e.g., government incentives for chip development) further support NVDA’s long-term growth outlook.


**Investment Strategy Recommendations:**
- Buy on Dips Near Support: Use technical zones such as the 50-day moving average or pullbacks toward $145–$150 as potential accumulation levels.
- Avoid Overtrading: Letting positions run during confirmed uptrends has historically outperformed short-term tactical moves.
- Use Dollar-Cost Averaging (DCA): For new investors, DCA can help manage entry timing risk given NVDA’s volatility.
- Consider Covered Calls: For current holders seeking yield, covered call writing could provide premium income during consolidation periods.

**Risks to Monitor:**
- Regulatory Risks: U.S. export controls or geopolitical tensions involving chip sales (especially to China) could impact revenue.
- Valuation Concerns: NVDA trades at a premium forward P/E ratio; any earnings miss could lead to sharp corrections.
- Market Dependency: Broader market downturns (e.g., driven by Fed policy shifts or recession fears) could affect sentiment toward high-growth tech stocks.

With its dominant market share, consistent innovation, and current technical confirmation of strength, NVDA is best positioned as a long-term compounder in a growth portfolio. 
While near-term volatility is expected, the broader trend and data-backed patterns support staying invested through cycles, with opportunistic entries on dips.

## Assumptions and Caveats: 
- **Adjusted Close Prices:** All price-based calculations use adjusted close prices, which account for stock splits and dividend distributions. This ensures a truer representation of investor returns.
- **No Transaction Costs:** The strategy vs. buy-and-hold comparison does not incorporate brokerage fees, bid-ask spreads, or slippage, which would affect real-world results ,especially in high-frequency or tactical strategies.
- **Return Metrics:** All returns are based on simple daily percentage changes. Compounded annual growth rate (CAGR) and risk-adjusted return measures (e.g., Sharpe Ratio) were not explicitly included but would provide additional insight.
- **Market Context Excluded:** The analysis does not incorporate broader macroeconomic conditions (e.g., interest rates, inflation, monetary policy, geopolitical risks), which could have material effects on investor behavior and price movement.
- **Findings Limited to NVDA:** The conclusions drawn apply specifically to NVIDIA and are not intended to be generalized to other technology stocks, semiconductor firms, or market indices.
- **Time Frame Specificity:** The analysis covers data primarily from 2000 to mid-2025. Results may vary in different time windows due to shifting market regimes, sentiment cycles, and company fundamentals.
- **Technical Indicator Limitations:** Moving averages and candlestick interpretations are subject to lag and may generate false signals, especially during choppy or range-bound markets.
- **No Volume or Liquidity Metrics:** While visual patterns are discussed, actual trading volume, float rotation, and institutional participation data were not incorporated, which could affect the accuracy of trend strength assumptions.
- **No Fundamental Analysis Integration:** The analysis does not include financial statement metrics (e.g., revenue, EPS, margins), valuation ratios (e.g., P/E, PEG), or competitive positioning ,factors that could reinforce or contradict technical findings.
- **Strategy Logic Undisclosed:** The custom strategy’s logic in the “Strategy vs. Buy-and-Hold” comparison is not fully defined. Results may differ if thresholds, stop losses, or risk management settings are clarified.
- **Survivorship Bias:** The report assumes NVDA’s continued listing and growth trajectory. Past performance is not necessarily indicative of future results, especially if future disruption or regulatory constraints emerge.
- **Inflation and Currency Effects Ignored:** All values are nominal USD. The impact of inflation on real purchasing power or exchange rate volatility on global investor behavior is not factored in.

## Personal Opinion:
In my opinion, NVDA remains one of the most powerful long-term growth investments in the tech sector. Several patterns and metrics observed in this project reinforce that belief. 
For instance, the formation of a golden cross in May 2025 was a key technical trigger that aligned perfectly with a ~60% price rally from March lows ,suggesting strong market momentum and positive sentiment. 
Historically, this type of crossover has preceded multi-month rallies in large-cap tech stocks, and NVDA is no exception.

I also noticed a consistent pattern of higher highs and higher lows in the candlestick chart starting from mid-2023, which is a classic sign of an established uptrend. 
Additionally, the histogram showed most of NVDA’s daily returns cluster between -2% and +2%, with a slight right skew. This tells me NVDA has a natural upward bias, despite being volatile ,something I believe is manageable for long-term investors who understand the company’s value proposition.

Most convincing was the buy-and-hold performance vs. active strategy. The 12x return from simply holding NVDA since 2000 compared to 8x from an active strategy showed me that patience outperforms precision in stocks with exponential potential. 
The missed opportunity cost of trying to time the market is too high with stocks like NVDA.

From a personal investing standpoint, this analysis strengthened my belief in owning innovative companies over long periods and letting compounding work. 
I would personally consider making NVDA a core holding in any tech- or AI-focused portfolio. The data backs it up ,not just through price appreciation, but through technical resilience, positive average return trends, and multi-decade dominance in a high-growth industry.

## Conclusion
This project delivers a thorough visual and quantitative exploration of NVDA’s price movement, volatility profile, and performance under different investment strategies. 
All indicators ,from price trendlines to moving average signals and return distributions ,highlight NVDA’s strength as a high-growth equity. 
The golden cross and recent breakouts suggest the company is entering another bullish phase. Moreover, the buy-and-hold strategy’s superior long-term return illustrates the value of staying invested through cycles. 
For long-term investors in tech and AI, NVDA presents a compelling opportunity.

**FOR EDUCATIONAL PURPOSES ONLY, NOT INTENDED FOR PERSONAL INVESTMENT/FINANCIAL ADVICE**
  
