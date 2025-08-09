 Windows Firewall Task — Block Telnet Port 23

 Objective
Demonstrate creating a firewall rule in Windows Defender Firewall with Advanced Security to block TCP port 23 (Telnet).

 Steps Performed

 1. Verified Admin Rights
Confirmed that the current account is a member of the Administrators group.

 2. Opened Firewall Settings
- Pressed Windows Key
- Searched for "Windows Defender Firewall with Advanced Security"
- Ran it as Administrator

 3. Created New Inbound Rule
- Selected Port
- Chose TCP
- Specified local port: 23
- Action: Block the connection
- Applied to all profiles (Domain, Private, Public)
- Named rule: Block Telnet Port 23

 4. Verified Rule
- Checked in **Inbound Rules** to ensure the rule was enabled.

 5. Exported Policy
- Clicked Action → Export Policy
- Saved as firewall-config.wfw

 Evidence
Screenshots included:
1. Creating new inbound rule (Port 23, TCP)
2. Policy export confirmation
3. Export dialog with filename firewall-config.wfw
4. Action menu showing Export Policy option

All evidence files are in this repository.

## How to Restore Defaults
- Open Windows Defender Firewall (basic control panel view)
- Click Restore defaults in the left menu
- Confirm

Or remove just the test rule:
- Go to Inbound Rules
- Find Block Telnet Port 23
- Right-click → Delete


