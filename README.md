I had uploaded the screenshots regarding my work what I did,I  had configured my firewall to block telnet port 23 then I had tried to access it locally by my machine and it showed that it is unaccessible that
means it had been blocked.I had done it in windows by Windows Firewall GUI by the following steps:-

Note:Before doing the following steps written below Click Turn Windows features on or off (on the left side).In the list, find and check "Telnet Client".

1. Open Firewall Configuration Tool by opening Windows Defender Firewall.
2. Listing Current Firewall Rules.Click Advanced Settings (on left side panel).View Inbound Rules and Outbound Rules for current configuration.
3.In Inbound Rules, select New Rule (right panel).Choose Port then click Next.Select TCP, enter 23 in Specific local ports then click Next.
Choose Block the connection then click on Next.Apply to Domain/Private/Public by checking the checkbox then click on next.
Name the rule here like here I had given “Block Telnet Port 23” and click Finish.
4. Test the Rule
Attempt to connect via Telnet to localhost 23 or from another machine using Telnet. It should be blocked.By opening command prompt and typing the command"telnet localhost 23".
After that it will display the message "Connecting To localhost...Could not open connection to the host, on port 23: Connect failed" which means telnet localhost port 23 had been blocked.      
6. Remove the Block Rule
When the work is done Go to Inbound Rules, find “Block Telnet Port 23”.
Right-click then click Delete.

Summary: How Firewalls Filter Traffic
Firewalls filter traffic by allowing or denying network packets based on rules set for ports, protocols, IP ranges, and connection types.
Inbound rules protect against unsolicited incoming connections.
Outbound rules restrict data leaving the device.
Rules can be customized for specific needs (e.g., blocking Telnet, allowing SSH).
Testing rules ensures security policies are correctly enforced.
Administrators restore the original firewall configuration by removing test or temporary rules, maintaining system safety and accessibility.
In essence, firewalls act as gatekeepers, letting in only the traffic you specify while blocking unwanted or potentially harmful connections.
In this how to connect via Telnet to localhost:23 or from another machine using Telnet. It should be blocked.
In this how to connect via Telnet to localhost:23 or from another machine using Telnet. It should be blocked.


