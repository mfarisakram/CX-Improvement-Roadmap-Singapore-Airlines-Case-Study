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


