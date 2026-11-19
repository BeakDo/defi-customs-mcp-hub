# DeFi Arbitrage, Prediction Odds, Korea Import Customs & B2B Remote MCP Hub

Zero-install Streamable HTTP (`2025-03-26`) **Model Context Protocol (MCP)** servers and live web calculators running on Cloudflare Edge, paired with bulk Pay-Per-Event extraction Actors on Apify Cloud.

Connect **Claude Desktop, Cursor, Windsurf, Cline, VS Code Copilot**, or custom Python and TypeScript agents directly via HTTPS URL with zero local Docker containers and zero API keys.

---

## Live Interactive Calculators & Terminals (Browser Ready)

### 1. Global & DeFi Arbitrage Terminals
1. **4-Venue Perpetual Funding Rate Arbitrage Scanner (Bitget, Hyperliquid, Kraken, Bybit)**: https://defi-route-intel.b2bintel-edge.workers.dev/bitget-funding-arbitrage
2. **Delta-Neutral Net Carry & Fee Break-Even Simulator**: https://defi-route-intel.b2bintel-edge.workers.dev/net-carry-calculator
3. **Pendle Fixed Yield (PT) vs Perp Funding Carry Monitor**: https://defi-route-intel.b2bintel-edge.workers.dev/ko/pendle
4. **Kalshi vs Polymarket Cross-Venue Prediction Market Odds**: https://defi-route-intel.b2bintel-edge.workers.dev/ko/prediction-markets
5. **Cross-Border Freelancer Invoice & L2 USDC Payout Fee Calculator**: https://smart-deal-calculator.b2bintel-edge.workers.dev/global-payouts
6. **SPF, DMARC, MX & Disposable Domain Deliverability Grader**: https://email-security-deliverability-grader.b2bintel-edge.workers.dev

### 2. 한국어 실전 계산기 모음 (Korean Calculators)
1. **비트겟(Bitget) 선물 수수료 계산기, 초대코드 혜택 및 실시간 펀딩비 차익 터미널**: https://defi-route-intel.b2bintel-edge.workers.dev/ko/bitget-fee-rebate
2. **선물 펀딩비 아비트라지 왕복 수수료 및 손익분기 시간 계산기**: https://defi-route-intel.b2bintel-edge.workers.dev/ko/net-carry
3. **알리익스프레스 할인코드, 코인할인, 카드할인 150달러 무관세 역산기**: https://smart-deal-calculator.b2bintel-edge.workers.dev/ali-promo-calculator
4. **해외직구 관부가세 계산기 (달러, 엔화, 유로, 위안화) vs 쿠팡 로켓배송 비교기**: https://smart-deal-calculator.b2bintel-edge.workers.dev
5. **맥미니 M4 및 아이패드 일본 엔화 직구 부가세 10% 비교기**: https://smart-deal-calculator.b2bintel-edge.workers.dev/mac-mini-apple-customs
6. **그래픽카드(RTX 5070, 5080) 및 PC 부품 직구 관부가세 비교기**: https://smart-deal-calculator.b2bintel-edge.workers.dev/gpu-pc-parts-customs

---

## Quick Connect (Remote MCP Configuration)

Add any or all of the four remote MCP servers to `claude_desktop_config.json`, `.cursor/mcp.json`, or Windsurf `mcp_config.json`:

```json
{
  "mcpServers": {
    "defi-route-intel": {
      "url": "https://defi-route-intel.b2bintel-edge.workers.dev/mcp"
    },
    "korea-customs-and-deal": {
      "url": "https://smart-deal-calculator.b2bintel-edge.workers.dev/mcp"
    },
    "b2b-domain-and-lead-intel": {
      "url": "https://b2b-intel-rapidapi-worker.b2bintel-edge.workers.dev/mcp"
    },
    "email-deliverability-grader": {
      "url": "https://email-security-deliverability-grader.b2bintel-edge.workers.dev/mcp"
    }
  }
}
```

---

## Available MCP Tools by Endpoint

### 1. `defi-route-intel` (`https://defi-route-intel.b2bintel-edge.workers.dev/mcp`)
1. `scan_perp_funding_spreads`: Real-time annualized perpetual funding rate spreads across **Bitget USDT-M Futures (`890` markets)**, **Hyperliquid L1**, **Kraken Futures**, and **Bybit Linear Perps**.
2. `compare_pendle_fixed_vs_funding`: Compares live Pendle Principal Token (PT) fixed implied APYs on Ethereum and Arbitrum against perpetual funding carry benchmarks.
3. `scan_prediction_market_odds`: Live implied YES probabilities and cross-venue probability gaps across **Kalshi** and **Polymarket**.
4. `get_institutional_stable_yields`: Verified `$10M+` TVL DefiLlama stablecoin vaults separating organic base fee APY from token emission incentives.
5. `quote_crosschain_usdc_bridge`: Net USDC received, gas cost, and bridge fees across Arbitrum, Base, Optimism, Ethereum, and Polygon via LI.FI plus Solana Jupiter swap benchmarks.
6. `check_krw_kimchi_premium`: Live Upbit KRW spot prices and implied `KRW-USDT` FX spreads against global USD mark prices.

### 2. `korea-customs-and-deal` (`https://smart-deal-calculator.b2bintel-edge.workers.dev/mcp`)
1. `calculate_korea_import_customs`: Computes South Korean import duty, VAT, customs clearance fees, and landed KRW cost across USD, JPY, EUR, and CNY vs domestic retail delivery.
2. `compare_crossborder_payout_fees`: Compares net USD and KRW take-home pay across L2 USDC settlement, Wise mid-market FX, SWIFT bank wires, and PayPal commercial invoices.

### 3. `b2b-domain-and-lead-intel` (`https://b2b-intel-rapidapi-worker.b2bintel-edge.workers.dev/mcp`)
1. Live B2B corporate domain tech stack detection (`48` SaaS signatures), DNS/RDAP verification, Oracle NetSuite SuiteApp ERP partner directory intelligence (`724` ISVs), FDA 510(k) clearances, US federal contract awards, and SEC Form D filings.

### 4. `email-deliverability-grader` (`https://email-security-deliverability-grader.b2bintel-edge.workers.dev/mcp`)
1. Live SPF, DMARC, MX, and disposable-domain security grading via DNS-over-HTTPS.

---

## Scheduled Bulk Extraction on Apify Cloud (`BeakDo`)

For automated CSV, JSON, Webhook, n8n, Make, or Zapier pipelines with `$0.00` start fees:
- Profile & Storefront: https://apify.com/beakdo
- NetSuite SuiteApp ERP Partners: https://apify.com/beakdo/netsuite-suiteapp-leads-scraper
- SEC Form D Funded Startups: https://apify.com/beakdo/sec-form-d-funding-scraper
- Greenhouse, Lever & Ashby Hiring Signals: https://apify.com/beakdo/ats-career-signal-sniper
- Workday & SmartRecruiters Enterprise Jobs: https://apify.com/beakdo/workday-jobs-scraper
- Website Contact & Tech Stack Enricher: https://apify.com/beakdo/website-contact-tech-scraper
- Shopify B2B & D2C Store Intelligence: https://apify.com/beakdo/shopify-b2b-store-intel

## License

MIT License. Non-custodial informational calculators and public-data MCP tools only; nothing herein constitutes financial, tax, customs-brokerage, or investment advice.
