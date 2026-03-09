# Daily Crypto Industry Digest

## Prompt

I'm President of Ripple. I want to start each morning with a brief digest of only the key developments in the crypto and blockchain industry, sourced from credible media and notable social accounts. Not everything - just what matters.

Using the attached `news_sources.csv` (a sample day's worth of news items from various sources), build me a daily digest tool that:

1. **Filters for signal** - From the raw news items, select only the ones that matter for someone in my position. Filter criteria:
   - Directly relevant to Ripple's business lines (payments, custody, stablecoins, prime brokerage, treasury)
   - Competitive moves by SWIFT, Stellar, Circle, JPMorgan, Visa, or other payment/blockchain players
   - Regulatory developments (SEC, CFTC, international regulators, legislation)
   - Major institutional adoption moves (banks, asset managers, payment processors entering crypto)
   - Market-moving events (significant price moves, ETF flows, major hacks/failures)
   - Ignore: memecoins, NFT drops, minor altcoin news, pure retail speculation

2. **Daily Digest Format** (HTML email-style):
   - **Date and Reading Time** estimate at top
   - **Top 3 Stories** - The most important items with 2-3 sentence summaries and why they matter for Ripple specifically
   - **Regulatory Watch** - Any regulatory developments, organized by jurisdiction
   - **Competitive Radar** - What our competitors did/said
   - **Market Snapshot** - XRP price, BTC, ETH, RLUSD metrics, total crypto market cap, XRP ETF flows
   - **Worth Watching** - 2-3 emerging stories that aren't urgent but worth tracking

3. **Source Credibility** - Weight information from tier-1 sources (Bloomberg, Reuters, FT, WSJ, CoinDesk, The Block) higher than social media. Flag anything that's unverified or single-source.

Output as a clean, scannable HTML file that looks like a premium morning briefing. Should take 5 minutes to read.
