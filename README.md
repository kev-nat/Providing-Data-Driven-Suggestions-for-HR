# Providing-Data-Driven-Suggestions-for-HR

### **Overview**
<p align="justify"> In this project, I examined a dataset and developed predictive models to generate insights for the Human Resources (HR) department of a major consulting firm. I employed various machine learning models to forecast employee attrition, evaluated their performance, and selected the best-performing model for deployment. </p>

### **Business Understanding**
<p align="justify"> Salifort Motors' HR department aims to enhance employee satisfaction and has gathered data from their workforce but needs guidance on how to utilize it effectively. They seek data-driven insights to understand the factors influencing employee turnover, specifically asking, "What’s likely to make an employee leave the company?" </p>

<p align="justify"> My objectives in this project are to analyze the collected data and develop a predictive model to determine whether an employee is likely to leave. By identifying employees at risk of quitting, we can uncover the underlying reasons for their departure. Since recruiting new employees is both time-consuming and costly, improving employee retention will be advantageous for the company. </p>

### **Data Understanding**
<p align="justify"> The <a href="https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv">dataset</a>, contains 14,999 rows and 10 columns. The features encompass employee-reported job satisfaction levels (ranging from 0 to 1), the score of the employee's last performance review (ranging from 0 to 1), the number of projects the employee is involved in, the average number of hours worked per month, and an indicator of whether the employee left the company. </p>

<p align="justify"> The visualization below shows a stacked boxplot of <code>average_monthly_hours</code> distributions for <code>number_project</code>, comparing the distributions of employees who stayed versus those who <code>left</code>. </p>

![image](https://github.com/user-attachments/assets/2b678e62-e510-4911-818d-ef05f20fd914)

<p align="justify"> The scatterplot below shows the <code>average_monthly_hours</code> vs <code>satisfaction_level</code>, comparing employees who stayed vs those who <code>left</code>. </p>

![image](https://github.com/user-attachments/assets/5ba3d8c0-3265-486c-837f-e7123f9f5d3c)

<p align="justify"> A stacked histogram to compare department distribution of employees who left to that of employees who didn't </p>

![image](https://github.com/user-attachments/assets/782ed791-f4a1-47af-b27c-4bde2bc8bce9)

<p align="justify"> A heatmap to visualize how correlated variables are. Considering which variables we're interested in examining correlations between. </p>
  
![image](https://github.com/user-attachments/assets/2881455c-6271-417a-8c5b-c5415d590332)

### **Modeling and Evaluation**
<p align="justify"> A random forest model with 300 decision trees was utilized to identify the key features influencing employee turnover. The plot below indicates that in this random forest model, <code>last_evaluation</code>, <code>number_project</code>, <code>tenure</code>, and <code>overworked</code> are the most significant predictors, listed in descending order of importance. These features are also the top predictors in the decision tree model. The random forest model achieved an AUC of 94% and a recall of 90%. </p>

![image](https://github.com/user-attachments/assets/1dd8830c-33be-4f33-ade9-6bce20b43fb9)

### **Conclusion**
<p align="justify"> This model can assist the HR department in predicting which employees are likely to leave the company. Additionally, it can help identify the factors contributing to employee turnover, enabling the HR team to take actions to improve retention. This is particularly valuable as recruiting, interviewing, and hiring new employees is both time-consuming and costly. </p>
