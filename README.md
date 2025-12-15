
# Azure Virtual Desktop Architecture Diagram Corrections

This repository documents updates made to three Microsoft‑published Azure Virtual Desktop (AVD) architectural diagrams that contained inaccuracies. Each section includes the source diagram, a description, and the corrections applied.

---

## 1. **wvdatscale**

**Source:**  
https://learn.microsoft.com/en-us/azure/architecture/example-scenario/azure-virtual-desktop/azure-virtual-desktop#architecture

**Description:**  
A basic single‑region AVD architecture diagram illustrating network components and two host pools. The original diagram incorrectly placed one of the host pools within the hub subnet, and uses Windows Virtual Desktop rather than Azure Virtual Desktop

**Corrections Applied:**  
- Moved the desktop subnet out of the hub subnet into its own dedicated subnet. Updated Windows Virtual Desktop to Azure Virtual Desktop.

---

## 2. **azure-virtual-desktop-multi-region-resilient-deployment**

**Source:**  
https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/scenarios/azure-virtual-desktop/eslz-network-topology-and-connectivity#architectural-components-for-hub-and-spoke-with-hybrid-connectivity

**Description:**  
A multi‑region AVD resilient deployment diagram. The original version incorrectly referred to “WVD” rather than “AVD.”

**Corrections Applied:**  
- Replaced all references to **WVD** with **AVD**.  
-- Clarified that **FSLogix is not used with personal host pools**.

---

## 3. **apply-zero-trust-to-Azure-Virtual-Desktop-diagrams**

**Source:**  
https://learn.microsoft.com/en-us/security/zero-trust/azure-infrastructure-avd#reference-architecture

**Description:**  
A Zero Trust‑focused AVD architecture. The original diagram incorrectly showed network connectivity for only one host pool and routed it to the firewall instead of the AVD gateway.

**Corrections Applied:**  
- Updated and added network links to correctly route connectivity through the AVD gateway for all host pools.

