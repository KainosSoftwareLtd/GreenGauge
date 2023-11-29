# Measurement maturity

This pillar of the maturity model covers ....

* [Collecting data](#Collecting-data)
* [Applying standards](#Applying-standards)
* [Carbon proxies](#Carbon-proxies)
* [KPIs](#KPIs)
* [Benchmarking yourself](#Benchmarking-yourself)

### Collecting data
It's important that you can collect the data that allows you to understand and evaluate the environmental impact of your software. Analysing this data over time allows you to use historical data to support the need for any future changes or improvements.

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Full lifecycle collection** | The data required to understand the carbon impact of building, Developing, Operating and Usage the software. Do you collect all of this data today? | Some information is collected or derived from other sources on an ad-hoc basis. | Some areas are quite mature though others may be lacking e.g. we may have lots of data around build/deployment but little around usage. | Mature data collection across all areas to understand the full lifecycle. |
| **Storage** | All this data needs to be stored somewhere, do you have a mechanism for this? | Theres no real policy around this. data is not centralised | Some data is centralised onto corporate systems, but stored in different formats. | Data is collected within centrally managed corporate systems that can be easily accessed. |
| **Visualisation** | How easily can you access and analyse the data to create visualisations? | Ad-hoc visualisations/carbon equivalencies are created with something like Excel spreadsheets instead of specialised visualisation tools. | Some dashboards created using point-in-time data. | Dashboards exist and make use of near real-time data. |

### Applying Standards
Once you have collected the data, it is important to apply industry standards and techniques to create a common language for your reporting. For example, adopting recognised standards like the Software Carbon Intensity(SCI) Specification creates a repeatable, scalable and predictable way of calculating the carbon impact of software. 

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **GHG** | Applying the Green House Gas(GHG) Protocol to how your categorised your impact across 3 scopes:<ol><li>Direct emissions</li><li>Indirect emissions from, for example, the electricity supply</li><li>Supply chain emissions</li></ol> | We are unaware of the scopes or significance | We have measured Scope 1 and 2 emissions and are actively seeking to reduce impacts. | We have measured Scope 1, 2 and 3 emissions and are actively seeking to reduce impacts including through your supply chain. |
| **SCI** | Measuring the environmental impact of your software using the Software Carbon Intensity(SCI) speification. The more efficient your code, lower your impact for a given unit of value. | We are unaware of software carbon intensity specification or yet to apply it. | We have completed a point-in-time calculation for SCI for a given service. | We regularly calculate our SCI for a given service and use this to identify improvements/support decision-making. |
| **FinOps** | Applying the FinOps foundation framework to optimise cloud resource utilisation and reduce costs | We apply optimisations on an ad-hoc basis whenever its felt the bill is becoming too expensive. | We have completed an assessment with an action plan in place/being progressed to address findings. | In addition to assessments, we focus on making sure that decision-making happens as early as possible in the process. |

### Carbon proxies
Sometimes you won't have the data because it might not exist or can't get access to it. Use of carbon proxies can help to plug these gaps with equivalencies. Equivalencies work on the basis that you can make assumptions about one metric relative to another e.g. some key carbon proxies regarding cloud computing include cost and utilisation. As you spend more money or less or tweak resource utilisation to eliminiate waste, your carbon impact will closely follow. Hence the carbon proxy.

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Resource Utilisation** | For each component (or combination of them within your solution) how well can you track information related to your consumption of them e.g. Cost, Utilisation, Storage size, Data Transfer volumes etc. | For each service you track/optimise costs and look at capacity planning for future growth around utilisation/storage/data transfer. | We have identified some key metrics as carbon proxies e.g. cost as a measure of CO<sub>2</sub>e. We use these proxies to support decision making as required. | We have identified several carbon proxies which are regularly tracked as part of our reporting and are used to influence decision making. |
| **Service Delivery** | From the perspective of the service consumer there are tools that can help you identify what improvements can be made. For example there are website scanners that can provide feedback on page weight, server response times and similar. | We track request response times and some other basic metrics. Most of the information collection is server-side. | We make use of real-user-monitoring or application performance management solutions providing detailed information on client-side telemetry. This lets us understand carbon proxies from the perspective of our users. | We make use of real-user-monitoring or application performance management solutions providing detailed information on client-side telemetry. This lets us understand carbon proxies from the perspective of our users and these insights influence our decision making. |

### KPIs
Defining and tracking Key Performance Indicators(KPI) aligned to your green software ambitions creates accountability and demonstrates the importance of regular measurement for real-time tracking. Doing this provides clear feedback loops and the possibility for organisations to offer incentives based on what is going well, offer corrections where it isn't.
            
| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Tracking** | If you aren't setting Green Software KPIs against current initiatives then benefit tracking is moot - you don't know |  We don't set Green Software goals or targets that we track as KPIs. | We do have Green Software KPIs but tracking can be ad-hoc. | We set Green Software KPIs with the same level of rigour/governance as other service KPI's. We can link attainment of the KPIs against value derived. |
| **Trend Analysis** | Are you analysing KPI changes over time to identify trends, and then changing processes based on what is working and isn't? | We don't track a lot of metrics so the impact of this is unknown. | We look at trends periodically based on available data and may change things adjust our path. | We regularly look at trends to build on what is working, and course correct what is not. We share this information across the organisation as part of lessons learnt. |
| **Incentives** | How do you encourage people to engage with setting/tracking KPI's? Tracking another KPI which can be rather abstract is unlikely to be appealing by itself. | We don't provide many incentives to set or track green software KPIs. | We provide some incentives to set or track green software KPIs but they can be de-prioritised in favour of other, more important KPI's. | We incentivise, elevate and prioritise Green Software KPI's as a primary concern. |

### Benchmarking yourself
What does "good" look like both within your organisation and relative to other organisations which are similar to yours? How do you establish a benchmark of good so you know if your ambitions are rooted in reality? For example, have you established an internal leaderboard against your green software KPIs?  

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Internally** | Internal benchmarking can be a useful way to create competition between staff/teams/groups and provide a gamified incentive around green software. | We don't really do this today and what happens is largely informal. | We share success stories and learnings alongside the benefits realised. This happens occasionally when teams have a good story to tell. | We share success stories and learnings alongside the benefits realised. This happens consistently and regularly with teams encouraged to share. |
| **Externally** | External benchmarking can be a way for you to learn from others in Industry/community/Competitors/government on how to be better. | We don't really do this today. | We look to compare ourselves to similar organisations via use of publicly available tools. | We actively compare ourselves to similar organisations via use of publicly available tools and share our progress externally on successes we've had to inspire others. |