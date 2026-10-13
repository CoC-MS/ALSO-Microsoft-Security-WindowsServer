# 🛡️ ALSO Microsoft Security Windows Server Policy Templates

> A collection of Microsoft Security Windows Server policies to help organizations accelerate secure deployments to servers with Microsoft Defender for Servers (Defender for Cloud), Microsoft Defender for Endpoint or Business Server with Intune. 

**Works with Microsoft 365 Business Premium + Defender Business for Servers and up.**

> [!IMPORTANT]
> **⚠️ IMPORTANT: This solution only allows you to manage Endpoint Security policies in Intune for Firewall, Antivirus, and Attack Surface Reduction. It does not fully replace all configurations that may have been deployed through Configuration Manager (ConfigMgr) or Group Policy. Always review existing configurations before assigning any of these policies to avoid duplicate settings, conflicts, or misconfigurations caused by overlapping policies.**
---

> [!IMPORTANT]
> **⚠️ IMPORTANT: Read this before importing and using any policies.**

### Works with following licenses

| Tag | Minimum Required License |
|:---:|--------------------------|
| **MDBS** | Microsoft 365 Business Premium + Microsoft Defender for Business Server -on-premises servers only (can't have mixed licensing with 2 others below |
| **MDES** | Microsoft 365 E3 or Microsoft 365 E5 + Microsoft Defender for Endpoint Server - on-premises servers only (can't have mixed licensing with 2 others above and below |
| **DFS** | Microsoft Defender for Servers P1 and P2 in Defender for Cloud - works with servers in Azure or Arc onboarded servers (can't have mixed licensing with 2 others above |

---

| Resource | Description |
|-----------|-------------|
| 🛡️ **Security Information** | [View Security Policy](SECURITY.MD) |
| 📖 **Supported and Unsupported OS and Scenarios** | [View description](#supported-and-unsupported-operating-systems-and-scenarios) |
| 📖 **Supported licenses** | [View description](#works-with-following-licenses) |
| 📖 **Before importing ALSO_WINDOWSSERVER_POLICIES** | [View description](docs/public/README.md#before-importing-also_windowsserver_policies) |

----

## 📂 File Structure

All files are organized into categories

- [`ALSO_WINDOWSSERVER_POLICIES`](ALSO_WINDOWSSERVER_POLICIES)
  - [`ALSO – LI – MDBS – Basic – v1.0 - Windows Server - Endpoint Security - ASR -  Configuration - Audit Mode- D.json`](ALSO_WINDOWSSERVER_POLICIES/ALSO%20%E2%80%93%20LI%20%E2%80%93%20MDBS%20%E2%80%93%20Basic%20%E2%80%93%20v1.0%20-%20Windows%20Server%20-%20Endpoint%20Security%20-%20ASR%20-%20%20Configuration%20-%20Audit%20Mode-%20D.json)
  - [`ALSO – MI – MDBS – Basic – v1.0 - Windows Server - Endpoint Security - Antivirus - AV Configuration - D.json`](ALSO_WINDOWSSERVER_POLICIES/ALSO%20%E2%80%93%20MI%20%E2%80%93%20MDBS%20%E2%80%93%20Basic%20%E2%80%93%20v1.0%20-%20Windows%20Server%20-%20Endpoint%20Security%20-%20Antivirus%20-%20AV%20Configuration%20-%20D.json)
  - [`ALSO – MI – MDBS – Basic – v1.0 - Windows Server - Endpoint Security - Firewall - Firewall Configuration - D.json`](ALSO_WINDOWSSERVER_POLICIES/ALSO%20%E2%80%93%20MI%20%E2%80%93%20MDBS%20%E2%80%93%20Basic%20%E2%80%93%20v1.0%20-%20Windows%20Server%20-%20Endpoint%20Security%20-%20Firewall%20-%20Firewall%20Configuration%20-%20D.json)

3 SettingsCatalog policies

---

## Supported and Unsupported Operating Systems and Scenarios

### ✅ Supported Operating Systems

| Operating System | Requirements |
|------------------|-------------|
| Windows Server 2012 R2 | Microsoft Defender for Down-Level Devices |
| Windows Server 2016 | Microsoft Defender for Down-Level Devices |
| Windows Server 2019 | KB5025229 installed |
| Windows Server 2019 Core | Server Core App Compatibility Feature on Demand installed |
| Windows Server 2022 | KB5025230 installed |
| Windows Server 2022 Core | KB5025230 installed |
| Windows Server 2025 | Supported |
| Domain Controllers | Supported. Review Microsoft documentation for important considerations before deployment. |

### ❌ Unsupported Operating Systems and Scenarios

| Operating System / Scenario | Status |
|----------------------------|--------|
| Windows Server Core 2016 and earlier | Not supported |
| Non-persistent desktops (VDI) | Not supported |
| Azure Virtual Desktop (AVD/WVD) | Not supported |
| 32-bit versions of Windows | Not supported |

> **Source:** Microsoft Learn  
> Full documentation is available here:  
> [Microsoft Defender Security Settings Management Documentation](https://learn.microsoft.com/en-us/intune/device-security/microsoft-defender/security-settings-management)
