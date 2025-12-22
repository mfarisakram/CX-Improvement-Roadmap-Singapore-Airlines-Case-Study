# Project Title: CX Improvement Roadmap (Singapore Airlines Case Study)

# 1. Introduction
Aviation and travel are my greatest passions. I view the entire passenger journey as a series of crucial touchpoints: from ticket purchase and airport arrival to the check-in process, the comfort of the in-flight seat and meal, and the overall onboard services. I always aim for seamless service and expect a high level of comfort, especially when paying a premium for the experience. However, particularly on long-haul flights, a consistently excellent experience is not always guaranteed.

# 2. Case Scenario
As a Junior Data Analyst within the Customer Experience (CX) department at Singapore Airlines, my primary role is to listen to what our passengers are saying. We take immense pride in our world-class service, but actively using feedback is the only way to stay ahead. Recently, we observed a subtle shift in the nature of customer comments, leading to a new task for me: understand exactly what happened in our review data over the last year.

My manager approached me with a specific concern. While we generally maintain high ratings, we urgently needed to pinpoint specific customer pain points to improve our 2024 strategy. The request was clear and simple: identify the top three categories of complaints for 2023.

To ensure these figures had meaningful context, I was also asked to compare them with our 2022 data. This comparison is vital, as it allows us to establish a pattern and determine whether an issue is a new, immediate concern or an underlying problem that has been happening for a long time.

# 3. Data Source
I would like to thank fellow Kaggler, Kanchana1990, for making the Singapore Airlines Reviews dataset available. For this case study, I performed the analysis using two full years of customer review data, specifically covering the period from 2022 through to the end of 2023. This two-year scope was essential for establishing clear patterns and trends in passenger complaints before diving into the specific pain points identified in the most recent year.

# 4. Main Goal
The primary objective of this analysis was to:

 1) Identify the top 3 categories of complaints in 2023.

 2) Compare these numbers with 2022 to spot trends.

 3) Provide clear evidence so the management team can allocate resources to fix these specific issues.

# 5. Data Preparation Process
My analysis began with a large initial dataset containing approximately 10,000 customer reviews from 2018 to March 2024. For this project, I filtered this data to focus exclusively on the 2022 and 2023 records, as these are the two most recent, complete years. Given the resulting dataset size, Microsoft Excel was the most appropriate tool for cleaning, summarising, and analysing the data.

The processing was executed in the following steps:

**A.** Data Cleaning and Transformation I first ensured data quality by checking the filtered tables to confirm there were no null values in the primary analytical columns (e.g., date and review text). I then transformed the raw datetime column into separate 'Year' and 'Month' columns. This transformation was critical for conducting the subsequent yearly comparison and monthly trend analysis.

**B.** Complaint Theme Categorisation The review column, which contains free-text customer feedback, required careful thematic categorisation. I established ten distinct complaint themes, such as "In-flight meal", "Seat/legroom issue", and "Luggage issue".

To systematically tag each review, I used a series of Excel functions including ```IF```, ```AND```, and ```OR``` combined with the ```ISNUMBER(SEARCH())``` logic. This approach allowed me to assign a '1' to a review row if it contained specific sets of keywords relevant to a theme, and '0' otherwise.

For example, to identify a "Luggage Issue", the function checked for a primary keyword (e.g., "luggage", "bag") AND a secondary keyword related to the failure (e.g., "lost", "damaged"). By applying this logic across all ten themes, I effectively converted the qualitative text data into quantitative data for analysis.

# 6. Key Findings
When comparing 2022 to 2023, the data tells an interesting story.

Total Volume: Some complaints are actually decreasing. For example, complaints about Flight Cancellation/Delay dropped from 93 in 2022 to 73 in 2023. This is a positive sign that our operations are stabilising.

**The Shift:** However, complaints about the physical experience inside the plane are increasing.

**The Top 3:** The most frequent complaints in 2023 were about Seats, Meals, and Service.

#### Analysis of Top Issues (2023)
**1. Seat and Legroom Issues (107 complaints)**

The Trend: In 2022, we had 67 complaints about this. In 2023, it jumped to 107.

The Insight: This is a massive increase. Since this number nearly doubled, it suggests that as our flights became fuller post-pandemic, passengers became much more sensitive to personal space and seat comfort.

**2. In-flight Meal (88 complaints)**

The Trend: This rose from 70 complaints in 2022 to 88 in 2023.

The Insight: While not as steep a rise as the seat issues, it is still an upward trend. Passengers are likely unhappy with the portion sizes, quality, or variety. For a premium airline, food is a key differentiator, so this increase is worrying.

**3. In-flight Service (73 complaints)**

The Trend: This went up from 58 in 2022 to 73 in 2023.

The Insight: This is a concern because service is usually our strongest point. A rise here means passengers felt the crew were perhaps less attentive or rushed.

# 7. Conclusion & Recommendations
The data shows a clear pattern. While our logistical operations (like getting flights out on time) improved in 2023, the "on-board experience" declined. The significant rise in complaints about seats, food, and service suggests that while we are getting people to their destinations, they are enjoying the journey less than they used to.

# Recommendations:

**Review Seat Comfort:** Investigate specific aircraft types where seat complaints are highest.

**Audit Meal Service:** Conduct a survey to determine if the food issue is related to taste, quantity, or choice.

**Support Crew Training:** Review staffing levels to ensure cabin crew have enough time to care for every passenger on full flights.

**Disclaimer Analyst's Note:** The analysis presented in this report was performed by the author. Generative AI services were utilised solely as a tool to assist with drafting the structure of the report and refining the language for clarity. The data gathering, core calculations, and final strategic recommendations remain the sole intellectual product of the author.
