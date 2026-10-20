# 🛡️ ALSO Microsoft Security Windows Server Policy Templates

> A collection of Microsoft Security Windows Server policies to help organizations accelerate secure deployments to servers with Microsoft Defender for Servers (Defender for Cloud), Microsoft Defender for Endpoint or Business Server with Intune. 


> [!IMPORTANT]
> **⚠️ IMPORTANT: This solution only allows you to manage Endpoint Security policies in Intune for Firewall, Antivirus, and Attack Surface Reduction. It does not fully replace all configurations that may have been deployed through Configuration Manager (ConfigMgr) or Group Policy. Always review existing configurations before assigning any of these policies to avoid duplicate settings, conflicts, or misconfigurations caused by overlapping policies.**
---

> [!IMPORTANT]
> **⚠️ IMPORTANT: Read this before importing and using any policies.**

<a id="getting-started"></a>
## 🚀 Getting started

1. Review the [general prerequisites](docs/public/general-prerequisites.md), [Windows Server requirements](docs/public/windows-server-prerequisites.md), [dependencies and error handling](docs/public/dependencies-and-errors.md), and [security information](https://github.com/CoC-MS/ALSO-Microsoft-Security-WindowsServer/tree/main?tab=security-ov-file).
2. Download package [`ALSO_WINDOWSSERVER_POLICIES`](ALSO_WINDOWSSERVER_POLICIES) and review licensing guide below.
3. Follow [How to import](docs/public/how-to-import.md) for extraction and import guidance.
4. Assign reviewed policies to a pilot group, check policy deployment reports and server impact, then expand in stages.


### Quick navigation

| Section | What you will find |
| --- | --- |
| [Getting started](#getting-started) | Prerequisites, package selection, and import. |
| [Windows Server Licensing Guide](#windows-server-licensing-guide) | License compatibility and limitations. |
| [Windows Server packages](#windows-server-packages) | Package contents and license mapping. |
| [Documentation](#documentation) | Links to supporting guides and the repository license. |

---

<a id="windows-server-licensing-guide"></a>
## Windows Server Licensing Guide

| Tag | Minimum Required License |
|:---:|--------------------------|
| **MDBS** | Microsoft 365 Business Premium + Microsoft Defender for Business Server -on-premises servers only (can't have mixed licensing with 2 others below |
| **MDES** | Microsoft 365 E3 or Microsoft 365 E5 or E7 + Microsoft Defender for Endpoint Server - on-premises servers only (can't have mixed licensing with 2 others above and below |
| **DFS** |  Any of those above + Microsoft Defender for Servers P1 and P2 in Defender for Cloud - works with servers in Azure or Arc onboarded servers (can't have mixed licensing with 2 others above |


Learn more: 

| Solution | Learn More |
|----------|------------|
| Microsoft Defender for Business Servers | [Learn More](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftDefenderforBusinessservers/MCA#ServiceSpecificTerms) |
| Microsoft Defender for Endpoint for Servers | [Learn More](https://www.microsoft.com/licensing/terms/productoffering/MicrosoftDefenderforEndpointforservers/MCA) |
| Microsoft Defender for Servers (P1 & P2) | [Learn More](https://www.microsoft.com/licensing/faqs/48) |

---

<a id="windows-server-packages"></a>
## 📦 Windows Server packages

| Package | JSON files | License mapping |
| --- | ---: | --- |
| [`ALSO_WINDOWSSERVER_POLICIES`](ALSO_WINDOWSSERVER_POLICIES) | 3 |

- [MDBS Antivirus policy](ALSO_WINDOWSSERVER_POLICIES/ALSO%20%E2%80%93%20MI%20%E2%80%93%20MDBS%20%E2%80%93%20Basic%20%E2%80%93%20v1.0%20-%20Windows%20Server%20-%20Endpoint%20Security%20-%20Antivirus%20-%20AV%20Configuration%20-%20D.json)
- [MDBS Firewall policy](ALSO_WINDOWSSERVER_POLICIES/ALSO%20%E2%80%93%20MI%20%E2%80%93%20MDBS%20%E2%80%93%20Basic%20%E2%80%93%20v1.0%20-%20Windows%20Server%20-%20Endpoint%20Security%20-%20Firewall%20-%20Firewall%20Configuration%20-%20D.json)
- [MDBS ASR Audit Mode policy](ALSO_WINDOWSSERVER_POLICIES/ALSO%20%E2%80%93%20LI%20%E2%80%93%20MDBS%20%E2%80%93%20Basic%20%E2%80%93%20v1.0%20-%20Windows%20Server%20-%20Endpoint%20Security%20-%20ASR%20-%20%20Configuration%20-%20Audit%20Mode-%20D.json)

---

<a id="documentation"></a>
## 📚 Documentation

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
| 🛡️ **[Security information](https://github.com/CoC-MS/ALSO-Microsoft-Security-WindowsServer/security)** | Read the security and usage information. |
| 📜 **[License](LICENSE)** | Read the repository licence. |

----
