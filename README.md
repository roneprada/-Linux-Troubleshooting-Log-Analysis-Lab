### 🔧 Incident — Linux Network Connectivity Failure

**Issue:**  
System unable to reach external network resources.

**Detection:**  
Ping requests to external IP failed.

**Investigation:**  
- Used `ping` to test connectivity  
- Used `traceroute` to identify where traffic was failing  

**Root Cause:**  
Network connectivity issue preventing outbound traffic.

**Resolution:**  
Validated network path and restored connectivity.

**Validation:**  
Successful ping and traceroute confirmed connectivity restored.

### 🔧 Incident — Service Not Responding

**Issue:**  
Application/service not responding on expected port.

**Detection:**  
Service unreachable from client.

**Investigation:**  
- Used `netstat -tulnp` to check listening ports  
- Verified whether the service was active  

**Root Cause:**  
Service not running or not listening on the expected port.

**Resolution:**  
Restarted or reconfigured the service.

**Validation:**  
Service successfully responded on the expected port.

### 🔧 Incident — Log-Based Error Investigation

**Issue:**  
System experiencing errors impacting performance.

**Detection:**  
Observed system instability and errors.

**Investigation:**  
- Used `grep error /var/log/syslog` to identify error messages  
- Analyzed logs to determine root cause  

**Root Cause:**  
Identified error entries in system logs indicating underlying issue.

**Resolution:**  
Addressed the issue based on log findings.

**Validation:**  
System logs showed no further critical errors and system stabilized.

## 🛠 Commands Used

- ping
- traceroute
- netstat -tulnp
- grep
- top
