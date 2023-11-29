# Measurement maturity

This pillar of the maturity model covers ....

* [Data](#Data)
* [Standards](#Standards)
* [Carbon proxies](#Carbon-proxies)
* [KPIs](#KPIs)
* [Benchmarking](#Benchmarking)


### Data
It's important that you can collect the data that allows you to understand and evaluate the environmental impact of your software. Analysing this data over time allows you to use the historical data to support the need for any future changes or improvements.

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Full lifecycle** | The data required to understand the carbon impact of building, Developing, Operating and Usage the software. Do you collect all of this data today? | Some information is collected or derived from other sources on an ad-hoc basis. | Some areas are quite mature though others may be lacking e.g. we may have lots of data around build/deployment but little around usage. | Mature data collection across all areas to understand the full lifecycle. |
| **Delivery** | The impact of creating the software in the first place, can you reason about cost of creation? | Whilst the data does exist, it can only be obtained on an adhoc basis. | Data exists on centralised systems and can be extracted in reports. | Data exists on centralised systems and can be integrated for real-time analysis. |
| **Storage** | All this data needs to be stored somewhere, do you have a mechanism for this? | Not centralised | Some data is centralised onto corporate systems, but stored in different formats. | Data is collected within centrally managed corporate systems that can be easily accessed via reports and programmatically. |
| **Visualisation** | How easily can you access and analyse the data to create visualisations? | Ad-hoc visualisations/carbon equivalencies are created with something like Excel spreadsheets instead of specialised visualisation tools. | Some dashboards created using point-in-time data. | Dashboards exist and make use of near real-time data. |

### Standards
Once you have collected the data, it is important to apply industry techniques and standards to allow collaboration and create a common language for your reporting. Adopting recognised standards like the Software Carbon Intensity Specification, creates a repeatable, scalable and predictable way of calculating the carbon impact of software. 

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **GHG** | GreenHouse Gas ProtocolThe GHG Protocol has 3 scopes:<ol><li>Direct emissions</li><li>Indirect emissions from, for example, the electricity supply</li><li>Supply chain emissions</li></ol> | We are unaware of the scopes or significance | We have measured Scope 1 and 2 emissions and are actively seeking to reduce impacts. | We have measured Scope 1, 2 and 3 emissions and are actively seeking to reduce impacts including through your supply chain. |
| **SCI** | Software Carbon Intensity(SCI) is a way to measure your rate of emissions. The more efficient your code is the lower your score will be. | We are unaware of software carbon intensity specification or yet to apply it. | We have completed a point-in-time calculation for SCI for a given service. | We regularly calculate our SCI for a given service and use this to identify improvements/support decision-making. |
| **FinOps** | The FinOps Foundation | We apply optimisations on an ad-hoc basis whenever its felt the bill is becoming too expensive. | We have completed an assessment with an action plan in place/being progressed to address findings. | In addition to assessments, we focus on making sure that decision-making happens as early as possible in the process. |

### Carbon proxies
Sometimes you won't have the data, it doesn't exist or can't get access to it. Using carbon proxies can help to plug these gaps with equivalencies. Equivalencies work on the basis that you can make assumptions about one metric relative to the thing that you wish to track e.g. some key carbon proxies regarding cloud computing include cost and utilisation. As you spend more or less money with your cloud provider or as capacity within your solution is wasted,  your carbon impact will follow closely.  

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Resource perspective** | For each component (or combination of them within your solution) how well can you track information related to your consumption of them e.g. Cost, Utilisation, Storage size, Data Transfer volumes etc. | For each service you track/optimise costs and look at capacity planning for future growth around utilisation/storage/data transfer. | We have identified some key metrics as carbon proxies e.g. cost as a measure of CO<sub>2</sub>e. We use these proxies to support decision making as required. | We have identified several carbon proxies which are regularly tracked as part of our reporting and are used to influence decision making. |
| **Consumer perspective** | From the perspective of the service consumer there are tools that can help you identify what improvements can be made. For example there are website scanners that can provide feedback on page weight, server response times and similar. | We track request response times and some other basic metrics. Most of the information collection is server-side. | We make use of real-user-monitoring or application performance management solutions providing detailed information on client-side telemetry. This lets us understand carbon proxies from the perspective of our users. | We make use of real-user-monitoring or application performance management solutions providing detailed information on client-side telemetry. This lets us understand carbon proxies from the perspective of our users and these insights influence our decision making. |

### KPIs
Defining and tracking Key Performance Indicators (KPI) aligned to your green software ambitions creates accountability and demonstrates the importance of measurement, tracking and impact. Doing this provides clear feedback loops and the possibility for incentives based on what is going right, and what is not.
            
| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Tracking** | If you aren't setting Green Software KPIs against current initiatives then how do you articulate the importance of them and track the benefits gained from them? |  We do not set Green Software KPIs. | We set Green Software KPIs but tracking can be ad-hoc. | We set Green Software KPIs with the same level of rigour/governance as other service KPI's. |
| **Trend Analysis** | Are you analysing changes to identify trends, and then changing processes based on what is working and is not. | We don't track a lot of metrics so the impact of this is unknown. | We update the impact of changes periodically based on available data. | We regularly update the impact of change and align it to reporting for other KPIs for the service. |
| **Incentives** | How do you encourage people to engage with the process? Tracking another KPI which can be somewhat abstract may not be appealing by itself. | We don't provide many incentives to set or track green software KPIs. | We provide few incentives to set or track green software KPIs. They are not seen as important as other KPI's so tend to be de-prioritised. | We prioritise Green Software KPIs similarly to other KPIs |

### Benchmarking
What does "good" look like both within your organisation and relative to other organisations which are similar to yours? How do you establish a benchmark of good so you know if your ambitions are rooted in reality? For example, have you established an internal leaderboard against your green software KPIs?  

| Measure | Description | Score: 1 | Score: 3 | Score: 5 |
| --- | --- | --- | --- | --- |
| **Internally** | Internal benchmarking can be a useful way to create competition between your staff and an incentive for your staff to engage with green software. | We don't really do this today and what happens is largely informal. | We share success stories and learnings alongside the benefits realised. This happens occasionally when teams have a good story to tell. | We share success stories and learnings alongside the benefits realised. This happens consistently and regularly with teams encouraged to share. |
| **Externally** | External benchmarking can be a way for you to learn from others in Industry/community/Competitors/government on how to be better. | We don't really do this today. | We look to compare ourselves to similar organisations via use of publicly available tools. | We actively compare ourselves to similar organisations via use of publicly available tools and share our progress externally on successes we've had. |