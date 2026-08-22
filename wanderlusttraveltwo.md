# Case 3 : Wanderlust Travel

## Solution to Wanderlust Travel Problem Framing, Ideation & Validation + Metrics: Building a Metrics Dashboard for Wanderlust Travel

The dashboard specifically needs to cover **KPIs,** **User Engagement,** **Revenue,** **and** **Operational Metrics.**

Below is how I would solve the case in a **PM Interview.**

**1. Executive Recommendation:**

I would **not create a dashboard with 30-40 disconnected metrics.**

Instead, I would build a **Search Metrics Tree:**

**Business Outcome → Search Success → User Funnel → Revenue → Operational Health**

**Recommended North Star Metric**

**Search-to-Booking Conversion Rate**

**Completed bookings from search / Search sessions × 100**

Why?

Because Wanderlust's Search team exists to help users find relevant travel options and ultimately contribute to bookings. Search-to-book conversion therefore connects **user intent + search experience + business outcome.**

This is also consistent with travel analytics approaches that connect search/referral activity to conversions and bookings.

**Metric Tree**

<img width="500" height="300" alt="case_3_img_1" src="https://github.com/user-attachments/assets/aca143fb-f52f-45ce-a8bf-87493a527b26" />

**2. Dashboard Structure:**

I recommend **5 Excel Sheets.**

| Sheet                      | Purpose                          |
| -------------------------- | -------------------------------- |
| **1. Executive Dashboard** | Overall health + key KPIs        |
| **2. Search Funnel**       | Identify where users drop        |
| **3. User Engagement**     | Understand user behaviour        |
| **4. Revenue**             | Connect search to business value |
| **5. Operations**          | Monitor search infrastructure    |

This structure directly addresses the case's problem of scattered information and enables faster, data-driven decisions.

i **Sheet 1 - Executive Dashboard:**

The Product Lead should be able to open the Excel file and understand the situation in **30 Seconds**.

**Top KPI Cards**

| KPI                         | Definition                                         | Why It Matters                           |
| --------------------------- | -------------------------------------------------- | ---------------------------------------- |
| **Search-to-Booking CVR** ⭐ | Bookings / Search sessions                         | Primary business outcome                 |
| Search Success Rate         | Searches returning usable results / Total searches | Measures whether search satisfies intent |
| Result CTR                  | Result clicks / Searches with results              | Measures result attractiveness           |
| Product View Rate           | Product views / Search sessions                    | Measures progression                     |
| Booking Initiation Rate     | Booking starts / Product views                     | Measures purchase intent                 |
| Booking Completion Rate     | Completed bookings / Booking starts                | Measures checkout success                |
| Revenue from Search         | Revenue generated from search-originated bookings  | Business impact                          |
| Revenue/Search              | Search-attributed revenue / Search sessions        | Monetization efficiency                  |
| Zero-result Rate            | Zero-result searches / Total searches              | Search quality problem                   |
| Search Error Rate           | Failed searches / Total searches                   | Technical health                         |
| P95 Search Latency          | 95th percentile search response time               | Performance                              |
| DAU/WAU Search Users        | Unique users searching                             | Engagement                               |

For travel funnels, product views, booking initiation and completed bookings are useful stages for locating conversion problems.

ii **Sheet 2 - Search Funnel:**

This should be the **most important diagnostic sheet.**

**Funnel**

<img width="251" height="348" alt="case_3_img_2" src="https://github.com/user-attachments/assets/adcee799-833a-4777-aa62-5bd06d2d7c67" />

**Metrics**

| Funnel Stage | Metric                  | Formula                              |
| ------------ | ----------------------- | ------------------------------------ |
| Search       | Search Sessions         | Count of search sessions             |
| Results      | Search Success Rate     | Searches with results / Searches     |
| Results      | Zero-result Rate        | Zero-result searches / Searches      |
| Results      | Result CTR              | Result clicks / Searches             |
| Product      | Product View Rate       | Product views / Searches             |
| Booking      | Booking Initiation Rate | Booking starts / Product views       |
| Payment      | Payment Completion Rate | Successful payments / Payment starts |
| Final        | Search-to-Book CVR      | Bookings / Search sessions           |

**Example**

Suppose:

- 100,000 searches
- 90,000 receive results
- 45,000 users click results
- 20,000 view product details
- 8,000 start booking
- 5,000 complete booking

Then:

**Search Success Rate**

= 90,000 / 100,000
= **90%**

**Result CTR**

= 45,000 / 90,000
= **50%**

**Product View Rate**

= 20,000 / 100,000
= **20%**

**Booking Initiation Rate**

= 8,000 / 20,000
= **40%**

**Search-to-Book Conversion**

= 5,000 / 100,000
= **5%**

These numbers are **illustrative only**, not Wanderlust's actual performance.

iii **Sheet 3 - User Engagement Metrics:**

The case explicitly says that understanding user behaviour can help the Search team personalize the experience and improve engagement.

I would divide engagement into four areas.

**A. Search Adoption**

| Metric          | Definition                     |
| --------------- | ------------------------------ |
| Search Users    | Unique users performing search |
| Searches/User   | Total searches / Search users  |
| Search Sessions | Sessions containing search     |
| Search Adoption | Users searching / Active users |

**B. Search Behaviour**

| Metric                 | What It Tells Us                       |
| ---------------------- | -------------------------------------- |
| Searches per Session   | Search intensity                       |
| Query Refinement Rate  | How often users modify searches        |
| Filter Usage Rate      | Whether filters are useful             |
| Sort Usage Rate        | Whether users need alternative ranking |
| Repeat Search Rate     | Whether users keep looking             |
| Average Results Viewed | Depth of exploration                   |
| Time to First Click    | Search decision speed                  |

**C. Search Quality**

| Metric                   | What It Tells Us                  |
| ------------------------ | --------------------------------- |
| Zero-result Rate         | Missing inventory / poor matching |
| Result CTR               | Relevance/attractiveness          |
| Search Abandonment       | Users leaving without engaging    |
| Query Reformulation Rate | Possible poor relevance           |
| No-click Rate            | Users don't find results useful   |

**D. Retention**

| Metric                 | Definition                             |
| ---------------------- | -------------------------------------- |
| Returning Search Users | Users who search again                 |
| Search Retention       | Users returning to search after X days |
| Repeat Booking Rate    | Returning customers who book again     |

**Very Important: Segment the Metrics**

A dashboard without segmentation can hide major problems.

I would make these **global Excel filters**:

**User**
- New vs Existing
- Logged-in vs Guest
- High-frequency vs Low-frequency

**Platform**
- Android
- iOS
- Web

**Travel Type**
- Flight
- Hotel
- Vacation package

**Geography**
- Country
- Region
- Origin
- Destination

**Search Characteristics**
- Domestic vs International
- One-way vs Round-trip
- Short vs Long lead time
- Popular vs long-tail destination

**Date**
- Day
- Week
- Month

Travel analytics platforms similarly use dimensions such as geography, routes, device, travel dates and travel type to diagnose performance.

iv. **Sheet 4 - Revenue Metrics:**

The case specifically identifies revenue generation as an important component of Search metrics.

The key principle:

**Don't just measure how many people search. Measure how effectively search creates economic value.**

**Core Revenue Metrics**

| Metric                           | Formula                                       |
| -------------------------------- | --------------------------------------------- |
| **Search-attributed Revenue**    | Revenue from search-originated bookings       |
| **Revenue/Search**               | Search revenue / Search sessions              |
| **Booking Value**                | Total booking value                           |
| **Average Booking Value**        | Booking value / Number of bookings            |
| **Search-to-Revenue Conversion** | Revenue-generating bookings / Search sessions |
| **Revenue per User**             | Search revenue / Search users                 |
| **Cancellation Rate**            | Cancelled bookings / Completed bookings       |
| **Refund Rate**                  | Refunded bookings / Completed bookings        |

**Revenue Diagnostic Tree**

<img width="250" height="250" alt="case_3_img_3" src="https://github.com/user-attachments/assets/30a68618-49e3-4f18-b9fe-3226142197b8" />

This helps answer:

"Revenue declined — did fewer users book, or did users book cheaper products?"

That's much more actionable than simply showing "Revenue ↓".

v. **Sheet 5 - Operational Metrics:**

The case specifically says Search infrastructure stability and performance must be monitored.

I would track:

| Metric                         | Purpose                          |
| ------------------------------ | -------------------------------- |
| **Search Latency P50**         | Typical response time            |
| **Search Latency P95**         | Slow-user experience             |
| **Search Latency P99**         | Extreme latency                  |
| **Search Error Rate**          | Failed searches                  |
| **API Error Rate**             | Backend failures                 |
| **Timeout Rate**               | Search requests timing out       |
| **Search Availability**        | System uptime                    |
| **Result Freshness**           | How current inventory/prices are |
| **Inventory Availability**     | Searchable inventory health      |
| **Data Pipeline Failure Rate** | Data quality                     |
| **Crash Rate**                 | App stability                    |
| **Incident Count**             | Operational reliability          |

**Why P95 instead of only average latency?**

Because an average can hide a bad tail.

Example:

Average latency = 1.2 sec
P95 latency     = 5.8 sec

The average looks healthy, but 5% of users may be experiencing a very slow search.
