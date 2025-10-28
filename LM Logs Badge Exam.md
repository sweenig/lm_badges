> What is a log anomaly in LM Logs?

* A log message that appears on multiple servers
* A log message that is always logged at the same time
* A duplicated error message
* `A log message pattern or structure never seen before for a resource`

> After deploying new log-based alerts, your team receives too many non-critical alerts. What should you do first?

* Increase the volume of alerts for visibility
* Disable all alerts
* `Refine the log alert query logic with log_level ="critical"`
* Convert all alerts to metric-based

> An organization wants to reduce the frequency of major incidents. They implement anomaly reviews, but only perform them on a quarterly basis. What change might improve or accelerate the results they’re seeing?

* Disable anomaly alerts
* Increase log retention only
* Focus only on metric dashboards
* `Move reviews to a weekly or bi-weekly cadence`

> What query configuration would NOT be used to look for failed login attempts?

* `_resource.group = “failed passwords”`
* _message ~ "failed login"
* _message ~ "authentication failed"
* message = “login failed”

> What is one benefit of using LM Logs for analyzing logs and metrics together?

* Reduces log data retention
* Requires fewer licenses
* Hides irrelevant alerts
* `Speeds up root cause identification`

> What field can be used in a query to search for alerts based on message severity?

* sys.sevflag
* _event.code
* Priority_tag
* `log_level=”critical”`

> Why might a user switch from Log Anomalies to All Logs when troubleshooting?

* `To view additional correlated logs not flagged as anomalies`
* To bypass the Overview tab
* To escalate incidents
* To trigger alert policies

> What capability allows users to identify relevant log messages without using the query language?

* Sentiment Graphing
* Log Exports
* `Log Analysis`
* Alert Aggregation

> You detect a concerning new anomaly type during testing in a staging environment that could also impact production environments. What should you do next?

* `Create a pipeline alert for similar patterns in all environments`
* Wait until users report issues
* Assume patterns are the same across environments
* Delete the staging logs

> Compare traditional log tools with LM Logs. What makes LM Logs more efficient in hybrid environments?

* `Full-context view via log and metric correlation`
* Limited platform support
* Manual query requirements
* Multi-tool dependency

> What does a keyword search in LM Logs primarily scan?

* User profiles
* `Log message field`
* Aggregated metrics
* Device configurations

> Which type of search is used to match field-value pairs exactly?

* `Exact match`
* Fuzzy match
* Regex
* Keyword

> A log anomaly flagged a minor disk issue. After investigating, you realize it could quickly escalate to a more serious problem. How do you move from detection to prevention?

* Delete the logs to save space
* Label the issue as low priority and archive it
* Schedule a reboot
* `Create a pipeline alert and apply it to all similar resources`

> Which log condition is required for anomaly detection to work in LM Logs?

* The log must have the word “ERROR”
* The log must be exported to CSV
* The log must be saved in a pipeline
* `The log must be mapped to a resource`

> What is the purpose of importing pre-written queries into LM Logs?

* `To easily add additional queries efficiently`
* To generate network maps
* To delete saved logs
* To limit user access to queries

> How do low-frequency log patterns assist in root cause analysis?

* They are always less relevant than high-frequency patterns
* They are filtered out automatically
* `They help identify rare or less recurring log events related to the issue`
* They usually indicate configuration backups

> Your team receives repeated alerts from a known system behavior. How can LM Logs help prevent repeated investigations of the same issue?

* Disable logging temporarily
* `Create a log alert pipeline and configure alert trigger conditions.`
* Filter out logs by severity
* Use static dashboards for alert review

> What is the default acknowledgement behavior for a basic log alert?

* Escalates after 5 minutes
* Auto acknowledgement after 4 days
* Never clears unless manually closed
* `Auto acknowledgement after 60 minutes unless modified`

> Which log type would best help a DevOps team monitor real-time application behavior and performance?

* Syslog
* Audit Logs
* `Application Logs`
* Windows Event Logs

> What is the purpose of resetting the anomaly detection profile in LM Logs?

* To enable automatic patching
* `To update the system's understanding of normal log behavior`
* To permanently delete archived log entries
* To clear log storage space

> A junior engineer needs to investigate a failed service but lacks knowledge of log query syntax. What could they use to complete the investigation efficiently?

* SNMP logs
* `Log Analysis with sentiment scoring`
* Alert History tab
* Read through all logs around the timeframe of the incident

> Which LM Logs feature allows users to save and reuse searches for known failure patterns?

* `Saved Queries`
* Log Search Templates
* Pattern Archives
* Graph Bookmarking

> Your team is investigating an outage in a hybrid infrastructure setup. How should LM Logs be used to shorten the Mean Time to Resolution (MTTR)?

* Assign multiple engineers to run independent queries
* Export logs to a third-party analytics platform
* Use traditional Syslog-only tools
* `Leverage LM Logs’ anomaly detection and correlate metrics on the same screen`

> Your alert fires on each error message, even for known benign issues. What is the best way to refine the alerting logic?

* Shorten the time-to-clear window
* Rely only on stateful alerts
* Turn off the alert completely
* `Use keyword filters with exact match or regex and include only critical sources`

> Which filter identifies anomalies that are “never before seen”?

* `_anomaly.type = “never_before_seen`
* _regex.error = “first_seen”
* _alert.source = “critical”
* _anomaly.level = “error”
