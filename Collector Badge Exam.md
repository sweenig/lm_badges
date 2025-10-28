> Which of the following is required for a collector to communicate with LogicMonitor?

* `Network access to LogicMonitor's servers via HTTP/TLS over port 443`
* A static IP address
* A dedicated VPN connection
* A proxy server

> When determining the optimal collector sizing and deployment strategy for a hybrid IT environment, which factors should you prioritize? (Select 2)

* The number of dashboards in LogicMonitor
* `Network latency between monitored resources and each collector host(s)`
* `The number of individual resources that a collector or group of collectors will need to monitor`
* Number of IT team members managing the LogicMonitor account

> A global enterprise manages multiple LogicMonitor Collectors across cloud and on-premises environments. What strategy best ensures monitoring continuity in the event of a collector failure?

* Increase CPU resources on the primary collector instead of using failover
* Rely on manual intervention to assign a new collector
* `Use a mix of ABCG for load balancing and One-to-One failover for critical resources`
* Implement only collectors hosted in the cloud for all environments

> What is a potential drawback of deploying only one Collector per region?

* It eliminates the need for failover configuration
* It requires multiple cloud-based dashboards
* `A single point of failure could impact monitoring continuity`
* The collector automatically scales with increased workloads

> What is the primary reason to deploy Collectors in multiple cloud regions?

* Ensuring proximity to monitored devices; each Collector should monitor cloud resources in the same region where it is installed
* `Deploying in multiple regions provides redundancy; Collectors in a different region will assume monitoring if one region experiences problems`
* To take advantage of LogicMonitor’s full suite of LogicModules
* Most companies experience significant cost savings from running resources in multiple regions

> When should a hybrid deployment strategy be used?

* When local monitoring is disabled
* For ensuring resiliency between multiple collectors
* `When resources exist both in the cloud and on-premises`
* When bandwidth is unlimited

> What are some indications that a Collector is overloaded and cannot keep up with its task load? (Select 2)

* `The collector is restarting multiple times per day`
* The LM Envision portal experiences slow load times
* `There are missed polls and gaps in graphs for devices monitored by the collector`
* There is a high percentage of failed API calls

> What is a drawback of not enabling automatic Collector failback?

* Collectors consume more bandwidth
* Updates are skipped
* `Primary Collectors may remain idle after recovery`
* Alerts are never escalated

> What does a large task queue in a Collector indicate?

* The Collector’s network configuration is invalid
* `The Collector is overloaded and cannot process tasks efficiently`
* Too many user accounts were created
* Device firmware is out of date

> What happens to a Collector when the collection interval for a particular LogicModule is reduced from every 10 minutes to every 1 minute?

* `The Collector’s workload may increase significantly, depending on the number of resources associated with the module`
* The system disables LogicModules
* The new collection tasks will be reassigned to another collector within an auto-balanced group
* Credentials are refreshed

> What is the benefit of configuring ABCGs in a dynamic cloud environment?

* Reduces LogicModule usage
* Enables SNMP polling
* Allows Collector logging to be disabled
* `Provides automated workload balancing and failover`

> What is the key metric that triggers rebalancing within an auto-balance collector group (ABCG)?

* One of the collectors in the group is on an unsupported version
* `The instance threshold set for a Collector is exceeded`
* One of the collectors in the group has missed multiple polls due to overload
* One of the collectors in the group has alerts for CPU and memory overload

> Why might you use a dedicated Collector for NetFlow data?

* To install fewer modules
* `To handle the volume and processing demand of flow traffic`
* To monitor user login attempts
* To suppress log-based alerts

> What is the primary purpose of enabling collector logging?

* `To track collector activity, troubleshoot issues, and detect security anomalies`
* To increase data storage limits
* To store user passwords securely
* To prevent collectors from sending monitoring data

> Why might a large enterprise need multiple collectors per region?

* `Ensure load distribution and resiliency`
* Decrease bandwidth billing
* Increase dashboard export frequency
* Improve customer login rates

> What does the LogicMonitor Collector do?

* `Acts as a bridge between infrastructure and LogicMonitor by collecting and transmitting data`
* Installs LogicModules
* Manages user access to LogicMonitor
* Provides reporting and visualization

> What is the primary function of the Collectors page in LogicMonitor?

* To adjust permissions for collector users
* To view a summary of recent alerts for monitored devices
* `To perform administrative tasks on Collectors including updates, configuring redundancy, grouping, and manual restarts`
* To configure data retention policies

> Which of the following best describes the role of Collector in LogicMonitor’s architecture?

* Stores raw monitoring data for historical analysis
* `Collects and transmits metrics and logs to the LogicMonitor platform`
* Generates reports based on historical data
* Manages the licensing of LogicMonitor users

> Which security measure within LM Envision can help to protect Collectors from unauthorized access?

* Disable all security features to simplify troubleshooting
* Restrict internet access to all collectors
* Rotate Collector credentials daily
* `Use role-based access controls within the portal to limit user access to Collectors`

> Which method ensures that a collector alert notification reaches the correct team for a timely response?

* Send all alerts to the entire company
* Only review alerts manually when performance issues arise
* `Assign an escalation chain for each Collector to a designated team or responsible individual`
* Enable alert suppression to avoid excessive notifications
