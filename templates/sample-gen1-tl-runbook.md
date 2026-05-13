# Gen1 to Gen2 Trusted Launch Migration Runbook

## 1. Goal
Upgrade Azure Generation 1 virtual machines to Generation 2 by enabling Trusted Launch using the Microsoft Upgrade-Gen1ToTL.ps1 script.

✅ Secure Boot: DISABLED  
✅ Migration Method: Trusted Launch (supported path)  

---

## 2. Scope
- Applies to Azure Gen1 VMs only
- Uses Microsoft Gen1-TrustedLaunch PowerShell workflow
- Covers pre-check, execution, validation, and rollback

---

## 3. Input (CSV)

Location: `templates/sample-gen1-tl.csv`

```csv
vmName,vmResourceGroupName,enableSecureBoot
myvm01,my-rg,FALSE
myvm02,my-rg,FALSE
