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

## 🚀 Deployment & Live Access

- **Live URL (HTTPS)**: [https://researchstudio.65-75-201-219.sslip.io](https://researchstudio.65-75-201-219.sslip.io)
- **Direct IP (HTTP fallback)**: [http://65.75.201.219:8085](http://65.75.201.219:8085)
- **GitHub Repository**: [https://github.com/harhmd/researchstudio](https://github.com/harhmd/researchstudio)

---

## 🛠️ Local Development & Docker

### Run with Docker Compose
```bash
docker compose up -d --build
```
Access at `http://localhost:8085`.

### Run Standalone
Simply open `index.html` in any modern web browser or serve via:
```bash
python -m http.server 8080
```

---

## 🔑 Gemini API Configuration
Click on the **Gemini API Key** button in the sidebar or **Settings** in the top navigation to set your Gemini API key. The key is stored locally in your browser (`localStorage`) and never transmitted to external third-party servers.
