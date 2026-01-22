

> You attempt to remove an outdated correlation model from Edwin AI but find there is no delete option. What should you do instead, and why?
* `Archive the model to retain its configuration history and ensure auditability`
* Deactivate the model and wait for it to expire automatically
* Export the model and manually delete it from your system logs
* Clone the model and overwrite the existing version to remove it

> Why should API credentials be assigned to a dedicated API user rather than a personal account?
* To ensure the API user has unrestricted administrator access
* To bypass role-based access controls within LogicMonitor
* Because personal accounts cannot create API keys
* `To prevent integration failures when individual users leave the organization`

> An organization wants its on-call engineers to decide when to create an incident rather than having it done automatically. Which configuration supports this workflow?
* Enable the “Close Incident” stop condition in the action group.
* `Use an interactive rule linked to a manual “Create Incident” action group.`
* Set the rule type to automatic for faster response.
* Disable all mapping between Edwin AI and ServiceNow.

> Why is it recommended to clone a rule instead of editing an existing one?
* `Cloning preserves the original baseline configuration for version control and rollback.`
* Cloning disables automatic triggers.
* Editing is faster and ensures immediate deployment.
* Editing prevents duplicate rule creation.

> When evaluating third-party integrations in Edwin AI, which governance principle ensures data relevance and system performance?
* Allow multiple overlapping integrations to ensure redundancy
* `Integrate only fields and systems that support defined business outcomes`
* Disable metadata normalization to simplify mappings
* Enable ingestion for every available CMDB attribute

> During implementation, you realize that devices are missing owner and application environment tags. What is the best first step to improve metadata quality?
* `Audit existing CMDB and LogicMonitor properties to identify missing fields.`
* Rebuild the correlation models using default templates.
* Delete and recreate all resource tags from scratch.
* Increase the frequency of Edwin AI’s ingestion schedule.

> Priya created several new rules for different data sources but now notices performance delays. What adjustment should she make to improve efficiency?
* Disable all interactive rules to reduce processing.
* `Consolidate overlapping rules into a smaller number of well-scoped rules.`
* Edit the default rules to include new filters.
* Increase the number of action groups linked to each rule.

> During a network issue, LM Envision identifies the affected devices and alerts the team. Edwin AI immediately analyzes the event, identifies the cause, and recommends a remediation playbook. What capability allows Edwin AI to go beyond LM Envision’s monitoring to deliver these automated recommendations?
* Manual configuration of static response workflows
* `Generative and unsupervised AI that enables conversational insights and autonomous remediation`
* Traditional machine learning requiring labeled datasets
* A preloaded library of manual troubleshooting checklists

> Which statement best describes an Insight in Edwin AI?
* A dashboard used to monitor AI agent activity.
* A temporary placeholder for alerts before they enter the rules engine.
* `A correlated group of related alerts that provide actionable context.`
* A visualization of performance metrics in a chart.

> Which of the following technologies is unique to Edwin AI and not part of the traditional AI in LM Envision?
* Dynamic thresholds
* Forecasting
* Anomaly detection
* `AI Agent`

> You log in to Edwin AI and notice that you cannot see the “Models” or “Actions” pages in the navigation panel. What is the most likely reason?
* Your portal has exceeded its dashboard limit
* The Edwin AI service is temporarily offline
* `Your user permissions do not include “Manage” access`
* The pages have been removed in a recent update

> Which best practice ensures that modifications to Edwin AI models remain auditable and do not disrupt existing operations?
* Edit active models directly in the production environment
* Delete outdated models without archiving them
* `Clone existing models before making adjustments`
* Use temporary models for experimentation

> During quarterly calibration, a monitoring lead notices that one model generates too few insights while another creates excessive noise. Which governance action aligns best with Edwin AI best practices? (Select two)
* `Refine or retire models with poor performance`
* Delete underperforming models to improve system efficiency
* `Verify ITSM mappings remain accurate`
* Adjust alert thresholds across every model equally to achieve balance in output volume

> Your team wants Edwin AI to automatically open incidents in ServiceNow when critical alerts occur. Which feature combination should you configure?
* `Rules linked to action groups that trigger ServiceNow incident creation`
* Agent permissions for incident-level access
* Insights filters applied to dashboards
* Metadata enrichment fields for critical events

> You’re preparing to make extensive configuration updates to Edwin AI rules and actions. What should you do first? (Select 2)
* Manually copy each rule and action to a spreadsheet for safekeeping
* Import new templates to overwrite your existing configurations
* `Archive all running models before starting the configuration updates`
* `Export a backup file of current configurations so they can be restored if needed`

> Which best practice helps maintain consistent automation performance over time? (Select 3)
* Add catch-all actions only when rules fail completely
* `Monitor configurations regularly`
* `Verify escalations, and updating configurations`
* `Review rules regularly`

> An operations engineer increases the minimum cluster density from 2 to 5 in an Edwin AI model. What is the most likely outcome of this change?
* The model will include unrelated alerts because the overlap requirement is lower
* `The model will form fewer clusters because more alerts must match before one is created`
* The model will form more clusters because alerts will be correlated faster
* The model will process alerts individually because timeouts are disabled

> A company is tracking the impact of Edwin AI on team efficiency. Which of the following results best reflects the intended value of the platform?
* All troubleshooting is deferred to third-party consultants
* Senior team members submit more support tickets than before
* Engineers spend more time reviewing archived logs
* `L1 team members can now troubleshoot faster thereby reducing the overall noise and address backlog issues faster`

> Why is it important to maintain consistent metadata naming conventions (e.g., “London” vs. “LDN”)?
* It ensures alerts are color-coded correctly in dashboards
* `Inconsistent names reduce Edwin AI’s ability to correlate and enrich alerts accurately`
* It enables faster ingestion speeds for new devices
* It increases the size of metadata storage requirements

> A user reports that their dashboard is showing no data. As an Edwin AI administrator, what should you check first?
* The API credentials on the Settings page
* The AI Agent configuration
* `The dashboard filters and time range settings`
* The system log archive for export errors

> In Edwin AI, what determines which dashboard appears as your homepage?
* The Insights Dashboard, which is permanently set as the homepage
* The Executive Dashboard assigned by your administrator
* The most recently created dashboard in your account
* `The dashboard you have marked as your favorite`

> Which of the following are best practices when prompting the AI agent? (Select 3)
* Ask multiple unrelated questions at once to save time
* `Be clear and specific in your question`
* `Review AI responses and sources before acting`
* `Provide Insight or CI names for context`

> Which of the following best describes what models do in Edwin AI?
* Models generate dashboards for monitoring performance.
* Models automate incident creation in ServiceNow.
* `Models use correlations and machine learning to group related alerts into insights.`
* Models determine user permissions and access levels.

> What is the purpose of mapped fields within an action?
* They enable action sequencing.
* `They control how data values transfer from source to target records.`
* They identify which rule is linked to the action.
* They determine if a rule runs automatically.

> A company’s DevOps team is receiving duplicate incidents for the same alert in ServiceNow. As the Edwin AI administrator, what should you check first?
* `Whether multiple automatic rules are targeting the same datasource.`
* If the alerts contain a mapped field for “duplicate.”
* If the rules are set to “interactive.”
* If users have Manage-level access.
