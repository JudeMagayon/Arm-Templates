# 🚀 Microsoft Sentinel - Free Log Sources Deployment

This repository contains an ARM template and UI definition that deploy **13 Microsoft Sentinel solutions** using the **Content Hub**, all mapped to **free log sources**.

### ✅ Included Free Log Sources

- Azure Activity Logs  
- Sentinel Health  
- Entra ID Sign-In Logs  
- Entra ID Audit Logs  
- Entra ID Risk Alerts (Identity Protection)  
- Office 365 Logs (Exchange, SharePoint, Teams)  
- Microsoft Defender for Endpoint (MDATP)  
- Microsoft Defender for Identity (AATP)  
- Microsoft Defender for Cloud Apps (MCAS)  
- Microsoft Defender for Cloud  
- Microsoft Defender for IoT  
- Microsoft Defender XDR – Alerts  
- Microsoft Defender XDR – Incidents  

---

## 📦 How to Deploy

Click the button below to deploy directly via the Azure Portal:

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FJudeMagayon%2FArm-Templates%2Fmain%2Fazuredeploy.json)

> 📌 You will be prompted to:
> - Select a Resource Group (must contain your existing Log Analytics workspace)
> - Enter your Log Analytics Workspace name
> - Confirm deployment of all 13 free Content Hub solutions

---

## 📁 Files Included

| File Name               | Description                                     |
|------------------------|-------------------------------------------------|
| `azuredeploy.json`     | ARM template for deploying all Content Hub solutions |
| `createUiDefinition.json` | Portal UI definition for custom deployment flow  |

---

## 📘 Notes

- These log sources incur **no ingestion cost** in Microsoft Sentinel.
- Retention beyond 30 days is optional and may incur storage costs.
- Deployment time: ~5 minutes.
- All Content Hub solutions use API version `2025-03-01`.

---

## 🔗 References

- [Microsoft Sentinel Free Data Sources](https://learn.microsoft.com/azure/sentinel/billing#free-data-sources)
- [Content Hub Deployment API](https://learn.microsoft.com/azure/sentinel/sentinel-solutions-deploy-api)

---

> 🛡️ Built for DepEd | Region: Southeast Asia | Estimated Volume: 80–150 GB/day
