> Which task should be performed after reorganizing resource groups?

*  Manually rescan all resources to update property values.
*  Restart all Collectors to reapply inheritance rules.
*  Recreate all subgroups from the old structure.
*  `Validate that dashboards, alert routing, and user permissions still work as expected with the new grouping structure`

> What is the main goal of Resource Management in LogicMonitor?

*  `To organize monitored components for efficient data collection, alerting and visibility.`
*  To configure monitoring intervals for all LogicModules.
*  To ensure alert thresholds are applied globally to all resources.
*  To assign Collector updates to device types automatically.

> Why would administrators want to create their own custom properties for monitored resources, in addition to custom properties that are required for monitoring? 

*  They override all Auto Properties by default.
*  To automatically replace missing system properties.
*  They are required before any LogicModule can apply to a resource.
*  `To provide business context or custom information such as owner or environment`

> What is a key difference between Wizard Mode and Expert Mode when adding a resource?

*  Expert Mode automatically runs Active Discovery before saving changes
*  `Wizard Mode checks for credentials and tests communication, while Expert Mode skips validation`
*  Wizard Mode prevents adding resources to multiple groups
*  Wizard Mode only supports Windows resources, while Expert Mode supports all platforms

> Why might an administrator want to create a PropertySource to create properties, rather than manually setting them?

*  PropertySources allow administrators to bypass inheritance rules and overwrite system properties.
*  `PropertySources automatically assign and update properties at scale`
*  PropertySources store values permanently, even if the underlying conditions no longer apply.
*  PropertySources eliminate the need for credentials by detecting sensitive values automatically.

> After disabling a DataSource, why might instance-level changes no longer reflect?

*  Only multi-instance DataSources can update instance lists
*  Disabling a DataSource removes instances from the resource
*  `Active Discovery for that DataSource stops entirely when the DataSource is disabled`
*  A PropertySource suppressed instance updates

> Why would a multi-instance DataSource associate with a resource according to its AppliesTo expression, but not actually show up for that resource in the Resource tree?

*  The Collector does not have the correct access credentials
*  The DataSource is out of date
*  `Active Discovery did not find any monitorable instances`
*  The resource is still in the “unmonitored devices” group

> What happens when you manually run Active Discovery for a resource?

*  `LogicMonitor reevaluates instances for each applicable DataSource`
*  Collector assignment is recalculated
*  All DataSources are removed and reapplied
*  The resource is moved to the top of the Resource Tree

> What happens when a resource that belongs to one or more dynamic groups is deleted from LM Envision?

*  The resource remains in all dynamic groups until manually purged from each one.
*  `The resource is removed from the platform and no longer evaluated by any dynamic group criteria.`
*  Dynamic groups automatically re-create the deleted resource on the next poll cycle.
*  The deleted resource continues contributing metrics through its cached data.

> Two sibling groups, “Windows Servers” and “Domain Controllers”, each define a different value for win.pass. A server belongs to both groups. Which outcome can occur if this configuration remains unchanged?

*  The resource will fall back to inheriting the global credential instead.
*  The system will try both credentials and use whichever one the system responds to.
*  The value from the group with more resources will be used automatically.
*  `The resulting credential value cannot be predicted by the administrator because peer-level conflicts are resolved internally and not exposed in the UI.`

> What advantage does applying credentials at the group level provide?

*  Credentials inherited from groups always take priority over resource-level values.
*  Credentials at the group level cannot be overridden, ensuring consistency.
*  `All resources in that group automatically inherit the credentials, reducing manual configuration.`
*  Group-level credentials rotate automatically without administrator involvement.

> A team needs to use Resource Explorer to view only AWS resources in the US-West-1 region and organize them by type to see alert statuses. Which setup should they use?

*  Group By provider, then apply a filter for AWS without specifying the region
*  Filter by alert severity first, then Group By Collector group to narrow the resource set
*  `Filter by provider and region, then Group By resourceType`
*  Use Saved Views with default grouping and manually scroll to find AWS resources in that region

> In LM Envision, what best defines a “resource”?

*  A physical device like a server, switch, router or storage array
*  `Any monitored entity with its own IP address or DNS name that can provide performance data.`
*  A monitoring template used to collect data from multiple systems.
*  A grouping rule that defines device placement in the resource tree.

> What can occur if property inheritance is not carefully planned across nested groups?

*  Inherited properties are automatically ignored to prevent duplication.
*  All inherited values are merged into a single concatenated property.
*  `Conflicting values may cause LogicMonitor to choose a property randomly, leading to inconsistent results.`
*  The system halts data collection for resources in conflicting groups.

> When managing properties, what should administrators document to maintain configuration clarity?

*  `Each property’s purpose, scope, and the level at which it is defined.`
*  Only properties that contain credential information.
*  All temporary properties, since they are automatically deleted later.
*  Only properties inherited from static groups.

> What is one potential consequence of modifying AppliesTo logic in an existing dynamic group?

*  All inherited credentials are reset to default.
*  `Resources that no longer meet the criteria are automatically removed from that dynamic group’s membership`
*  The dynamic group may temporarily appear empty until the AppliesTo expression is re-evaluated.
*  Resources that newly match the updated criteria are automatically added the next time the group is evaluated.

> During Basic NetScan configuration, what drives the dynamic placement of discovered resources into default groups like “Devices by Type/Windows Servers”?

*  The Collector’s MAC-address lookup
*  The NetScan naming convention
*  `AppliesTo scripting criteria within each dynamic group`
*  The selected NetScan policy group

> A team dashboard is configured to use a filter for a custom property called “business_unit” where the value equals “Finance.” During a review, the team notices that several Finance servers are missing from the dashboard, even though data collection is working normally for those resources. After investigating, an administrator discovers that the missing servers have property values such as “finance,” “FIN,” or “Finance Dept.” 

> What is the most likely reason these servers are not appearing on the dashboard?

*  Dashboards ignore custom property filters unless the property is defined globally at the account level.
*  `The dashboard filter is matching a specific property value, and inconsistent custom property values prevented those servers from being included.`
*  PropertySources updated the values automatically, causing them to be hidden until rediscovery completes.
*  Dashboards only display resources that belong to static groups, so dynamic grouping caused them to be excluded.

> What is the impact of disabling alert generation for a resource group?

*  Only system-generated alerts will continue to function.
*  `No alerts will trigger for any resources in that group or its subgroups.`
*  Collectors will stop collecting performance data for those resources.
*  The group’s alert thresholds will reset to global defaults.

> Why should credential inheritance be planned carefully before adding large numbers of resources?

*  `It ensures credentials are applied in predictable locations and prevents accidental overrides that could break monitoring.`
*  Because inherited properties cannot include dynamic values.
*  Because properties cannot be edited once resources inherit them.
*  It allows LogicMonitor to generate credentials automatically for each resource.

> Which situation would most likely cause nondeterministic credential behavior across resources?

*  Basic system discovery re-runs after 24 hours
*  A resource inherits a property from a global level
*  `The same credential property is defined in two sibling groups`
*  A PropertySource adds a new system property

> An admin wants to move 40 resources into a different grouping structure and also update their Preferred Collector. Which method is most efficient?

*  Edit each resource individually from the Resources page to update group placement and Collector assignment
*  `Use the Resource Group’s Inventory tab to perform both Move to Group and Change Preferred Collector actions`
*  Modify Collectors directly from the Collector management page
*  Create a temporary dynamic group to reorganize the resources based on a shared property, and set the new Collector as the preferred collector for the dynamic group

> What is the primary function of a Collector in LogicMonitor?

*  It processes alert notifications and sends them to configured users.
*  It determines which resources belong in each dynamic group.
*  `It acts as the bridge that gathers performance data from resources inside your environment and sends it to LM Envision.`
*  It stores and encrypts credentials for all monitored systems.

> If the same property key is set at multiple levels with a different value for each, which takes precedence?

*  The value discovered automatically
*  `The value set directly on the resource`
*  The value inherited from the deepest subgroup
*  The value set at the highest level of the resource tree

> Which example best represents a secure property that LM Envision will automatically mask?

*  owner.email
*  `jdbc.mysql.pass`
*  location.site
*  system.sysinfo