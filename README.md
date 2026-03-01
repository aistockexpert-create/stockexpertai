# stockexpertai
Multi-agent AI War Room simulating legendary investors (Buffett, Dalio, Simons) for stock analysis. 174k+ lines of TypeScript.

# Stock Expert AI: The Multi-Agent Investment War Room

**Live at:** [www.stockexpertai.com](https://www.stockexpertai.com)

## The Core Philosophy: OpEx Collapse via Trusted Agents
While Big Tech is trapped in a CapEx doom loop, we are focusing on the total collapse of OpEx. Stock Expert AI replaces a $50k/year financial advisor conversation with a high-fidelity, deterministic AI audit.

## Architecture Deep Dive
- **174,127 lines of TypeScript** across 743 files.
- **Deterministic Engine:** We don't just "chat." We run math first. The system calculates ROE, D/E, and FCF Yield before the LLM even sees the ticker.
- **Multi-Agent Orchestration (The Council):**
  - **Buffett Agent:** Moat analysis and owner earnings.
  - **Dalio Agent:** Macro regime and debt cycle positioning.
  - **Simons Agent:** Quant signals and mean reversion patterns.
- **Signal Processing:** - **Kalman Filter:** For noise reduction in price action data.
  - **Bayesian Dynamic Weighting:** 5 independent models (including Facebook Prophet) that "earn" their influence based on recent historical accuracy.

## Tech Stack
- **Frontend:** React/TypeScript with custom SSR for 6,000+ stock pages.
- **Backend:** Express with Server-Sent Events (SSE) for real-time deliberation streaming.
- **Workers:** Python child processes for heavy seasonality decomposition (Prophet).
