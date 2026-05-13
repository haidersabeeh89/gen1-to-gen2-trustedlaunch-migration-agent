# Copilot repository instructions

This repository uses GitHub Copilot to assist with Azure VM migrations from Generation 1 to Generation 2 by upgrading to Trusted Launch.

## Mandatory guidance
- Use the Microsoft Azure Gen1-TrustedLaunch repository and Microsoft Learn documentation as the primary source of truth.
- Do not suggest a direct Gen1 to Gen2 path without Trusted Launch.
- Default all migration examples and CSV templates to Secure Boot disabled.
- When generating CSV samples for Upgrade-Gen1ToTL.ps1, set `enableSecureBoot` to `FALSE` unless explicitly instructed otherwise.
- Always validate prerequisites before proposing execution:
  - supported VM size
  - supported OS
  - VM agent health
  - encryption state
  - backup policy
  - ASR state
  - lower-environment validation
- Always include production-safe output:
  - prerequisites
  - execution steps
  - risks/blockers
  - post-upgrade checks
  - rollback notes

## Preferred style
- Be concise, operator-friendly, and implementation-focused.
- Prefer checklists and ready-to-run examples over long prose.
- If a requested detail is not explicitly documented in source material, say so clearly.
``
