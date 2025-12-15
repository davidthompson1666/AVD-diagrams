Three files
1) wvdatscale
https://learn.microsoft.com/en-us/azure/architecture/example-scenario/azure-virtual-desktop/azure-virtual-desktop#architecture

Changes:
* Moved desktop subnet out of hub subnet into its own subnet


2) azure-virtual-desktop-multi-region-resilient-deployment
https://learn.microsoft.com/en-us/azure/cloud-adoption-framework/scenarios/azure-virtual-desktop/eslz-network-topology-and-connectivity#architectural-components-for-hub-and-spoke-with-hybrid-connectivity
Changes:
* Removed WVD with AVD
* Clarified FXLogix not used with personal pools

3) apply-zero-trust-to-Azure-Virtual-Desktop-diagrams 
https://learn.microsoft.com/en-us/security/zero-trust/azure-infrastructure-avd#reference-architecture
Changes:
* Removed spoke->firewall link, replaced with spoke->gateway link
