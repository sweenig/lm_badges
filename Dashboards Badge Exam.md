> Which of the following is a benefit of operational visibility through dashboards?

* Manages billing and invoicing
* Helps set up new users
* Tracks training attendance
* `Improves real-time system awareness`

> Why might a dashboard appear empty even though data is configured?

* `Time range is set incorrectly`
* Wrong LogicModule
* User lacks permissions ***I'd argue that this one is correct too***
* The dashboard is set to private

> In a “top 10” Dynamic Table widget, why might values differ from those in a “top 10” Custom Graph widget, if both widgets are referencing the same resources and datapoints?

* The table uses historical averages
* `The graph shows trends over time; the table shows the latest reported value`
* The table rounds all values
* They are based on different servers

> What does the slideshow feature in LogicMonitor do?

* Creates visual alerts
* `Cycles through a set of dashboards on a loop`
* Cycles through a fullscreen view of each widget on a dashboard
* Puts dashboards in full-screen view

> What does a Custom Graph Widget allow you to do?

* `Compare trends over time using multiple datapoints`
* Filter alerts by severity
* Visualize a single large number
* Embed external content

> Which of the following fields does NOT support dashboard tokens?

* `Datapoint`
* Title ***This is partially correct, widget titles support tokens while dashboard titles do not***
* Resource
* Group

> What must a LogicMonitor role include to view dashboard widget data?

* Access to Settings > Global
* Widget editing permissions
* `View access to both dashboards and related resource groups`
* View access to the dashboards only

> After importing a prebuilt dashboard from GitHub, the graphs are blank. What is a likely cause?

* Alerts were disabled
* The dashboard is using outdated widgets
* Filters were deleted
* `Token values haven’t been configured`

> When cloning a dashboard with a group token, what must you do to make it useful for a different region?

* Recreate the dashboard from scratch
* Update each widget’s threshold
* Change the token’s display name
* `Modify the token value at the dashboard level`

> Which widget field allows for filtering data to show only metrics for the C:\ drive?

* Resource
* `Instance` ***this assumes LM's datasource, not a custom one where a datatpoint might be dedicated to the C: drive***
* Group
* Datapoint

> Why should dashboards avoid including too much data?

* `It reduces focus and obscures key insights`
* It causes slower load times
* It increases security risks
* It violates data visualization guidelines

> Mike just integrated a GCP account into LogicMonitor. What should his first step be to gain insight into the environment?

* `Review and modify the out-of-the-box GCP dashboards`
* Disable alerts until further configuration
* Create a custom dashboard from scratch
* Import all historical data manually

> Which widget type is best for displaying a large, single KPI in bold?

* Alert List Widget
* `Big Number Widget`
* Custom Graph Widget
* Gauge Widget ***I'd argue this is right too if the KPI has known upper and lower bounds***

> Which of the following scenarios best illustrates the need for dashboard filters?

* You are importing a dashboard from GitHub
* `You need a single dashboard to visualize different office locations`
* You want to create custom color themes per user
* You want to set alert thresholds for multiple metrics

> Which scenario demonstrates a correct use of dashboard tokens?

* Typing ## into a widget title to hide its label
* `Using ##defaultResourceGroup## in the “group” field of each widget rather than a hard-coded value`
* Using * in the group field of each widget to make the dashboard dynamic
* Using tokens to store alert history logs

> When cloning a dashboard to make a copy for each cloud region, which approach saves the most time?

* `Use a token in the Group field of each widget`
* Edit LogicModules for each resource
* Create a filter for each new region
* Recreate every widget manually

> What’s the key difference between a public and private dashboard in LogicMonitor?

* Public dashboards are visible to anyone with a link, whereas private dashboards can only be seen by authenticated LogicMonitor users
* `Private dashboards are visible only to the creator and admins, whereas public dashboards are visible to any user with appropriate permissions`
* Private dashboards cannot be imported or exported, while public dashboards can
* Private dashboards cannot use tokens or filters, while public dashboards can use both these features

> Why is it important to tailor dashboards to different personas?

* To prevent dashboard deletion
* To match each team’s aesthetic preferences
* `To align metrics and data views with each role’s goals`
* To ensure the same view is used by all roles

> What should Maria do to adapt a dashboard for another regional site?

* Change widget types
* `Update the tokens to reference the new group`
* Duplicate the widgets only
* Rebuild the dashboard from scratch

> You’re analyzing disk usage and want to track which disks have crossed 85% capacity. Which feature could help you visualize this threshold on a graph?

* Add a gauge with warning range at 85%
* `Add a virtual datapoint to create a visual threshold line at 85`
* Set an alert threshold on the “percent used” datapoint to trigger alerts when usage hits 85%
* Add a DataSource filter for the disk capacity DataSource, and the alert thresholds for that DataSource will automatically appear on the graph