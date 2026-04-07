# The purpose of this lab was to show how to ingest threat intelligence indicators from external data source into Microsoft Sentinel, simulate a test event using one of these indicators, and then build a KQL query to find this event.
## Check the other files to see the details of each step.
## MITRE ATTACK tactic: TA0011: Command and control - technique: T1071: Application layer protocol.
## Steps:
- enabled a TAXII server data connector in MS Sentinel to receive threat intelligence indicators from Pulsedive
- created a virtual machine running Windows Server 2025 in my own test Azure subscription
- onboarded the VM to MS Defender for Endpoint to receive event telemetry from the VM
- randomly picked an IPv4 address from the threat intelligence data and connected to it from the VM
- built a KQL query in Sentinel to correlate: the IPv4 addresses from the threat intelligence data, and the network events of the VM
- finally, I checked if the query found a match that indicates suspicious activity.
