# Power_BI_Dashboard_PwC_Switzerland_-Job_Simulation

## Overview
This project is part of the PwC Switzerland Power BI Virtual Case Experience. It focuses on analyzing telecom data using Power BI to create interactive dashboards that provide insights into customer service, retention trends, and diversity & inclusion efforts.

## Project Scope
The goal of this project is to visualize key performance indicators (KPIs) to assist decision-making in different business areas of a telecom company. The analysis is divided into three main tasks:

## Customer Service Analysis
Understanding call center efficiency and customer satisfaction by analyzing:
- **Overall Customer Satisfaction** – Customer feedback ratings.
- **Call Center Performance** – Calls answered vs. abandoned.
- **Time-Based Call Analysis** – Peak call times and average handling speed.
- **Agent Performance** – Comparing average talk duration vs. calls answered.
![image](https://github.com/user-attachments/assets/3ac19ffe-0c75-47a1-a7f7-1b74dd52dbb0)

## Insights from the Call Center Trends Dashboard:
- **Total Calls: 5000**

The call center handled a significant volume of calls, indicating a busy environment that requires efficient resource management.
- **Answer Rate: 81.08%**

A relatively high answer rate suggests good responsiveness, but there is room for improvement to minimize abandoned calls.
- **Average Speed of Answer: 54.75 seconds**

The average time to answer a call is nearly a minute, which may affect customer satisfaction. Reducing this could enhance service quality.
- **Average Call Duration: 0.41 minutes (approximately 25 seconds)**

Calls are relatively short, which may indicate quick resolutions or rushed interactions that might affect customer satisfaction.
- **Resolution Rate: 72.92%**

While a majority of calls are resolved, nearly 27% remain unresolved, suggesting the need for better issue resolution strategies.
- **Calls Per Day Trend**

Fluctuations in call volume suggest peak times that could be used to optimize agent staffing.
- **Customer Satisfaction Score: 2.8/5**

A low satisfaction score indicates that customers may be experiencing issues with service quality, wait times, or resolution effectiveness.
- **Calls Handled by Agent**

Some agents handle significantly more calls than others, highlighting potential workload imbalances or differences in efficiency.

**Filtering Options**

Filters for month, agent, topic, and resolution status allow deeper insights into specific trends and performance metrics.
### Recommendations:
- Improving resolution rates and satisfaction scores should be a priority.
- Optimizing staffing during peak hours could help manage call volumes more effectively.
- Analyzing individual agent performance might uncover training or resource needs to enhance efficiency.

## Customer Retention Analysis
Understanding customer churn patterns and identifying opportunities for proactive retention strategies.

- **Customer Churn Rate:** The churn rate stands at 26.54%, indicating a significant portion of customers are leaving. This represents a revenue loss of $2.86M.
- **Churn by Payment Method:** Customers using electronic checks have the highest churn rate (34%), suggesting a need to review billing experiences for these users.
- **Churn by Internet Service Type:** Customers with fiber optic internet have the highest churn rate (42%), compared to DSL (19%), highlighting potential service quality concerns.
- **Contract Type Impact:** Month-to-month contracts show the highest churn (55%), while customers on one-year (21%) and two-year (24%) contracts churn less. Encouraging longer-term commitments may help reduce churn.
- **Churn by Paperless Billing:** 41% of churned customers opted for paperless billing, while 59% did not, suggesting billing preferences may not be a key driver of churn.
- **Churn by Gender:** The churn rate is almost evenly split between male (51%) and female (49%), indicating no strong gender-based trend.
- **Churn by Subscription Length:** Customers in their first year have the highest churn rate, which gradually decreases with tenure. This suggests that early-stage customer engagement and support are critical for retention.

![image](https://github.com/user-attachments/assets/a3dfbbb9-8eb0-48eb-8a4f-43876216c01e)

### Recommendations:
- Implement personalized retention strategies for high-risk groups, such as fiber optic users and electronic check payers.
- Encourage long-term contracts through discounts or loyalty incentives to improve retention.
- Enhance onboarding and support for new customers to reduce early-stage churn.
- Investigate service quality issues for fiber optic users to improve satisfaction and lower churn rates.

## Diversity & Inclusion Analysis

Assessing gender diversity in hiring, promotions, and job levels to identify areas for improvement in workplace inclusion.

- **Hiring Gender Distribution:** The company maintains a balanced hiring ratio, with 48.48% men and 51.52% women hired, indicating an effort toward gender diversity.
- **Turnover Rate: The 9.40% turnover rate, with 47 total leavers, suggests stability but warrants further analysis to ensure retention strategies are inclusive.
- **Gender Representation by Job Level:** Women are well-represented at junior levels but face a declining presence at higher job levels (e.g., Senior Manager, Director, and Executive), indicating potential barriers to leadership roles.
- **Promotion Rates by Gender:** 11% of men and 9% of women were promoted, revealing a slight gender gap in career advancement.
- **Hiring Trends by Job Level (Post FY21):** Women dominate new hires at junior levels, but men are significantly favored for higher roles, raising concerns about leadership pipeline diversity.

**Hiring by Department:**
- HR: 100% female hires
- Operations: 59% female, 41% male
- Sales & Marketing: 61% male, 39% female
- Finance and Strategy have a near equal gender split, but imbalances in other areas highlight recruitment gaps.
![image](https://github.com/user-attachments/assets/e5566ee8-b827-48b2-973b-4bfd17732809)

### Recommendations:

- Implement mentorship and leadership programs to increase female representation in senior roles.
- Encourage equitable promotion opportunities to close the gender gap in career growth.
- Address gender imbalances in hiring across departments to foster a more inclusive workforce.
- Analyze potential retention challenges for women in higher positions and develop targeted retention initiatives.

## Key Insights
| **Category**  | **Key Finding**  |
|--------------|-----------------|
| Customer Service  | Identified inefficiencies in call center operations, leading to actionable improvements. |
| Customer Retention | Highlighted customer churn risk factors, enabling proactive retention efforts. |
| Diversity & Inclusion | Uncovered gender disparities in promotions, helping HR strategize better inclusivity initiatives. |

## Installation and Usage
1. **Download Power BI Desktop**: [Power BI Download](https://powerbi.microsoft.com/)
2. **Open the provided Power BI (.pbix) file**
3. **Explore dashboards using filters and slicers**
4. **Use insights to drive data-driven decision-making**

## Example DAX Calculation
```DAX
Customer_Churn_Rate = 
    DIVIDE(
        COUNTROWS(FILTER(Customers, Customers[Status] = "Churned")),
        COUNTROWS(Customers),
        0
    )
```
