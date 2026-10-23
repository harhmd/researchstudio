# PhD Thesis Research Studio (researchstudio)

🎓 **PhD Thesis Research Studio: Multi-Agent Academic Audit System**  
Dedicated for **Ts. Hj Nor Azhar Bin Abdul Hamid (MBA) (B.C.M)**

**Thesis Title:**  
*"AI Chatbot Adoption Readiness in Malaysian Agriculture: Mediating Roles of Acceptance, Trust, and Satisfaction"*

---

## 🌟 Overview

The **PhD Research Studio** is a multi-agent academic auditing and peer-review platform powered by Google Gemini AI. It evaluates thesis chapters across rigor, methodology, theoretical framework, data analysis, synthesis, coherence, and APA 7th Edition compliance.

### 🤖 Autonomous Audit Agents
1. **Chapter 1: Foundation Agent** – Audits Introduction, Background, Problem Statement (low digital literacy, trust deficits, aging demographic), Research Questions, and National Agro-Food Policy 2.0 (DAN 2.0) context.
2. **Chapter 2: Theorist Agent** – Evaluates TRAM, TAM, TRI models, literature matrix, Trust & Satisfaction mediators, and Age moderator.
3. **Chapter 3: Methodologist Agent** – Audits quantitative survey methodology, Melaka smallholder farmer sampling, PLS-SEM framework, and G*Power justification ($n=256$).
4. **Chapter 4: Analyst Agent** – Assesses measurement models (Cronbach's Alpha, Composite Reliability, AVE, HTMT, Fornell-Larcker) and structural path coefficients.
5. **Chapter 5: Synthesizer Agent** – Critiques discussion, theoretical/practical implications, multilingual design, human-in-the-loop backup, and limitations.
6. **Coherence Master Agent** – Verifies the "Golden Thread" consistency across research questions, variables, and methodologies.
7. **Master Tribunal** – Simulates a defense peer-review consensus across all chapters, evaluating defense readiness and generating an APA 7-compliant final report.

---

## 🔄 Gemini API Key Rotation & Multi-Tier Pool

The platform features an enterprise-grade **Gemini API Key Rotation Engine**:
- **Multi-Account & Multi-Tier Support**: Register multiple API keys labeled by Google Account and AI Studio Tier:
  - **Free Tier** (15 RPM / 1M TPM)
  - **Tier 1 (Pay-As-You-Go)** (1,000 RPM / 4M TPM)
  - **Tier 2 (Scale)** (2,000 RPM / 8M TPM)
  - **Tier 3 (High-Throughput)** (4,000 RPM / 16M TPM)
  - **Enterprise Tier**
- **Smart Rotation Strategies**:
  1. **Round-Robin**: Evenly balances requests across all active keys in the pool.
  2. **Account-Distributed**: Dispatches consecutive calls across different Google accounts to maximize total aggregate rate limits.
  3. **Free Tier First**: Prioritizes Free Tier keys to save costs, automatically bursting/failing over to Paid Tiers if an HTTP 429 quota exhaustion is detected.
  4. **Paid Tier Priority**: Uses high-speed paid keys first for lowest latency and highest throughput.
- **Auto-Failover & Cooldown**: When any key encounters an HTTP 429 (Resource Exhausted) or 503 error, it is placed in an automatic 60-second cooldown while the rotator immediately reroutes the current request to the next available key without interrupting the thesis critique.
- **Comprehensive Model Coverage**:
  - `gemini-3.8-flash` (Latest Flagship - Fast & Agentic)
  - `gemini-3.5-flash-lite` (Ultra-Low Latency & High Throughput)
  - `gemini-3.1-pro-preview` (Deep Academic Reasoning & Rigor)
  - `gemini-3.1-flash-lite` (Lightweight High-Frequency)
  - `gemini-3-flash-preview` (Canvas Native Default)
  - `gemini-flash-latest` (Always Points to Latest Flash)
  - `gemini-1.5-pro` & `gemini-1.5-flash`
  - **Custom Model Name** input field for newly announced models.
- **Bulk Import / Export**: Quickly paste multiple keys (`API_KEY, Account, Tier`) or export/import JSON backups.
- **Client-Side Privacy**: All API keys reside strictly inside your browser's private `localStorage` and are never logged or stored on any intermediate server.

---

## 🚀 Live Access & Deployment

- **Live URL (HTTPS)**: [https://researchstudio.65-75-201-219.sslip.io](https://researchstudio.65-75-201-219.sslip.io)
- **Direct IP (HTTP fallback)**: [http://65.75.201.219:8085](http://65.75.201.219:8085)
- **GitHub Repository**: [https://github.com/harhmd/researchstudio](https://github.com/harhmd/researchstudio)
- **Coolify Instance**: Managed on VPS `65.75.201.219` under project **PhD Research Studio**.

---

## 🛠️ Local Development & Docker

```bash
# Run with Docker Compose
docker compose up -d --build
```
Access at `http://localhost:8085`.
