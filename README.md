# 🛡️ ALSO Microsoft Security Windows Server Policy Templates

> A collection of Microsoft Security Windows Server policies to help organizations accelerate secure deployments to servers with Defender for Servers (Defender for Cloud), Defender Business for Servers and Endpoint for Servers with Intune. 

**Works with Defender Business for Servers and up.**

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

## 📂 File Structure

All files are organized into categories

```text
/
├── ALSO_WINDOWS_SERVER
├── 


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
ALSO – LI – MDBS – Basic – v1.0– WindowsServer – AV- D
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

1. Ensure that you have MDBS, MDES or DFS licenses
2. Ensure that you meet minimum requirements for OS
3. Ensure you are using Intune today
4. Ensure that Defender for Endpoint instance and/or Defender for Cloud are active on your subscriptions

Required role to have are Security Administrator 

3. Navigate to security.microsoft.com -> Settings -> Endpoints -> Enforcement scope
4. Toggle these settings ON and Save

<img width="2061" height="1266" alt="image" src="https://github.com/user-attachments/assets/11937eab-bc8a-4643-a84c-6a93e017ce2d" />
