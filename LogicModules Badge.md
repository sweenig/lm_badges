> A security team needs to search and analyze historical authentication failures across all Linux servers over the past 30 days. Which LogicModule type is designed to support log ingestion and storage for searching and analysis?

* DiagnosticSources
* RemediationSources
* EventSources
* `LogSources`

> A LogicModule’s AppliesTo expression evaluates to False for a resource. What is the result?

* The resource is marked as unmonitored.
* `The module does not associate with the resource.`
* The Collector retries the evaluation every minute until it returns True.
* The module associates but remains disabled.

> Where can users visualize topology relationships for a resource?

* In the Raw Data tab of a TopologySource
* Under Settings > Modules > TopologySources
* Under Settings > Maps
* `On the Maps tab of the resource or resource group`

> Which of the following best describes the purpose of the AppliesTo field in a LogicModule?

* `It evaluates a logical expression to determine whether the module associates with a resource.`
* It defines the data collection interval for a module.
* It assigns credentials to a resource during discovery.
* It controls which dashboards display the module’s data.

> Which of the following LogicModule types primarily provide contextual relationships between resources but do not typically generate alerts?

* LogSources
* DataSources
* `TopologySources`
* ConfigSources

> Which LogicModule types can be configured to alert on specific patterns or anomalies within log messages? (Select 2)

* PropertySources
* `EventSources`
* `LogSources` (FYI, this is technically not correct since you don't set the alert threshold on the module, but in the alert pipeline/pipeline alerts. You can ingest logs without any LogSources and still set alert pipelines/pipeline alerts.)
* ConfigSources

> What happens when you install an updated version of a LogicModule?

* A duplicate module is created automatically.
* `The existing installed version in your portal is overwritten.`
* The module is marked as deprecated.
* The update applies only to new resources.

> What is the primary purpose of a TopologySource?

* `To discover and define relationships between resources for dependency mapping`
* To classify resources into relationship categories for monitoring applicability
* To automatically create ERIs (external resource identifiers) for resources and instances
* To collect connectivity metrics used to infer dependencies

> Which settings can be preserved during a module update? (Select 2)

* `Alert Thresholds`
* Collector installation path
* `AppliesTo`
* User role assignments

> A module is marked as “Deprecated” in My Module Toolbox. What does this indicate?

* The module cannot collect data.
* The module has been customized locally.
* `The module is planned for removal in a future release.`
* The module has already been deleted from the portal.

> Which property is unique in that it can contain multiple comma-separated values and is frequently used in AppliesTo logic?

* `system.categories`
* system.collector
* system.hostname
* system.displayname

> When a DiagnosticSource is executed automatically by a Diagnostic Rule, when does it run?

* `When a matching alert meets the defined rule conditions`
* On a fixed 24-hour schedule
* Only during resource onboarding
* When a PropertySource reruns

> What is the primary role of a DataSource in LogicMonitor?

* To execute corrective actions when alerts occur
* To classify resources and assign system properties
* `To collect numeric time-series data that drives graphs and metric-based alerts`
* To generate topology maps between related devices

> You see a module with the status “Update” in My Module Toolbox. What does this mean?

* The module is no longer associated with any resources.
* The module has failed to collect data.
* `A newer version of the installed module is available in Exchange.`
* The module has been deprecated and removed.

> Which of the following is a customer-managed responsibility within their own portal environment?

* Publishing official modules to the Exchange
* Automatically deploying new module updates to all customer portals
* `Choosing when to add new modules and apply module updates`
* Performing security reviews of community-submitted modules before publication

> Which changes are most likely to impact monitoring coverage after a module update? (Select 2)

* User role permission updates
* `Active Discovery changes`
* `AppliesTo changes`
* Dashboard layout changes

> Which component of a LogSource helps reduce noise by limiting which log entries are processed?

* `Filters`
* AppliesTo
* Resource Mapping
* Basic Information

> What role does the system.categories property play in device classification?

* It defines how a device is grouped within the Resources tree
* It automatically assigns specific DataSources and other LogicModules to a device
* It determines which Collector a device is assigned to
* `It stores category values that can be used as part of LogicModule AppliesTo logic`

> Which scenario most appropriately uses a complex datapoint?

* Discovering new virtual machines on a host
* `Calculating disk usage percentage from total and used space values`
* Mapping dependencies between two servers
* Polling a device for SNMP interface counters

> How are Diagnostic Rules used within LogicMonitor?

* To assign DiagnosticSources to resources during onboarding
* `To automatically execute a DiagnosticSource when defined alert conditions are met`
* To modify alert routing or escalation behavior when specific alerts trigger
* To schedule recurring diagnostic executions at fixed intervals