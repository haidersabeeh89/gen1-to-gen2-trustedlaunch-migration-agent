---
description: Generate a migration plan for Azure Gen1 VMs using the Microsoft Gen1-TrustedLaunch PowerShell workflow with Secure Boot disabled.
---

Generate a migration plan for the provided Azure Gen1 VMs using the Microsoft Gen1-TrustedLaunch script workflow.

Requirements:
- Use only the supported path: Gen1 to Gen2 by upgrading to Trusted Launch.
- Keep Secure Boot disabled.
- Generate or review CSV entries with `enableSecureBoot=FALSE`.
- Validate prerequisites and identify blockers:
  - unsupported VM size
  - unsupported OS
  - Azure Backup policy
  - ASR enabled
  - disk encryption enabled
  - VM agent health
  - EFI / disk partition risk
- Provide:
  1. Goal
  2. Assumptions
  3. Prerequisite validation
  4. Migration steps
  5. CSV sample
  6. PowerShell execution example
  7. Risks/blockers
  8. Post-upgrade validation
  9. Rollback notes
``
