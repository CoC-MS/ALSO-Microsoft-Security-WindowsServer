# 🛡️ ALSO Microsoft Security Windows Server Policy Templates

> A collection of Microsoft Security Windows Server policies to help organizations accelerate secure deployments to servers with Microsoft Defender for Servers (Defender for Cloud), Microsoft Defender for Endpoint or Business Server with Intune. 

**Works with Microsoft 365 Business Premium + Defender Business for Servers and up.**

> [!IMPORTANT]
> **⚠️ IMPORTANT: This solution only allows you to manage Endpoint Security policies in Intune for Firewall, Antivirus, and Attack Surface Reduction. It does not fully replace all configurations that may have been deployed through Configuration Manager (ConfigMgr) or Group Policy. Always review existing configurations before assigning any of these policies to avoid duplicate settings, conflicts, or misconfigurations caused by overlapping policies.**
---

> [!IMPORTANT]
> **⚠️ IMPORTANT: Read this before importing and using any policies.**

| Resource | Description |
|-----------|-------------|
| 🛡️ **Security Information** | [View Security Policy](SECURITY.MD) |
| 📖 **Supported and Unsupported OS and Scenarios** | [View description](docs/public/supported-operating-systems-and-scenarios.md) |
| 📖 **Supported licenses** | [View description](#works-with-following-licenses) |
| 📖 **Before importing ALSO_WINDOWSSERVER_POLICIES** | [View description](docs/public/README.md) |

----

### Works with following licenses

| Tag | Minimum Required License |
|:---:|--------------------------|
| **MDBS** | Microsoft 365 Business Premium + Microsoft Defender for Business Server -on-premises servers only (can't have mixed licensing with 2 others below |
| **MDES** | Microsoft 365 E3 or Microsoft 365 E5 + Microsoft Defender for Endpoint Server - on-premises servers only (can't have mixed licensing with 2 others above and below |
| **DFS** | Microsoft Defender for Servers P1 and P2 in Defender for Cloud - works with servers in Azure or Arc onboarded servers (can't have mixed licensing with 2 others above |

---

## [📂 File Structure](docs/public/file-structure.md)

- [`ALSO_WINDOWSSERVER_POLICIES`](ALSO_WINDOWSSERVER_POLICIES)
  - [`ALSO – LI – MDBS – Basic – v1.0 - Windows Server - Endpoint Security - ASR -  Configuration - Audit Mode- D.json`](ALSO_WINDOWSSERVER_POLICIES/ALSO%20%E2%80%93%20LI%20%E2%80%93%20MDBS%20%E2%80%93%20Basic%20%E2%80%93%20v1.0%20-%20Windows%20Server%20-%20Endpoint%20Security%20-%20ASR%20-%20%20Configuration%20-%20Audit%20Mode-%20D.json)
  - [`ALSO – MI – MDBS – Basic – v1.0 - Windows Server - Endpoint Security - Antivirus - AV Configuration - D.json`](ALSO_WINDOWSSERVER_POLICIES/ALSO%20%E2%80%93%20MI%20%E2%80%93%20MDBS%20%E2%80%93%20Basic%20%E2%80%93%20v1.0%20-%20Windows%20Server%20-%20Endpoint%20Security%20-%20Antivirus%20-%20AV%20Configuration%20-%20D.json)
  - [`ALSO – MI – MDBS – Basic – v1.0 - Windows Server - Endpoint Security - Firewall - Firewall Configuration - D.json`](ALSO_WINDOWSSERVER_POLICIES/ALSO%20%E2%80%93%20MI%20%E2%80%93%20MDBS%20%E2%80%93%20Basic%20%E2%80%93%20v1.0%20-%20Windows%20Server%20-%20Endpoint%20Security%20-%20Firewall%20-%20Firewall%20Configuration%20-%20D.json)

---

## Before importing ALSO_WINDOWSSERVER_POLICIES

- [Prerequisites](docs/public/general-prerequisites.md)
- [Required Configuration](docs/public/windows-server-prerequisites.md)
- [📖 Naming Convention](docs/public/policy-naming.md)
- [How to import policy templates ALSO_WINDOWSSERVER_POLICIES](docs/public/how-to-import.md)
- [Issues?](docs/public/reporting-issues.md)
