# CactusCon2026

# Agentic Supply Chain Attack: The Nx "s1ngularity" Compromise

This repository contains research and forensic artifacts from the August 2025 Nx supply chain attack. 

## Incident Overview
* **Target:** Nx Build System (npm)
* **Payload:** `telemetry.txt` (Malware)
* **Exfil:** `base64.json`

## Artifacts Included
- **telemetry.txt**: The core logic that searches for AI binaries and executes the weaponized prompt.
- **base64.json**: The triple-encoded data structure used for exfiltrating `.npmrc` secrets and environment variables.

---
*Disclaimer: This research is published in a personal capacity for educational purposes.*
