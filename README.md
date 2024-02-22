# Customer Segmentation Analysis (Ed-tech data)


## Background:
The success of any business heavily relies on understanding its customers and catering to their needs effectively. our organisation, aims to enhance its marketing strategies by segmenting its customer base to tailor marketing efforts, improve customer experience, and maximize revenue.

## Objective:
The primary objective of this project is to segment customers based on their behavior, preferences, and demographics to facilitate targeted marketing campaigns and personalized experiences.



#### Challenges:
- Heterogeneous Customer Base:Our customer base consists of individuals with diverse preferences, purchasing behaviors, and demographics.
- Data Complexity: Customer data is collected from various sources, leading to complexity in data structures and formats.
- Optimal Segmentation: Identifying meaningful customer segments to ensure actionable insights and effective marketing strategies.
- Scalability: Ensuring that the segmentation approach is scalable and adaptable to accommodate future growth and changes in customer behavior

### Tools Used
Power BI: Used for data visualization, analysis, and creating interactive dashboards.


### Project Statement
The primary objectives of the project were:

- Data Collection and Preparation: Gather and clean customer data from various sources to ensure data quality and consistency.
- Exploratory Data Analysis (EDA): Perform exploratory analysis to understand customer demographics, behavior, and preferences.
- Visualization and Insights: Develop interactive dashboards in Power BI to visualize segmentation results and extract actionable insights.
- Recommendations: Provide recommendations for targeted marketing campaigns, product recommendations, and personalized customer experiences.

### Project Structure
1) Data Preprocessing: Includes data cleaning, feature engineering, and data transformation.
2) Exploratory Data Analysis: Visualizations and insights derived from the exploration of customer data.

3) Power BI Dashboard: Interactive dashboard showcasing segmentation results, visualizations, and insights.


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a xlsx file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column Board", "column Grade" & "column Date of orientation" options.
- Step 3 : Also since by default, profile will be opened only for 500 rows so you need to select "column date of orientation based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present except column named "Name of student".
- Step 5 : Changed data types into valid formate,removed null values and changed date formate to month in separate column.
- Step 6 : Written DAX expression on count of students who are active and refunded  and analysed from which segment they belongs to.
- Step 7 : Imported 'CSAT' score through feedback forms and merged column in the same dataset.
- Step 8 : Visual filters (Slicers) were added for four fields named "% of active customer", "Customer satisfaction", "Customer engagment" & "Overall customer in specific region".

- Step 9 : Two card visuals were added to the canvas, one representing Max registration by which segment & other representing average customer engagement.
           Using visual level filter from the filters pane, basic filtering was used & null values were unselected for consideration into average calculation.
           
           Although, by default, while calculating average, blank values are ignored.

- Step 10 : A bar chart was also added to the report design area representing the number of active customers. While creating this visual, field named "Board" was also added to the Legends bucket, thus number of customers are also seggregated according the Board. 
- Step 11 : File represents two different visuals ,One is of month wise active and refund count another shows segmentation analysis.

  

- Step 12 : In the report view, under the insert tab, two text boxes were added to the canvas, in one of them name of the airlines was mentioned & in the other one company's tagline was written.
- Step 13 : In the report view, under the insert tab, using shapes option from elements group a rectangle was inserted & similarly using image option company's logo was added to the report design area. 
- Step 14 : Calculated column was created in which, customers were grouped into various age groups.

for creating new column following DAX expression was written;
       
        Active customer=
          
        "(Overall customer)-(refund in current month)",
                
Snap of new calculated column ,




![Snap_1](https://github.com/Pavan3201DS/Customer-segmentation/assets/159137836/8e40445f-54aa-43bf-be9c-03ee001e0f39)


        
- Step 15 : New measure was created to find total count of customers.

Following DAX expression was written for the same,
        
        Count of Customers = COUNT(% of active customer feedback)
        
A card visual was used to represent count of customers.

![Snap_Count](https://github.com/Pavan3201DS/Customer-segmentation/assets/159137836/76d85759-e068-4071-ab1b-d2117104491e)

- Step 16 : New visual is added in the canvas (Purchase behaviour) to know from which segment max customers purchasing course

 

 A card visual was used to represent this perecntage.
 
 Snap of % of customers who purchased course, this 
 
 ![Snap_Percentage](https://github.com/Pavan3201DS/Customer-segmentation/assets/159137836/c7bcc973-026c-4497-98c2-6107c0f80989)

 
 - Step 17 : New visual page is added which shows month wise registration to the course
 
 
 ![Snap_3](https://github.com/Pavan3201DS/Customer-segmentation/assets/159137836/14c22573-75d4-4559-8fc3-0bd4c1172e60)
 

# Snapshot of Dashboard (Power BI Service)

![dashboard_snapo](https://github.com/Pavan3201DS/Customer-segmentation/assets/159137836/566973c9-d4d8-4f55-b461-d4761b9f435d)

 

# Insights

A two page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] Total Number of Customers = 319

   Number of satisfied Customers = (58.68 %)


   Number of neutral/unsatisfied customers= (27.58 %)



           thus, higher number of customers are neutral/satisfied.
           
### Results
Identified four distinct customer segments based on purchasing behavior, demographics, and geographic location.

Segment 1: High-Value Customers - High cost registration,high engagement.

Segment 2: Potential Loyal Customers - Moderate spending, occasional purchases, but high engagement.

Segment 3: Discount Seekers - Low to moderate spending,but mostly during discount periods.

### Files included
customer_segmentation.pbix: Power BI file containing the interactive dashboard.
Dataset from course registration.
Resourse : Self collected data from current organisation

README.md: Project overview, instructions, and documentation.
