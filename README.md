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
| **MDES** | Microsoft 365 E3 or Microsoft 365 E5 or E7 + Microsoft Defender for Endpoint Server - on-premises servers only (can't have mixed licensing with 2 others above and below |
| **DFS** |  Any of those above + Microsoft Defender for Servers P1 and P2 in Defender for Cloud - works with servers in Azure or Arc onboarded servers (can't have mixed licensing with 2 others above |

| Resource | Description |
| --- | --- |
| 📚 **[Documentation index](docs/public/README.md)** | Browse all deployment documentation. |
| 📖 **[Policy and configuration descriptions](docs/public/policy-collections.md)** | Review the preserved descriptions of every workload collection. |
| 🪟 **[Windows Server prerequisites](docs/public/windows-server-prerequisites.md)** | Device types and OS versions supported |
| 🚀 **[General prerequisites](docs/public/general-prerequisites.md)** | Review roles, licensing, prepare Intune and Defender. |
| 🧩 **[Dependencies prerequisites](docs/public/dependencies-and-errors.md)** | Review required configuration, assignments, and Windows Server DeviceOSVersion values. |
| 📖 **[Policy naming](docs/public/policy-naming.md)** | Understand licence tags and naming components. |
| 📂 **[File structure](docs/public/file-structure.md)** | Find the package and policy files. |
| 📥 **[How to import](docs/public/how-to-import.md)** | Follow the original illustrated import guidance. |
| 🐛 **[Reporting issues](docs/public/reporting-issues.md)** | Open an issue. |
| 🛡️ **[Security information](SECURITY.MD)** | Read the security and usage information. |
| 📜 **[License](LICENSE)** | Read the repository licence. |

----
