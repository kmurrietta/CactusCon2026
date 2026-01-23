# CactusCon2026

# Agentic Supply Chain Attack: The Nx "s1ngularity" Compromise

This repository contains research and forensic artifacts from the August 2025 Nx supply chain attack. This incident is significant as it represents one of the first documented cases of malware "prompt engineering" local AI CLIs to perform automated reconnaissance.

## Incident Overview
* **Target:** Nx Build System (npm)
* **Vector:** Compromised publishing token (bypassing 2FA)
* **Payload:** `telemetry.js` (Agentic Malware)
* **Novelty:** Hijacking of `claude`, `gemini`, and `amazon-q` binaries for filesystem enumeration.

## Artifacts Included
- **telemetry.js**: The core logic that searches for AI binaries and executes the weaponized prompt.
- **base64.json**: The triple-encoded data structure used for exfiltrating `.npmrc` secrets and environment variables.

## Key Takeaways for Defenders
1. **Log Everything:** Detection was only possible through command-line logging on macOS.
2. **AI Guardrails Matter:** The attack was partially mitigated by the AI's refusal to follow malicious instructions.
3. **Identity is the Perimeter:** Move to OIDC-based trusted publishing for npm/GitHub.

---
*Disclaimer: This research is published in a personal capacity for educational purposes.*
