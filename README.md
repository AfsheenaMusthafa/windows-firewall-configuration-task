# windows-firewall-configuration-task
Practical task demonstrating Windows Firewall configuration — listing rules, blocking inbound traffic on Port 23 (Telnet), testing, and restoring default settings with documentation and screenshots.
# 🔒 Windows Firewall Configuration Task

## 📌 Steps Performed

1. **Open Firewall Configuration Tool**  
   - Opened **Windows Defender Firewall** via Control Panel → *System and Security* → *Windows Defender Firewall*.  
   - Alternatively, searched "Windows Defender Firewall" in the Start menu.

2. **List Current Firewall Rules**  
   - Navigated to **Advanced Settings** → *Inbound Rules* and *Outbound Rules*.  
   - Reviewed existing rules to check what traffic was allowed or blocked.

3. **Add a Rule to Block Inbound Traffic on Port 23 (Telnet)**  
   - In *Inbound Rules*, clicked **New Rule** → **Port** → Selected **TCP** → Specified **Port 23** → Chose **Block the connection** → Applied to all profiles → Named the rule "Block Telnet".

4. **Test the Rule**  
   - Attempted to connect to Port 23 locally; connection was blocked as expected.

5. **Remove the Test Rule**  
   - Located "Block Telnet" rule in **Inbound Rules**.  
   - Right-clicked → **Delete** to restore original firewall state.

6. **Documented Commands/Steps**  
   - GUI-based configuration steps recorded above.

---

## 🛡️ How Windows Firewall Filters Traffic

Windows Firewall works by applying a set of **rules** that decide whether to allow or block network traffic.

- **Inbound rules** control data coming *into* the system from the network.  
- **Outbound rules** control data leaving the system.  
- Each rule can be based on parameters such as **IP address**, **port number**, or **protocol** (TCP/UDP).  
- When a packet matches a rule, the firewall either **allows** or **blocks** it depending on the rule’s configuration.  
- If no specific rule matches, the default action for that profile (Domain, Private, Public) is applied.

---




