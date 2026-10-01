# 🛡️ ALSO Microsoft Security Windows Server Policy Templates

> A collection of Microsoft Security Windows Server policies to help organizations accelerate secure deployments to servers with Defender for Servers (Defender for Cloud), Defender Business for Servers and Endpoint for Servers with Intune. 

**Works with Microsoft 365 Business Premium + Defender Business for Servers and up.**

> [!IMPORTANT]
> **⚠️ IMPORTANT: This solution only allows you to manage Endpoint Security policies in Intune for Firewall, Antivirus, and Attack Surface Reduction. It does not fully replace all configurations that may have been deployed through Configuration Manager (ConfigMgr) or Group Policy. Always review existing configurations before assigning any of these policies to avoid duplicate settings, conflicts, or misconfigurations caused by overlapping policies.**
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

> [!IMPORTANT]
> **⚠️ IMPORTANT: Read this before importing and using any policies.**

| Resource | Description |
|-----------|-------------|
| 🛡️ **Security Information** | [View Security Policy](https://github.com/CoC-MS/ALSO-Microsoft-Security-WindowsServer?tab=security-ov-file) |
| 📖 **Supported and Unsupported OS and Scenarios** | [View description](https://github.com/CoC-MS/ALSO-Microsoft-Security-WindowsServer?tab=readme-ov-file#supported-and-unsupported-operating-systems-and-scenarios) |
| 📖 **Supported licenses** | [View description](https://github.com/CoC-MS/ALSO-Microsoft-Security-WindowsServer?tab=readme-ov-file#works-with-following-licenses) |
| 📖 **Before importing ALSO_WINDOWSSERVER_POLICIES** | [View description](https://github.com/CoC-MS/ALSO-Microsoft-Security-WindowsServer?tab=readme-ov-file#before-importing-also_windowsserver_policies) |

## 📂 File Structure

All files are organized into categories

```text
/ALSO-Microsoft-Security-WindowsServer
├── ALSO_WINDOWSSERVER_POLICIES/SettingsCatalog
3 SettingsCatalog policies


```

### Works with following licenses

| Tag | Minimum Required License |
|:---:|--------------------------|
| **MDBS** | Microsoft 365 Business Premium + Defender for Business for Servers -on-premises servers only (can't have mixed licensing with 2 others below |
| **MDES** | Microsoft 365 E3 or Microsoft 365 E5 + Defender for Endpoint for Servers - on-premises servers only (can't have mixed licensing with 2 others above and below |
| **DFS** | Defender for Servers P1 and P2 in Defender for Cloud - works with servers in Azure or Arc onboarded servers (can't have mixed licensing with 2 others above |

---

## 📖 Naming Convention

All policy templates follow the naming format below:

```text
<ALSO>-<ImpactLevel>-<MinimumLicense>-<BaselineLevel>-<Version>-<OS>-<Main Category>-<Sub Category>-<Settings>-<Assignment>
```

### Example

```text
ALSO – LI – MDBS – Basic – v1.0– WindowsServer – Endpoint Security - Antivirus - AV Configuration - D
```

---

## 🧩 Naming Components

| Component | Description |
|-----------|-------------|
| **ALSO** | Company providing the policy template to have a better control |
| **Impact** | Impact level of policy, low (LI), medium (MI) or high (HI) |
| **MinimumLicense** | Minimum Microsoft license required to use the policy |
| **BaselineLevel** | Baseline level of policy, Basic, Advanced |
| **Version** | Policy version, v1.0, v1.1 etc|
| **MacOS** | Operating system |
| **MainCategory** | Name of main category, Device Configuration, Device Compliance etc|
| **SubCategory** | Name of sub category, MDE, AV, Disk etc|
| **Settings** | Short settings description |
| **Assignment** | Assignment scope- device (D) or user (U)|


## Before importing ALSO_WINDOWSSERVER_POLICIES

## Prerequisites

Before importing **ALSO_WINDOWSSERVER_POLICIES**, ensure the following prerequisites are met:

| Requirement | Details |
|------------|---------|
| Licensing | Microsoft Defender for Business (MDB), Microsoft Defender for Endpoint Server (MDES), or Defender for Servers (DfS) licensing is required. |
| Operating System | Verify that your servers meet the minimum supported operating system requirements listed above. |
| Intune | Microsoft Intune must be deployed and actively used for device management. |
| Defender Services | Microsoft Defender for Endpoint and/or Microsoft Defender for Cloud must be enabled and configured in your tenant or subscriptions and all servers needs to be onboarded to Defender with status Onboarded and Active. |
| Permissions | You must have the **Security Administrator** and **Intune Administrator**  roles assigned. |

## Required Configuration 

1. Navigate to: security.microsoft.com -> Settings -> Endpoints -> Enforcement scope and toggle ON these settings 

<img width="2061" height="1266" alt="image" src="https://github.com/user-attachments/assets/37e9ab7f-253e-419c-8f6c-b6b8e0cac383" />

2. Navigate to intune.microsoft.com -> Endpoint security > Microsoft Defender for Endpoint, and set Allow Microsoft Defender for Endpoint to enforce Endpoint Security Configurations to On.

<img width="1420" height="862" alt="image" src="https://github.com/user-attachments/assets/88068da1-754f-43d5-85ae-368c5e63b66b" />

> [!IMPORTANT]
> **⚠️IMPORTANT: Always double check official documentation here:** 

> **Source:** Microsoft Learn  
> Full documentation is available here:  
> [Microsoft Defender Security Settings Management Documentation](https://learn.microsoft.com/en-us/intune/device-security/microsoft-defender/security-settings-management)

