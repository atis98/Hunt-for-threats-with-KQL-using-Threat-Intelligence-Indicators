# Steps:
- in my own demo Azure subscription, I created an Azure virtual machine with Windows Server 2025
- I connected to the VM via Azure Bastion, logged in to MS Defender and went to Settings-Endpoints-Onbording section to onboard the VM.
- I downloaded and ran the onboarding script. Now the VM was successfully onboarded to Defender for Endpoint.
- I made sure it is providing telemetry by running this KQL query. As you can see, events were arriving: <img width="882" height="595" alt="Screenshot 2026-04-07 at 11 51 23" src="https://github.com/user-attachments/assets/d810ae08-e729-46a4-9b78-88f6335f2172" />
