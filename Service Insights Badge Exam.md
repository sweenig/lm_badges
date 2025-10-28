
> Why is customer complaint volume not considered a direct performance metric in LM Envision?

* `It doesn't provide real-time infrastructure data`
* It cannot be tracked by LM Envision
* It reflects only external feedback, not internal availability
* It’s only relevant for the HR department

> Which of the following best describes the limitation of a single auto-created DataSource for service monitoring?

* It applies different aggregation methods to the same datapoint
* `It combines unrelated datapoints into a single source, reducing clarity`
* It cannot be viewed or edited through the Module Toolbox
* It is unable to collect metrics from databases or network devices

> Which of the following would not typically be considered a business service for most organizations?

* `Web application firewall`
* Customer portal
* Communication platform
* Order processing system

> You are reviewing one of the auto-created services. How do you find the DataSource used for monitoring it?

* Search the log files from the collector
* `Open the service and view the LogicModule in the Module Toolbox`
* View the Alerts tab for the resource group
* Run a report on all devices in the portal

> What is the collection type used in the LogicModule created by a service auto-creation rule?

* Scripted metrics
* Raw data
* Collector-level data
* `Aggregate data`

> What is one reason separating application, database, and network metrics into different DataSources might be preferred for Service monitoring?

* `It makes it easier to troubleshoot issues by isolating health indicators`
* It eliminates the need to assign service properties during setup
* It reduces the overall number of resources required for monitoring
* It prevents LM Envision from generating too many alerts

> Fill in the blank. In LogicMonitor, Conditional Count is useful for ___________.

* `detecting how many service members meet a specific condition`
* importing metrics from external APIs
* identifying configuration drift between services
* building collector groups

> What is the primary purpose of monitoring a business service from a top-down perspective?

* `To understand how individual IT components support overall business objectives`
* To collect more metrics for dashboards
* To track employee productivity in IT teams
* To monitor services without considering dependencies

> What does LogicMonitor create when you configure a new service with selected metrics and aggregation methods?

* `A new DataSource that performs aggregate calculations`
* A synthetic transaction to represent service latency
* A custom script that polls each device directly
* An API-based plugin that replaces the original DataSources

> You are configuring a service to monitor a group of web servers. You want to generate an alert if more than two servers are unavailable at the same time. Which aggregation method and metric configuration might you use?

* Use the "mean" method on CPU to calculate the average across servers
* Use the "max" method on memory usage to detect outliers across servers
* Use the "sum" method on a response time metric to track performance spikes
* `Use a "conditional count" on a status datapoints to count how many servers are down`

> Which aggregation method should you use if you want to track the average response time across multiple web servers?

* Threshold
* Maximum
* `Mean`
* Sum

> What does “cardinality” refer to in the context of auto-created services?

* The size of the LogicModule used to build the service
* The performance threshold used in alerting rules
* `The number of services created based on property combinations`
* The number of metrics selected for each rule

> Which of the following can be configured when creating an Auto Creation Rule? (Select 2)

* `Filters to exclude resources without required tags`
* The polling frequency of each individual service
* `A naming pattern based on device properties`
* Historical log data from services before creation

> How are services named automatically during rule creation?

* `By combining selected property values with optional prefixes and suffixes`
* By appending the current date to each resource name
* By using a fixed string applied to every service
* By using LogicMonitor's default service naming algorithm

> Why might you choose instances instead of entire resources as service members?

* `Only specific instances contribute to the service’s functionality`
* Only instances allow metrics to be aggregated
* Instances reduce licensing costs in LogicMonitor
* Instances allow services to include resources from multiple regions
