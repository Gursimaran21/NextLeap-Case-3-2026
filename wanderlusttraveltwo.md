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
