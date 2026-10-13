# 🛡️ ALSO Microsoft Security Windows Server Policy Templates

> A collection of Microsoft Security Windows Server policies to help organizations accelerate secure deployments to servers with Microsoft Defender for Servers (Defender for Cloud), Microsoft Defender for Endpoint or Business Server with Intune. 


> [!IMPORTANT]
> **⚠️ IMPORTANT: This solution only allows you to manage Endpoint Security policies in Intune for Firewall, Antivirus, and Attack Surface Reduction. It does not fully replace all configurations that may have been deployed through Configuration Manager (ConfigMgr) or Group Policy. Always review existing configurations before assigning any of these policies to avoid duplicate settings, conflicts, or misconfigurations caused by overlapping policies.**
---

> [!IMPORTANT]
> **⚠️ IMPORTANT: Read this before importing and using any policies.**

### Windows Server Licensing Guide

| Tag | Minimum Required License |
|:---:|--------------------------|
| **MDBS** | Microsoft 365 Business Premium + Microsoft Defender for Business Server -on-premises servers only (can't have mixed licensing with 2 others below |
| **MDES** | Microsoft 365 E3, F3 or Microsoft 365 E5 + Microsoft Defender for Endpoint Server - on-premises servers only (can't have mixed licensing with 2 others above and below |
| **DFS** |  Any of those above + Microsoft Defender for Servers P1 and P2 in Defender for Cloud - works with servers in Azure or Arc onboarded servers (can't have mixed licensing with 2 others above |

| Resource | Description |
|-----------|-------------|
| 🛡️ **Security Information** | [View Security Policy](SECURITY.MD) |
| 📖 **Supported and Unsupported OS and Scenarios** | [View description](docs/public/supported-operating-systems-and-scenarios.md) |
| 📖 **Supported licenses** | [View description](#works-with-following-licenses) |
| 📖 **Before importing ALSO_WINDOWSSERVER_POLICIES** | [View description](docs/public/README.md) |

----

## Before importing ALSO_WINDOWSSERVER_POLICIES

- [Prerequisites](docs/public/general-prerequisites.md)
- [Required Configuration](docs/public/windows-server-prerequisites.md)
- [📖 Naming Convention](docs/public/policy-naming.md)
- [How to import policy templates ALSO_WINDOWSSERVER_POLICIES](docs/public/how-to-import.md)
- [Issues?](docs/public/reporting-issues.md)
