## What this repo does
This repository provides a GitHub Copilot custom agent for migrating Azure Gen1 VMs to Gen2 using the Trusted Launch workflow.

## Components
- Custom agent: handles migration reasoning and runbook generation
- Prompt templates: enforce repeatable workflows
- CSV templates: used for PowerShell script execution
- Copilot instructions: enforce Secure Boot = FALSE and safe practices

## Key behavior
- Uses only supported path: Gen1 → Trusted Launch (Gen2)
- Keeps Secure Boot disabled by default
- Always performs prerequisite validation before execution
