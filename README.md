


# Data-Visualization-with-Power-BI
<hr><b>Tools Used:</b> Power BI Desktop, Power Query, DAX, Power BI Service<hr>

![powerbi_project1_report](https://github.com/user-attachments/assets/633d59de-a6bd-4985-955f-e2f04c0bb267)

## Part 1: Defining Project Goals and Understanding the Data


For this project, I utilized an Excel dataset containing answers from a survey on professionals in careers related to data analysis. Microsoft Power BI was used to clean, transform, and visualize this data. The goal of this project was to answer the following questions about the data:

- Is work/life happiness related to salary?
- What were the most popular programming languages amongst participants?
- How does salary vary based on job title?

In order to work towards answering these questions, the dataset must first be observed and understood. A snippet of the original dataset is shown in figure 1.
<br><br>

![original_data_powerbi](https://github.com/user-attachments/assets/fe1535c1-d694-44ae-96d5-2dc34d0745b2)

Fig. 1. Original Survey DataSet

## Part 2: Data Cleaning and Transformation


After taking a look at the data, various aspects of it stood out that needed to be modified. The first of these was a number of completely empty columns, which were removed. These empty columns are shown in figure 2. The next modification was to handle certain columns which had an answer option of "other". This category was generalized into one "option" category, in order to group the various text entries together. This generalization was performed by splitting the column between "other" and the rest of the text entered by the participant. This split column was then removed from the dataset. This process is displayed in figure 3. Also, some columns that were deemed unneccessary for analysis, such as an email column (which only held the value "anonymous"), were removed. It was also observed that many rows in the dataset did not have a value for the "Highest Level of Education" field. These rows were removed from the dataset. The last data cleaning step that was taken had to do with the "Current Yearly Salary" field. Originally, this was a range of salary values. The average was taken from this range, and moved to a new column labeled "Salary". This new column was then multiplied to show the full salary value, as opposed to showing the value in thousands.

<br><br>

![powerbi_project1_step1_1](https://github.com/user-attachments/assets/5d77dfe5-1234-44fd-9c39-39288172b430)

Fig. 2. Empty Columns

<br><br>

![powerbi_project1_step2](https://github.com/user-attachments/assets/8a7da4a9-1e79-4bc8-8cc5-27d8afe986be)

Fig. 3. Splitting Columns


## Part 3: Data Visualization


Now that the data has been cleaned, the next step was to visualize it in the report view of Power BI. Three card visuals were used to display the number of survey participants, the average participant age, and the Pearson Correlation Coefficient between work/life happiness and salary. The correlation coefficient is discussed in detail in part 4 of this write-up. Additionally, two gauge visuals were used to display the average rating for salary and work/life balance. A clustered bar chart was used to depict the average salary by job title. For further categorization of data, a pie chart was created to show the favorite programming languages, and a treemap was created to show the participants by country. A scatter plot was created to show the relationship between salary and the score given to work/life balance. A histogram was also created which shows the participant count for various salary bins. The full report is displayed in figure 4.
<br><br>

![powerbi_project1_report](https://github.com/user-attachments/assets/48b203ea-4bcd-4e2a-92c7-39d97834f103)

Fig. 4. Power BI Report
<br><br>

## Part 4: Data Analysis


After visualizing the data, these visualizations were used to create insights that help to answer the originally posed questions about the dataset. The first question to answer has to do with the relationship between salary and the work/life balance score. Using the scatter plot and correlation coefficient, it was determined that there was a weak positive relationship between these two fields. This determination is backed up by the trend line of the scatter plot, and the coefficient of 0.25. Although there is a relationship between these fields, it is not one that has a strong effect on either. The next question to answer has to do with programming languages. The top two programming langauges among participants were Python and R. This makes sense, as these are the most popular languages for data analysis. The final question relates to variation of salary by job title. Looking at the report, it appears that most of the included job titles stayed around the $60k mark, with some outliers being data scientist, database developer, and student. This has been my process of cleaning, transforming, visualizing, and analyzing data.
