# Skills-china-travel-101-
An all-in-one AI Agent Skill for foreign tourists in China. 
Four Features: Payment Guides, Cultural Naming, AI Art (Seal/Landscape), Smart LBS Food Discovery with Allergy Safety. Fully compatible with OpenClaw and Tencent SkilHub and Alipay
# China Travel 101: The Ultimate AI Agent Skill for Global Explorers

`China Travel 101` is an all-in-one AI Agent Skill designed to bridge the gap for foreign tourists visiting China. From navigating the complex digital payment landscape to deep cultural immersion through AI-generated art, this skill provides everything a traveler needs to feel like a local.

Fully compatible with **OpenClaw**, **Tencent SkilHub**, and major AI agent frameworks.

---

## 🌟 4 Core Features

### 1. 💳 Seamless Mobile Payment Guides (WeChat & Alipay)
Navigating China's "cashless" society is the #1 challenge for tourists.
*   **Step-by-Step Tutorials**: English interface setup for WeChat and Alipay.
*   **Digital Onboarding**: Guide for real-time ID verification and linking international cards (Visa, Mastercard).
*   **Transaction Support**: Context-aware help for scanning QR codes and handling payment failures.

### 2. 🎨 Cultural Naming & AI Art Creation
Transform a foreign identity into a Chinese cultural masterpiece.
*   **Semantic Naming**: Intelligent conversion of original names into Chinese based on deep etymological meanings.
*   **Poetry Generation**: Automatic creation of classical Chinese poems (Jueju) embedding the user's name.
*   **Art Prompts**: High-fidelity prompt engineering for:
    *   **Traditional Seal Carvings**: Square soapstone seals with ancient script.
    *   **Landscape Painting**: Ink-wash Shanshui art inspired by the generated poetry.

### 3. 🍱 Smart LBS Food Discovery with Allergy Safety
Eat with confidence using real-time location-based services (LBS).
*   **Local Discovery**: Recommends authentic dining spots in Shanghai, Suzhou, and Hangzhou based on your current GPS coordinates.
*   **Allergy Guard (Lobster OpenClaw Feature)**: Spontaneously prompts users to register allergies and automatically flags risky ingredients in recommended dishes.

### 4. 🏥 Emergency Medical & Essential Resources
Safety first in a foreign environment.
*   **Instant Location**: Find the nearest 24h pharmacies and hospitals with Emergency Room (ER) facilities.
*   **Bilingual Crisis Support**: Provides translated medical phrases for immediate communication with healthcare providers.

---

## 🛠️ Developer Integration Guide

Global developers can integrate these skills into their AI agents using the following source files:

### 📄 1. The Core Logic: `SKILL.md`
The [SKILL.md](.trae/skills/china-travel-101/SKILL.md) contains the underlying prompt engineering, cultural logic, and safety protocols. Use this to understand the behavioral flow of the agent.

### � 2. Tencent SkilHub: `tencent_skilhub_manifest.json`
To deploy on [SkilHub.tencent.com](https://skilhub.tencent.com):
*   **Source**: [tencent_skilhub_manifest.json](.trae/skills/china-travel-101/tencent_skilhub_manifest.json)
*   **Capability**: Declares `geolocation_api` and `poi_search` permissions.
*   **Runtime**: Optimized for GPT-4o/Claude-3.5-Sonnet on the Tencent cloud environment.

### 🦞 3. OpenClaw Hub: `openclaw_config.yaml`
To deploy on [ClawHub.ai](https://clawhub.ai) or the [China Mirror](https://mirror-cn.clawhub.com):
*   **Source**: [openclaw_config.yaml](.trae/skills/china-travel-101/openclaw_config.yaml)
*   **Configuration**: Set `location_tracking: true` and `safety_mode: "Strict-Allergy-Filter"` to activate the advanced safety features.
*   **Triggers**: Pre-configured intent triggers for naming, art, and emergency LBS actions.

---

## 📦 Getting Started
1. **Clone the repository**:
   ```bash
   git clone https://github.com/XiaoAIPensieve/china-travel-101.git
   ```
2. **Import Skills**:
   * For **Trae/Claude Desktop**: Copy the `.trae/skills/china-travel-101` folder to your project root.
   * For **OpenClaw**: Upload `openclaw_config.yaml` to your agent dashboard.

---
*Empowering global travelers with the wisdom of China.*
