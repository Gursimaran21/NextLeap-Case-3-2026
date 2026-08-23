# Case 3 : Wanderlust Travel

## Solution to Wanderlust Travel Problem Framing, Ideation & Validation + Metrics: Building a Metrics Dashboard for Wanderlust Travel

**1. The Most Important Metric Tree:**

For the case submission, I would show this diagram.

<img width="522" height="673" alt="case_3_img_5" src="https://github.com/user-attachments/assets/e39b8ed8-f59c-4212-85f4-b90f8006ac09" />

**2. How I Would Prioritize Metrics:**

The case gives Prerana only **one week** to create the Excel prototype.

Therefore, I would use an **MVP dashboard** rather than trying to build everything.

**Tier 1 - Must Have**

**1.** Search-to-Booking Conversion

**2.** Search Success Rate

**3.** Zero-result Rate

**4.** Result CTR

**5.** Product View Rate

**6.** Booking Initiation Rate

**7.** Booking Completion Rate

**8.** Search-attributed Revenue

**9.** Revenue/Search

**10.** Search Volume

**11.** Search Error Rate

**12.** P95 Search Latency

**Tier 2 - Diagnostic**

- Searches/User
- Search abandonment
- Query refinement
- Filter usage
- Sort usage
- Average results viewed
- Cancellation
- Refunds
- P50/P99 latency
- API failures

**Tier 3 - Advanced**

- Personalization lift
- Search relevance score
- Destination-level demand
- Price competitiveness
- Recommendation performance
- Cohort retention
- Experiment impact

**3. Excel Dashboard Layout:**

I would make the first Excel tab look approximately like this:

<img width="575" height="720" alt="case_3_img_6" src="https://github.com/user-attachments/assets/f8202776-576a-4100-b420-1f0251f02953" />

**4. Add Traffic-Light Status:**

This makes the Excel prototype much more useful for a Product Lead.

| Metric             | Current | Target | Status |
| ------------------ | ------: | -----: | ------ |
| Search-to-Book CVR |    4.8% |   5.0% | 🟡     |
| Search Success     |     91% |    95% | 🟡     |
| Zero-result Rate   |      8% |    <5% | 🔴     |
| Result CTR         |     53% |    50% | 🟢     |
| Search Error Rate  |    0.8% |    <1% | 🟢     |
| P95 Latency        | 2.8 sec | <3 sec | 🟢     |

**Important:** these target values are illustrative. The case provides no actual Wanderlust benchmarks, so I would not present them as company facts.

**5. Add Trend Analysis:**

Every major metric should show:

**Current value + Previous period + % change + trend**

Example:

| KPI            | Current | Previous | Change |
| -------------- | ------: | -------: | -----: |
| Searches       |    100K |      92K |  +8.7% |
| Search Success |     91% |      94% |  -3.0% |
| Result CTR     |     53% |      51% |  +3.9% |
| Booking CVR    |    4.8% |     4.5% |  +6.7% |
| Revenue        |      ₹X |       ₹Y |   +12% |

This makes the dashboard answer:

**"What changed?"**

rather than simply:

"What is the number?"

**6. Add an Insight Section:**

This is where you can demonstrate **Product Manager thinking**, rather than just analytics.

At the bottom of the dashboard:

**7. Key Insights:**

**1. Search volume increased, but search success declined.**

→ Investigate inventory coverage / search relevance.

**2. Result CTR improved but booking conversion declined.**

→ Investigate product detail page, pricing or checkout friction.

**3. Zero-result searches increased significantly.**

→ Investigate destination coverage, spelling/synonym handling and inventory.

**4. Search latency increased while abandonment increased.**

→ Investigate infrastructure performance.

This follows the principle of using funnel stages to identify where users are being lost and then drilling into the corresponding experience problem.

**8. Example Product Decisions From the Dashboard:**

This is an excellent section to include in your case presentation.

| Dashboard Signal     | Possible Problem      | Product Action             |
| -------------------- | --------------------- | -------------------------- |
| Zero-result ↑        | Poor search coverage  | Improve matching/inventory |
| Result CTR ↓         | Poor relevance        | Improve ranking            |
| Searches/session ↑   | Users struggling      | Improve discovery          |
| Filter usage ↑       | Users need refinement | Improve filters            |
| Product views ↓      | Poor results          | Improve ranking/content    |
| Booking initiation ↓ | Low purchase intent   | Improve pricing/UX         |
| Payment completion ↓ | Checkout friction     | Simplify payment           |
| Latency ↑            | Infrastructure issue  | Optimize search API        |
| Error rate ↑         | Technical instability | Investigate backend        |
| Revenue/search ↓     | Monetization issue    | Improve ranking/value mix  |

**9. What Makes This Dashboard Strategically Valuable?**

The case identifies four reasons for building the dashboard:

**1. Data-driven decision-making**

Instead of manually collecting data from different systems, the team gets one source of truth.

**2. Competitive advantage**

The team can identify search problems faster and respond to changing customer behaviour.

**3. Customer expectations**

Behavioural and search-quality metrics help identify pain points and opportunities for personalization.

**4. Resource allocation**

The dashboard helps determine which problems deserve engineering/product investment.

So the dashboard should ultimately answer **four Product Lead questions:**

<img width="445" height="202" alt="case_3_img_7" src="https://github.com/user-attachments/assets/cf22bee7-1ceb-4c41-a70f-3bf29e47cd8c" />

**10. Final Recommended Dashboard Hierarchy**

For the presentation, I would summarize the entire solution as:

**LEVEL 1 - Business Outcome**

**Search-attributed Revenue**

↓

**LEVEL 2 - Primary Search KPI**

**Search-to-Booking Conversion Rate**

↓

**LEVEL 3 - Funnel Drivers**

**Search Success → Result CTR → Product View → Booking Start → Booking Completion**

↓

**LEVEL 4 - Diagnostic Metrics**

**Zero-result → Refinement → Filters → Abandonment → Relevance**

↓

**LEVEL 5 - System Health**

**Latency → Errors → Availability → Data Freshness**

This prevents the dashboard from becoming a "metric dump."

**11. My Final MVP - 12 Metrics:**

If your Product Lead says:

**"Prerana, you only have space for 12 metrics. What would you choose?"**

I would answer:

|   # | Metric                           | Category       |
| --: | -------------------------------- | -------------- |
| ⭐ 1 | **Search-to-Booking Conversion** | KPI            |
|   2 | Search Volume                    | Engagement     |
|   3 | Search Success Rate              | Search Quality |
|   4 | Zero-result Rate                 | Search Quality |
|   5 | Result CTR                       | Engagement     |
|   6 | Product View Rate                | Engagement     |
|   7 | Booking Initiation Rate          | Conversion     |
|   8 | Booking Completion Rate          | Conversion     |
|   9 | Search-attributed Revenue        | Revenue        |
|  10 | Revenue/Search                   | Revenue        |
|  11 | Search Error Rate                | Operations     |
|  12 | P95 Search Latency               | Operations     |

**Why these 12?**

Because together they answer:

**Are people searching? → Are they finding useful results? → Are they engaging? → Are they booking? → Is Search generating revenue? → Is the system healthy?**

**12. Conclusion:**

**I would build Wanderlust Travel's Search Metrics Dashboard around Search-to-Booking Conversion as the primary outcome metric, supported by a funnel of Search Success, Result CTR, Product Views, Booking Initiation and Booking Completion. Revenue metrics such as Search-attributed Revenue and Revenue per Search would connect Search performance to business growth, while Zero-result Rate, Search Error Rate and P95 Search Latency would act as diagnostic indicators.**

**The dashboard would be segmented by platform, geography, travel product, user type and search characteristics so the team can identify where performance gaps originate. The Excel MVP would contain an Executive Dashboard, Search Funnel, User Engagement, Revenue and Operational Health views, with current performance, previous-period comparison, trends and traffic-light status.**

**This approach converts fragmented data into an actionable decision system: the team can identify what changed, understand why it changed, prioritize the highest-impact problems and allocate resources accordingly.**

That directly addresses the case's central challenge: moving Wanderlust's Search team from **manual, fragmented analysis to faster, data-driven product decisions.**

## Go back to [README](README.md)
