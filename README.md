# Introduction
Aviation and travel are my greatest passions. I view the entire passenger journey as a series of crucial touchpoints: from ticket purchase and airport arrival to the check-in process, the comfort of the in-flight seat and meal, and the overall onboard services. I always aim for seamless service and expect a high level of comfort, especially when paying a premium for the experience. However, particularly on long-haul flights, a consistently excellent experience is not always guaranteed.

# Case Scenario
As a Junior Data Analyst within the Customer Experience (CX) department at Singapore Airlines, my primary role is to listen to what our passengers are saying. We take immense pride in our world-class service, but actively using feedback is the only way to stay ahead. Recently, we observed a subtle shift in the nature of customer comments, leading to a new task for me: understand exactly what happened in our review data over the last year.

My manager approached me with a specific concern. While we generally maintain high ratings, we urgently needed to pinpoint specific customer pain points to improve our 2024 strategy. The request was clear and simple: identify the top three categories of complaints for 2023. To ensure these figures had meaningful context, I was also asked to compare them with our 2022 data. This comparison is vital, as it allows us to establish a pattern and determine whether an issue is a new, immediate concern or an underlying problem that has been happening for a long time.

# Data Source
I would like to thank fellow kagglers, Kanchana1990 for making [Singapore's Airlines Review](https://www.kaggle.com/datasets/kanchana1990/singapore-airlines-reviews) dataset available. For the purpose of this case study, I performed the analysis using two full years of customer review data, specifically covering the period from 2022 through to the end of 2023. This two-year scope was essential for establishing clear patterns and trends in passenger complaints before diving into the specific pain points identified in the most recent year.

# Main Goal
The primary objective of this analysis was to:
1) Identify the top 3 categories of complaints in 2023.
2) Compare these numbers with 2022 to spot trends.
3) Provide clear evidence so the management team can allocate resources to fix these specific issues.

# Data Preparation Process
Here is the simple process I followed:

## Data Cleaning: 
1) I looked through the raw reviews to ensure the dates were correct and that the comments were categorised properly (e.g., tagging a comment about "small seats" under "Seat/Legroom").

2) Grouping: I organised the data by year (2022 vs. 2023) and by specific complaint categories.

3) Pivot Table Analysis: I created a summary table (Pivot Table 1) to count exactly how many times each issue was mentioned in each year. This allowed me to see the "Grand Total" and the year-on-year changes clearly.

# Key Findings

When comparing 2022 to 2023, the data tells an interesting story.

* Total Volume: Some complaints are actually going down. For example, complaints about Flight Cancelation/Delay dropped from 93 in 2022 to 73 in 2023. This is a great sign that our operations are stabilising.
* The Shift: However, complaints about the physical experience inside the plane are going up.
* The Top 3: The most frequent complaints in 2023 were about Seats, Meals, and Service/Delays.

# Result
[View Dashboard](https://github.com/mfarisakram/excel-dashboard/blob/main/dashboard.png)

Here is the breakdown of the top issues we faced in 2023 based on the data.

### 1. Seat and Legroom Issues (107 complaints) This was the number one complaint for 2023.
The Trend: In 2022, we had 67 complaints about this. In 2023, it jumped to 107.
The Insight: This is a massive increase. Passengers are finding the seats uncomfortable or the legroom insufficient. Since this number nearly doubled, it suggests that as our flights became fuller post-pandemic, passengers became much more sensitive to personal space and seat comfort.

### 2. In-flight Meal (88 complaints) Food was the second biggest issue.
The Trend: This rose from 70 complaints in 2022 to 88 in 2023.
The Insight: While not as steep a rise as the seat issues, it is still an upward trend. Passengers are likely unhappy with the portion sizes, the quality, or the variety of the food served. For a premium airline, food is a key differentiator, so this increase is worrying.

### 3. In-flight Service & Flight Delays (Tie at 73 complaints) In third place, we have a tie between two categories.
In-flight Service: This went up from 58 in 2022 to 73 in 2023. This is a concern because service is usually our strongest point. A rise here means passengers felt the crew were perhaps less attentive or rushed. 
Flight Cancellation/Delay: As mentioned, this actually improved (down from 93 in 2022), but it is still high enough to be in the top 3.

# Conclusion
The data shows a clear pattern. While our logistical operations (like getting flights out on time) improved in 2023 compared to 2022, the "on-board experience" declined. The significant rise in complaints about seats, food, and service suggests that while we are getting people to their destinations, they are enjoying the journey less than they used to.

# Recommendations
Based on these findings, I recommend the following actions:

* Review Seat Comfort: We should investigate specific aircraft types where seat complaints are highest. It might be time to check if seat cushions need replacing or if the layout in Economy needs review.
* Audit Meal Service: We need to look at the food menus again. A survey could help us find out if the issue is taste, quantity, or choice.
* Support Crew Training: With service complaints rising, our cabin crew might be overworked due to full flights. We should look into staffing levels to ensure they have enough time to care for every passenger.

#### Disclaimer
Analyst's Note: The analysis presented in this report, including the data summaries and interpretation, was performed by the author. Generative AI services were utilised solely as a tool to assist with drafting the structure of the report, suggesting efficient Excel formula logic, and refining the language for clarity and adherence to British English standards. The data gathering, core calculations, and final strategic recommendations remain the sole intellectual product of the author.

