**Issue Summary**

From 11:45 PM to 5:30 AM on November the 2nd in 2022, My server experienced an outage due to a prescheduled reboot that ended in failure. 
The points of failure are coming from the rebooting of the load balancer. Tried a maintenance update and a reboot notification for a window of 2:45 hours (11:45 PM to 2:30 AM). 
The root cause of the outage was due to the data on the the server not auto-mounting at boot time.

**Timeline**

11:45 PM: Reboot begins
12:26 AM: Outage begins
12:26 AM: Alerts sent
12:30 AM: Silenced all subsequent alerts due to server behavior being “normal”
1:30 AM: Server down and no one can reach the site
1:30 AM: Alerts sent
2:30 AM: Server restarts begin
5:30 AM: 100% of traffic back online

**Root Cause**

At 12:26 AM, the reboot of the load-balancer continued to fail. The failover server (secondary server) did not come back up for for 3 hours. 
The software update was fine, yet it affected the overall performance of the site. 
It was not reconnecting to the secondary server. It seems like the incident to be a routine behavior of a server reboot, thus any further alerts were silenced automatically.

**Resolution and Recovery**

The NSX CLI is used to get detailed information about tail logs and take packet captures. It also, looks at the metrics for trouble shooting the load balancer.
Verification of basic services are running by checking the routing table.
Processes started to recover slowly. We estimated time to reboot and recovery time to span 4 hours.
To help with recovery, we retarted affected servers. I manually restarted unicorn processes on the web application servers to further correct the reboot process.
The process was slow to prevent any possible cascading failures and to avoid a wide scale reboot — affecting our customers even further.
By 5:30 AM, traffic was restored.

**Corrective and Preventative Measures**

 In the last 2 to 5 days, I’ve made an internal review and analysis of the outage. The following measures are actions that I will follow for prevention and to improve response times in the future.
 An update to their systems to prevent further issues in the future are done accordingly. There were no one present to possibly resolve the situation by manually fixing any issues that came up.
 For scheduled reboots like this, there should be a 24 hour operations rotation in order to monitor every aspect of the update.
