> Your team suspects that certain thresholds are configured differently across similar servers that should have the same thresholds. What tool could help you identify and clean up these inconsistencies?

* Resource Explorer
* Collector Status Report
* `Alert Thresholds Report`
* Device Dashboard

> You are monitoring API response times in LogicMonitor. You want to detect both fixed violations (above 2 seconds) and abnormal patterns. Which threshold strategy best meets your goal?

* `Hybrid thresholds (combine static and dynamic)`
* Static thresholds
* Dynamic thresholds
* No thresholds

> Before an alert can be routed to a tool like ServiceNow or Jira, what must be done?

* Configure the integration and associate it with a device or group
* `Configure the integration, add it to an escalation chain, and build a rule pointing to the chain`
* Add the integration directly as the recipient of an alert rule
* Enable API access for the integration under “Portal Settings”

> For how many consecutive polls must behavior report as ‘normal’ before an alert clears?

* Alerts clear immediately when the value no longer meets the threshold condition
* It depends on the escalation chain configured for each alert
* 3 consecutive polls, to ensure the issue is truly fixed
* `It depends on the Alert Clear interval in the DataSource`

> When using default settings for a dynamic threshold, what happens when a datapoint’s value is more than 3 band factors from normal for five consecutive polls?

* The alert is suppressed automatically
* The system clears all previous alerts
* `A critical alert is triggered`
* A warning alert is generated

> How much training data is required for LogicMonitor to calculate a baseline for dynamic thresholds when the polling interval is 15 minutes or less?

* 5 hours of data
* `12 hours of data`
* 1 day of data
* 7 days of data

> What benefit does adding custom columns to the Alerts table provide?

* It displays alert severity levels
* It allows for better collaboration when troubleshooting
* It automatically displays alert rules and escalation chains
* `It can provide additional context to help teams prioritize alerts faster`

> If an alert matches more than one alert rule, and the rules have the same priority number, what will happen to the alert notification?

* The rule that comes first alphabetically will take precedence
* `It is indeterminate which rule will take precedence`
* The system routes notification to both destinations
* All rules are ignored and the alert will not be routed

> How do dynamic thresholds determine what is considered “normal” behavior?

* By replicating other devices’ thresholds
* By comparing device performance with other similar devices
* `Using algorithms that analyze historical performance data`
* By using fixed percentage values

> Which of the following best describes the warning alert severity in LogicMonitor?

* A condition that requires immediate attention
* `A condition that could potentially become a problem`
* A condition that indicates a confirmed system failure
* A condition that requires no action from users

> If you monitor a legacy file server with predictable performance, which threshold type is most appropriate?

* No Threshold
* `Static Threshold`
* Dynamic Threshold
* Critical Threshold

> Why should alert tuning be considered an iterative process?

* Because ITIL recommends quarterly tuning
* `Because environments change over time`
* Because alerts clear after 90 days
* Because tuning cannot be automated

> What is the purpose of the “Trigger Interval” setting in alert thresholds?

* To define the alert’s escalation timing
* To determine how often dashboards refresh
* `To define how many consecutive polls the condition must exist before alerting` (FYI, this should be ***how many consecutive poll cycles*** or ***how many consecutive polls beyond the first***)
* To specify how long to wait between stages of an escalation chain

> What does Root Cause Analysis (RCA) do in LogicMonitor?

* Automatically summarizes related alerts into a single report
* Temporarily disables polling for affected resources
* Automatically clears dependent alerts once the root cause is resolved
* `Suppresses downstream alerts that stem from a single failure`

> Why is it best practice for each DataSource to include a “No Data” alert on only one datapoint?

* Because multiple “No Data” alerts could suppress other alert types from firing
* Because multiple “No Data” alerts slow down collection
* `One is sufficient because usually if one datapoint stops working, all the others will also stop working`
* Because “No Data” alerts consume extra storage

> What happens when a metric’s value returns to normal and remains stable through the clear interval?

* The alert must be manually acknowledged
* `The alert automatically clears`
* The alert remains active until an acknowledgment is received
* The alert transitions to a ”clear” state but stays visible in dashboards until manually cleared

> What is the purpose of an "escalation chain” in LogicMonitor?

* It defines the official troubleshooting steps for each alert
* `It defines the destinations of an alert notification`
* It assigns ownership for resolving alerts
* It determines which alerts will be routed to which places

> Where can dynamic thresholds be configured in LogicMonitor?

* `At any level of the resource tree or in the DataSource definition`
* On the Alerts page
* Only at the instance level
* Only globally in the DataSource definition

> What permissions must a user have to configure alert routing in LogicMonitor?

* Manage permissions for “Alert Rules”
* Full administrator permissions to “account settings”
* `Manage permissions for “Alert Settings”`
* Full administrator permissions for the portal

> Why is it recommended to use a placeholder “Integrations” user when adding a user to an escalation chain?

* To ensure alerts bypass all normal routing
* To simplify permissions management for API users
* `To simplify management and avoid confusion of attaching it to a random real user`
* To ensure all integrations share the same notification settings

> What does the blue shaded area represent when viewing a dynamic threshold graph in LogicMonitor?

* The critical alert range
* The min, max and average values for the datapoint over time
* `The expected range of a datapoint’s normal behavior`
* The manual override area

> Which filter option helps you view alerts that are no longer active?

* Severity filter set to “Warning”
* `Cleared filter set to “Yes” or “All”`
* Time range set to “Last 24 Hours”
* Acknowledged filter set to “All”

> What does the alert clear interval determine in LogicMonitor?

* How often notifications are resent during escalation
* `How many polling cycles a metric must remain normal before the alert clears` (FYI this should read ***How many polling cycles beyond the first*** or ***How many polling cycles besides the first***)
* How often the system checks to see if the alert still meets the threshold condition
* How long LogicMonitor waits before automatically resetting the threshold

> What types of alerts can be viewed on the Alerts page?

* Threshold-based alerts
* Escalation chain alerts only
* `Metric, Log, Config, and Service alerts`
* Security and compliance alerts

> What should you do if a datapoint frequently triggers alerts but requires no action?

* `Suppress or tune the alert to reduce noise`
* Escalate the alert to critical
* Disable the datapoint
* Route notifications to email instead of a text or voice call notification

> What is the role of an alert rule when integrating with external systems?

* To override all escalation chains and use the integration instead
* `To determine which alerts are sent to the integration`
* To select the escalation chain associated with an integration.
* To format alert messages for ticket creation

> What is the purpose of acknowledging (ACK’ing) an alert?

* `To signal ownership and stop further alert notifications`
* To mark the alert as resolved and close the ticket automatically
* To temporarily silence the alert while maintaining escalation state
* To clear the alert immediately

> How much historical data does LogicMonitor use to refine dynamic threshold calculations over time?

* 30 days of data
* 24 hours of data
* `Up to 15 days of recent data`
* 1 week of data

> A monitoring team wants to sustain effective alert tuning across their organization. Which two practices should they adopt? (Select 2)

* Route all alerts globally to ensure visibility
* `Regularly review`
* Disable all “No Data” alerts for simplicity
* `Alert reports to identify noiseUse dashboards to visualize alert trends and threshold breaches` (This typo should probably be fixed)

> What does the Filter Bar on the Alerts page allow you to do?

* `Narrow alerts by severity, time range, and alert type`
* Change Collector configurations
* Schedule maintenance windows globally
* Modify DataSource polling frequency

> Why might a user enable both static and dynamic thresholds on the same datapoint? (Select 2)

* To remove the need for manual tuning
* `To provide coverage for both fixed limits and abnormal behavior`
* To reduce alert noise, in the case that a static threshold is hit but the behavior is normal <- This is the right answer, but the test software thinks it's not. (LM may fix this)
* `To disable alerts for duplicate datapoints` <- This is not the right answer, but the test software thinks it is.

> What is a recipient group within an escalation chain?

* A placeholder used to store inactive recipients
* `A collection of users or contacts that receive alerts as a single entity`
* A list of devices associated with a collector
* A temporary set of filtered alerts

> Which report provides full details of each alert, including severity and triggering value?

* `All Alerts from Last 24 Hours Report`
* Alert Routing Summary
* No Data Report
* Alert Frequency Report

> What happens when an alert is escalated manually?

* It re-sends the notification to the same stage for confirmation
* `It immediately notifies the next stage in the escalation chain`
* It automatically raises the alert to the next severity level
* It resets the escalation interval timer

> Which token dynamically inserts the value that triggered an alert into the message?

* ##LEVEL##
* `##VALUE##`
* ##NUMBER##
* ##THRESHOLD##

> What is required for a dynamic threshold to begin generating alerts? (Select 2)

* `A sufficient baseline of historical data`
* `A deviation from normal behavior`
* Nothing is required; dynamic thresholds work out-of-the-box, similar to static thresholds
* Static thresholds must also be enabled for the datapoint so the system can determine normal behavior

> What is the purpose of using forecasting in LogicMonitor?

* To visualize projected capacity limits for monitored metrics
* To automatically adjust thresholds based on usage trends
* To test alert routing without sending notifications
* `To predict when a datapoint may reach alert status based on historical trends`

> How does a time-based escalation chain differ from a standard one?

* It adjusts escalation timing based on how long an alert remains unacknowledged
* ` It routes alerts differently based on the day or time the alert was triggered`
* It automatically suppresses alerts during scheduled downtime periods
* It prioritizes alert delivery by alert severity instead of by user group

> If you want to apply unique thresholds to a single disk on a specific server, where should you tune?

* Global level
* Group level
* Device type level
* `Instance level`

> At which level do threshold settings override all others in LogicMonitor?

* `Instance level`
* Group level
* Resource level
* Global level

> What is the function of rate limits in escalation chains?

* `To prevent excessive notifications within a given time period`
* To slow down data collection rates
* To suppress alerts during downtime
* To limit how often alerts can re-trigger within a given timeframe.

> Sophia’s team receives dozens of CPU alerts for >80% usage across many virtual machines. After investigating, she finds this level is normal for their workload. What action should Sophia take to reduce noise while maintaining useful alert coverage?

* `Tune the default CPU threshold for the VM group`
* Disable all CPU-related DataSources
* Change all alert severities from critical to warning
* Delete the inherited thresholds from the DataSources

> Which severity level is used when a datapoint slightly exceeds its normal range?

* Error
* `Warning`
* Informational
* Critical

> What is the purpose of a ‘No Data’ alert?

* To alert when a Collector is unreachable
* `To alert when a device stops responding entirely`
* To alert when a threshold value is too high
* To alert when an alert clears prematurely

> If you are not seeing an expected alert on the Alerts page, what should you check first?

* The alert routing settings
* The raw data tab
* ` The filters and time range on the Alerts page`
* The alert threshold

> What determines whether an alert is routed to a specific destination?

* The value of the tokens in the alert’s message template
* Whether it is in a particular resource group
* `Whether it matches the parameters set in the alert rule`
* The type of device generating the alert

> What is a band factor in the context of dynamic thresholds?

* A limit for the number of alerts per minute
* `A measure of deviation from normal behavior`
* A percentage of total device uptime
* It represents the fixed value of the dynamic threshold at any given time

> What is the main purpose of LogicMonitor’s default thresholds?

* To ensure every device is held to the same alerting standards
* To eliminate the need for manual alert configuration
* `To provide an initial baseline for alerting that can be tuned for your environment`
* To ensure manufacturer guidelines are followed

> Why is it important to tune LogicMonitor’s default thresholds?

* `Because default thresholds won’t always be accurate for your specific environment`
* Because thresholds are only applied to new devices
* Because tuning is required to activate alert routing
* Because default thresholds cannot generate critical alerts

