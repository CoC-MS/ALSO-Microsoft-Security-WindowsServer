# General prerequisites

**Disclaimer:** Licensing prerequisites and feature availability listed on this page may be incorrect, incomplete, or outdated. We strongly recommend verifying all licensing information against the latest official Microsoft licensing documentation before making any purchasing or deployment decisions.

**Enterprise licenses:** [Microsoft Enterprise Plan Comparison](https://cdn-dynmedia-1.microsoft.com/is/content/microsoftcorp/microsoft/bade/documents/products-and-services/en-us/education/Modern-Work-Plan-Comparison-Enterprise.pdf)

**SMB licenses:** [Microsoft SMB Plan Comparison](https://cdn-dynmedia-1.microsoft.com/is/content/microsoftcorp/microsoft/bade/documents/products-and-services/en-us/education/Modern-Work-Plan-Comparison-Enterprise.pdf)

## Before importing ALSO_WINDOWSSERVER_POLICIES

## Required Configuration 

1. Navigate to: security.microsoft.com -> Settings -> Endpoints -> Enforcement scope and toggle ON these settings for at least Windows Servers. Consider Domain Controllers, but be very careful with that. 

PS: You need to use Defender for Servers in Defender for Cloud to benefit from last setting. Check Azure portal that your Arc onboarded or Azure servers are visible there and that they are covered by Defender for Servers P1 or P2 licenses

<img width="2061" height="1266" alt="image" src="https://github.com/user-attachments/assets/37e9ab7f-253e-419c-8f6c-b6b8e0cac383" />


2. Navigate to intune.microsoft.com -> Endpoint security > Microsoft Defender for Endpoint, and set Allow Microsoft Defender for Endpoint to enforce Endpoint Security Configurations to On.

<img width="1420" height="862" alt="image" src="https://github.com/user-attachments/assets/88068da1-754f-43d5-85ae-368c5e63b66b" />

> [!IMPORTANT]
> **⚠️IMPORTANT: Always double check official documentation here:** 

> **Source:** Microsoft Learn  
> Full documentation is available here:  
> [Microsoft Defender Security Settings Management Documentation](https://learn.microsoft.com/en-us/intune/device-security/microsoft-defender/security-settings-management)
