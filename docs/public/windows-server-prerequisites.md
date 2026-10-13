# Required Configuration 

1. Navigate to: security.microsoft.com -> Settings -> Endpoints -> Enforcement scope and toggle ON these settings for at least Windows Servers. Consider Domain Controllers. 

<img width="2061" height="1266" alt="image" src="https://github.com/user-attachments/assets/37e9ab7f-253e-419c-8f6c-b6b8e0cac383" />

2. Navigate to intune.microsoft.com -> Endpoint security > Microsoft Defender for Endpoint, and set Allow Microsoft Defender for Endpoint to enforce Endpoint Security Configurations to On.

<img width="1420" height="862" alt="image" src="https://github.com/user-attachments/assets/88068da1-754f-43d5-85ae-368c5e63b66b" />

> [!IMPORTANT]
> **⚠️IMPORTANT: Always double check official documentation here:** 

> **Source:** Microsoft Learn  
> Full documentation is available here:  
> [Microsoft Defender Security Settings Management Documentation](https://learn.microsoft.com/en-us/intune/device-security/microsoft-defender/security-settings-management)

## Create dynamic security groups in Entra for assignments

1. Create dynamic security group to catch your Windows Server devices

<img width="1731" height="715" alt="image" src="https://github.com/user-attachments/assets/149c3592-76dc-4f7e-9577-79d9fc9fda2f" />

To split it up in different OS groups, you need to add one more syntax with value for each policy you create. For example one for 2016, 2019 and so on. (Look at table below or in Entra ID -> Device -> Version) 

<img width="1713" height="740" alt="image" src="https://github.com/user-attachments/assets/ce9f2ff7-b263-4ce3-b03d-b8d1d92c6d93" />

## Windows Server Latest DeviceOSVersion Reference

| Windows Server | Release | DeviceOSVersion |
|---|---|---|
| Windows Server 2016 | 1607 | `10.0.14393` |
| Windows Server 2019 | 1809 | `10.0.17763` |
| Windows Server 2022 | 21H2 | `10.0.20348` |
| Windows Server 2025 | 24H2 | `10.0.26100` |

> [!IMPORTANT]
> **⚠️ IMPORTANT: Always double check Version coloumn value in Entra ID for your servers.**
