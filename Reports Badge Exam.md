# Reports

> A manager wants a report that highlights trends in application errors without displaying every individual log entry. Which result type should be selected?

* Basic & Aggregation
* Basic
* `Aggregation`
* Raw Events

> How do threshold limits vary? (Select 3)

* `By export format`
* `By report type`
* `By generation method`
* By report group

> An administrator is creating a Metrics Explorer report for all production web servers. The server names follow a naming convention such as web-prod-01, web-prod-02, and web-prod-03. Which filter expression is most appropriate?

* Use the != operator to exclude all production servers
* `Use the =~ operator to match the naming pattern`
* Use the = operator to match a single server
* Use the !~ operator to exclude matching server names

> Which type of question is best answered by a report instead of a dashboard?

* `Which resources had the highest CPU usage during the last 30 days?`
* Which dashboard widget should be resized?
* Which alert rule should be muted right now?
* Which services are currently showing warning status?

> When should a report be scheduled instead of run ad hoc? (Select 2)

* `When it is needed regularly`
* When previewing report output
* When testing filters
* `When it involves large data`

> When should you enable Allow Shared Reports?

* When filtering data
* `When sharing with users who do not have login access`
* When scheduling reports
* When exporting CSV files

> A Metrics Explorer report returns every Linux server, but one test server named "linux-test-01" should not appear in the results. What is the best way to modify the filter?

* Use the = operator to match every Linux server
* `Use the != operator to exclude the test server by name`
* Use the =~ operator to match only the test server
* Use the !~ operator to exclude all Linux servers

> Before saving a Metrics Explorer report, an administrator wants to verify that Query Builder generated the expected LMQL syntax. Which feature should they review?

* Report History
* Export Preview
* Report Schedule
* `Query Preview`

> Which type of question is best answered by a Log Query Report?

* Which users are inactive?
* `Which log events match this query?`
* Which resources belong to which groups?
* How long were resources in alert?

> You are creating a Resource SLA Report for four production application servers. The service is considered available only if all four servers are simultaneously meeting their SLA targets. Which Calculation Method should you choose?

* Percent all resources available
* Only display Resources with less than 100% availability
* Average of all SLA Metrics
* `Display SLA Summary (Total %)`

> A report needs to focus only on Linux servers in a large mixed environment. What is the best approach?

* Apply a Time Range filter
* Sort By field
* `Use a dynamic group`
* Select all resources

> A company stores operational reports and executive reports in separate report groups. A user has Manage permission only for the operational report group. Which outcome is expected?

* The user automatically receives View permission for every report group.
* `The user can create, edit, schedule, and delete reports only in the operational report group.`
* The user can generate executive reports but cannot manage operational reports.
* The user can edit reports in both groups but schedule reports only in the operational group.

> A security analyst needs to review specific log messages related to an incident over the past week. Which report should be used?

* `Log Query Report`
* Alert Report
* Metrics Explorer
* Audit Log

> Which report helps confirm whether alerts were suppressed during maintenance?

* `SDT Inventory`
* Metric Report
* Resource Inventory
* Alert Trends

> Why is sorting by severity useful?

* It reduces data volume
* It changes report scope
* `It prioritizes critical alerts first`
* It removes low alerts

> What does enabling the 95th percentile option in an Interface Bandwidth report help determine?

* The total volume of inbound and outbound traffic transferred
* The single highest bandwidth value recorded during the report period
* The arithmetic mean of all bandwidth samples during the report period
* `The sustained bandwidth level after excluding brief usage spikes`

> A user has Manage permission for a report group. When they generate a report, they notice that some resources included in the same report when run by an administrator are missing from their results. What is the most likely explanation?

* The report was configured to display only resources owned by the user who generated it.
* `The user's role does not have permission to view certain resources, so those resources are excluded from the generated report output.`
* Manage permission allows users to modify reports, but only administrators can generate reports that include all monitored resources.
* The report group's Manage permission only allows users to generate reports for resources they have personally added to the group.

> Why is consistent naming important?

* It increases report performance
* It controls access
* `It improves report discoverability`
* It reduces data size

> What is a key risk of deleting a report?

* `Disrupting recurring workflows`
* Increasing report size
* Reducing report accuracy
* Slowing system performance

> A user is building a query for a Metrics Explorer Report and clicks Validate before saving. What is the primary purpose of this step? (Select 2)

* To convert the report into a scheduled report
* `To ensure selected criteria produce valid report results`
* To compress the report output before export
* `To check that the query syntax is correct`