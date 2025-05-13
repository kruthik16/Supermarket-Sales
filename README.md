# Supermarket-Sales
Supermarket-Sales EDA analysis (answering common question by the stakeholders)
Project Background
The growth of supermarkets in most populated cities are increasing and market competitions are also high. The dataset is one of the historical sales of supermarket company which has recorded in 3 different branches for 3 months data. Predictive data analytics methods are easy to apply with this dataset.

Attribute information
Invoice id: Computer generated sales slip invoice identification number
Branch: Branch of supercenter (3 branches are available identified by A, B and C).
City: Location of supercenters
Customer type: Type of customers, recorded by Members for customers using member card and Normal for without member card.
Gender: Gender type of customer
Product line: General item categorization groups - Electronic accessories, Fashion accessories, Food and beverages, Health and beauty, Home and lifestyle, Sports and travel
Unit price: Price of each product in $
Quantity: Number of products purchased by customer
Tax: 5% tax fee for customer buying
Total: Total price including tax
Date: Date of purchase (Record available from January 2019 to March 2019)
Time: Purchase time (10am to 9pm)
Payment: Payment used by customer for purchase (3 methods are available – Cash, Credit card and Ewallet)
COGS: Cost of goods sold
Gross margin percentage: Gross margin percentage
Gross income: Gross income
Rating: Customer stratification rating on their overall shopping experience (On a scale of 1 to 10)
Data Source : [https://kaggle.com/datasets/aungpyaeap/supermarket-sales]
With this given dataset the following questions are being answered. Insights and recommendations are provided on the following key areas:

What are the key factors driving revenue and profitability across different branches and product lines?
How do customer demographics (such as customer type and gender) impact purchasing behavior and product preferences?
What are the patterns or trends in customer satisfaction ratings across branches, times, or product lines?
Which payment methods are most popular, and do they correlate with larger purchases or specific customer segments?
Are there seasonal or time-based trends in sales volume, and how can we leverage them to maximize peak times?
An interactive Tableau dashboard used to report and explore sales trends can be found here Dashboard Link . Tablaeu story 1

Data Structure & Initial Checks
The companies main database structure as seen below consists of two tables: table 1 and table 2 with a total row count of 1000 records. A description of each table is as follows:

Table 1:glimpse of data
Table 2:summary of data
[Entity Relationship Diagram here]

Executive Summary
Overview of Findings
Revenue and profitability are primarily driven by high-margin and low margin product lines like 'Food & Beverages' & 'Home & life-style' , with Branch C outperforming other ones due to larger customer bases and operational efficiencies. Customer demographics reveal that members drive higher spending and loyalty, while gender preferences indicate male customers have higher spending than Health & Beauty to female customers. Lastly, customer satisfaction trends highlight the need to address peak-time challenges, with lower ratings for 'health & beauty' in branch A , 'Food and bevarages' in B & 'sports & travel' and ' home & lifestyle' for C.

[Visualization, including a graph of overall trends or snapshot of a dashboard]

Insights Deep Dive
What are the key factors driving revenue and profitability across different branches and product lines?:
Main insight 1. The primary factors driving revenue are product line performance, branch differences, and customer type. Branch C shows the highest revenue, driven by strong sales in high-demand product lines like 'Food and beverages' and 'Fashion Accessories.' In terms of profitability, All branches stand out due to high gross margins in specific product lines, suggesting that operational efficiencies or customer preferences may play a role.  For 'A' it is:'Home and lifestyle', 'sports and travel', 'Electronic'. For 'B' it is ; 'Sports and travels', 'health and beauty'. For 'C' it is 'Food and beverages and Fashion Accessories'. Branch Revenue Revenue with each product line

Main insight 2. In branch 'A''s  product line of 'health and beauty','food and beverages', 'Fashion Accessories' having a high gross margin percentage means a company is keeping a large portion of its sales revenue as profit after subtracting the cost of goods sold, indicating efficient cost management and potentially higher profitability, while having "low gross income" means the company is generating a relatively small amount of profit from sales, even if their gross margin percentage is high, which could be due to low sales volume.On the other hand, Branch 'B' is being efficient in selling 'Sports and travel'. But in other product lines, special mention , 'Fashion accessories ' and 'food and beverages' having low gross income. Branch profit Margin Unit price Margin

Main insight 3. In Branch 'C' the story is quiet opposite from branch 'A'. It is giving higher revenue in products like, 'Food and beverages', 'Fashion Accessories'. While bringing low revenue in ' Home and life style ' and 'health and beauty'. Although Branch 'B' produce most revenue and efficient in selling ' Sports and Travel', Among the 3 branches it sells 'Health and beauty' efficiently.

Main insight 4. Branch C shows the highest revenue, driven by strong sales in high-demand product lines like 'Food and beverages' and 'Fashion Accessories.' In terms of profitability, All branches stand out due to high gross margins in specific product lines, suggesting that operational efficiencies or customer preferences may play a role.  For 'A' it is:'Home and lifestyle', 'sports and travel', 'Electronic'. For 'B' it is ; 'Sports and travels', 'health and beauty'. For 'C' it is 'Food and beverages and Fashion Accessories'.

How do customer demographics (such as customer type and gender) impact purchasing behavior and product preferences?:
Main insight 1. After analyzing the purchasing patterns, we see that members tend to purchase more frequently and spend more per visit compared to non-members, especially in categories like Food and brvarages and Home & Lifestyle, and Sports and travel(see spending pattern by customer type chart). Aditinally, Female basket size, means the item grabbed each visit is 9.7% more than a male customer(see basket size chart). Additionally they tend to give, 9.2$ more revenue on an average(Average spending comparison chart).

viz1
Main insight 2. Additionally, female customers appear to less prefer categories like Health & Beauty, yet they prefer Food and beverages more. There’s also a trend of male members favoring Health& beauty, sports and beverages, electronics, potentially indicating a high-value demographic that could be targeted with loyalty incentives(see product line preference Heatmap). Female customer spends approx 24$ more than a male customer in the supermarket across all branches (see Avg.spend per visit by gender) .

viz2
Main insight 3. In the following heatmap you can see there are the overall all type of payments made by female customer for 'Health & Beauty' across all branches is lesser than the rest. Again for male customers have significantly less spending on credit cards in 'Home and lifestyle' section. Product line preferences by payment method

Main insight 4. In this following heatmap we can Female- member customers gives more revenue than male-member customers.

High Margin products
[Visualization specific to category 2]

What are the patterns or trends in customer satisfaction ratings across branches, times, or product lines?:
Main insight 1. Overall, Branch C has higher ratings in both type of members and non-members with average of ratings 7.068. Then the higher satisfaction is at branch A following branch B.

Main insight 2. The highest rating recieved by Branch 'B' and 'C' during 12:00 which is average of 7.39. For A it is 18:00 which is 7.31.

Main insight 3. In the following heat map we can see there is some constand bad ratings to the product line which closely similar to the point we discussed in previous inshights for different questions. Link of the tablaeu heatmap Product line satisfaction trend

Main insight 4. In this bubble chart the revenue in peak hours which is 12- 13 pm . The rating for each product how it varies for each branch. The 'Fashion Accessories' in branch A & C 'Health and Beauty' in B gives more revenue. Feel free to try out the filters, Tablaeu bubble chart

Cross Factors Analysis

Are there seasonal or time-based trends in sales volume, and how can we leverage them to maximize peak times?:
The data present here is giving sales of one year ( Jan 2019- Dec 2019). So, due to insufficient data it is hard to tell if there is trends present in the data based on one cycle.
Recommendations:
Based on the insights and findings above, we would recommend the [stakeholder team] to consider the following:

Focus on High-Margin Products: Prioritize stocking and promoting high-margin product lines like Health & Beauty and Food & Beverages. Recommendation or general guidance based on this observation.

Branch-Specific Strategies: Invest in operational efficiencies for underperforming branches to align their profitability with top-performing ones. Tailor inventory to suit regional preferences to drive higher sales. Recommendation or general guidance based on this observation.

Loyalty Program Enhancements: Introduce targeted rewards for members based on their purchasing patterns to further boost loyalty. Convert non-members by offering introductory discounts or membership benefits.. Recommendation or general guidance based on this observation.

Customer Feedback Systems: Deploy surveys and feedback tools to continuously monitor satisfaction and address pain points in real-time. Recommendation or general guidance based on this observation.

Assumptions and Caveats:
Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

Assumption 1 (ex: missing country records were for customers based in the US, and were re-coded to be US citizens)

Assumption 1 (ex: data for December 2021 was missing - this was imputed using a combination of historical trends and December 2020 data)
