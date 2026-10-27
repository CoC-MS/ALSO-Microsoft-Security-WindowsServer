# 📂 File structure

[Public documentation](README.md)

This repository contains one Windows Server policy package. Its policy JSON files are inside the package's `SettingsCatalog` folder.

## 📦 Available package

| Package | Policy JSON files | Scope |
| --- | ---: | --- |
| [`ALSO_WINDOWSSERVER_POLICIES`](../../ALSO_WINDOWSSERVER_POLICIES) | 3 | Windows Server Endpoint Security policies for Antivirus, Firewall, and Attack Surface Reduction (ASR) in Block and Audit Mode. |

The count covers the JSON files currently in the package's `SettingsCatalog` folder. All three policy names carry the `MDBS` marker; these are naming components, not separate package choices. See [Policy naming](policy-naming.md) and the [Windows Server licensing guide](../../README.md#windows-server-licensing-guide) for context.

> [!WARNING]
> These templates cover Endpoint Security settings, not every Windows Server configuration managed through Configuration Manager (ConfigMgr) or Group Policy. Review existing configurations before assigning policies to avoid duplicate settings, conflicts, or misconfigurations caused by overlapping policies.

## 🗂️ Package contents

Browse all files under [`ALSO_WINDOWSSERVER_POLICIES/SettingsCatalog`](../../ALSO_WINDOWSSERVER_POLICIES/SettingsCatalog), or open an individual policy:

| Policy JSON | Contents |
| --- | --- |
| [MDBS Basic Antivirus](../../ALSO_WINDOWSSERVER_POLICIES/SettingsCatalog/ALSO%20%E2%80%93%20MI%20%E2%80%93%20MDBS%20%E2%80%93%20Basic%20%E2%80%93%20v1.0%20-%20Windows%20Server%20-%20Endpoint%20Security%20-%20Antivirus%20-%20AV%20Configuration%20-%20D.json) | Microsoft Defender Antivirus configuration. |
| [MDBS Basic Firewall](../../ALSO_WINDOWSSERVER_POLICIES/SettingsCatalog/ALSO%20%E2%80%93%20MI%20%E2%80%93%20MDBS%20%E2%80%93%20Basic%20%E2%80%93%20v1.0%20-%20Windows%20Server%20-%20Endpoint%20Security%20-%20Firewall%20-%20Firewall%20Configuration%20-%20D.json) | Windows Firewall configuration. |
| [MDBS Advanced ASR Block and Audit Mode](../../ALSO_WINDOWSSERVER_POLICIES/SettingsCatalog/ALSO%20%E2%80%93%20HI%20%E2%80%93%20MDBS%20%E2%80%93%20Adv%20%E2%80%93%20v1.0%20-%20Windows%20Server%20-%20Endpoint%20Security%20-%20ASR%20-%20%20Configuration%20-%20Block%20and%20Audit%20Mode-%20D.json) | Preconfigured ASR rules in Block and Audit Mode, with monitoring in the Defender portal. |

See [General prerequisites](general-prerequisites.md), [Windows Server prerequisites](windows-server-prerequisites.md), [Dependencies prerequisites](dependencies-and-errors.md), and [How to import](how-to-import.md) before deployment.
