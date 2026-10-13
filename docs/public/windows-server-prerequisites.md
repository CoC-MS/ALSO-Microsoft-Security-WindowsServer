# Windows Server prerequisites

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
