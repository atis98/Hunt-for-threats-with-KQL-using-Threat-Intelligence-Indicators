# Steps:
- In this final step, the goal is to discover a correlation, an event match between the threat intelligence IP addresses, and those IP addresses that we actually connected to.
- One part of the data (the threat intelligence) is in the "ThreatIntelIndicators" table.
- The other part (the actual established connections) is in the "DeviceNetworkEvents" table.
- So I built the following KQL query to join these 2 tables on the IPv4 address value, and show those events where my test IP address appears in both tables: <img width="824" height="508" alt="Screenshot 2026-04-07 at 12 08 06" src="https://github.com/user-attachments/assets/2e509811-7a55-43c0-a3fe-c7355749c309" />
