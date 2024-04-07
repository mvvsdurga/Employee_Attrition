EMPLOYEE ATTRITION

Project Summary:
  Employee attrition is the rate at which the employee leaves an organization either voluntarily or involuntarily. It is important for an organization to maintain low employee turnover to cut down the costs of recruiting new employees, to maintain high productivity, etc.. Our project is mainly to analyze the employee attrition rate and to identify the factors that can cause employee attrition, which can help organizations work in those areas so that they can retain their employees. 
Problem Statement: Cause and Factors that can cause employee attrition in an organization.
  For our Analysis, we took a dataset from Kaggle, which has around 1500 records and 35 columns. This dataset is created by IBM data scientists, which is for their reference.
Dataset: https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset
   After extracting the dataset we used that data to create models such as Logistic Regression, Neural Networks, Decision Trees, etc using Azure Machine Learning platform and for data preparation and model building of Genetic Algorithm, we used Heuristic Lab optimizer and later used Tableau to visualize the results we obtained. 
Data Exploration and Data Preparation:
 The Dataset that we have taken has around 1500 rows and 35 columns. Out of 35 columns, 34 are independent variables and the other one is a dependent variable which is Attrition, that will be predicted in the models.
                          
The data we took doesn’t have any missing values but for running the Genetic Algorithm, we changed the Attrition and overtime columns from String to Binary (0 or 1).
Tools Used:
1)	Heuristic Lab (Creating GA model)
2)	Azure ML (Creating data models)
3)	Tableau (Visualization of results)
Independent and Dependent Variables:
  From the problem statement, we know that we are predicting Employee Attrition, therefore from the dataset, the dependent variable/ Target Variable is “Attrition” and the independent variables used for prediction are:            Age,BusinessTravel,DailyRate,Department,DistanceFromHome,Education,EducationField,EmployeeCount,EmployeeNumber,EnvironmentSatisfaction,Gender,HourlyRate,JobInvolvement,JobLevel,JobRole,JobSatisfaction,MaritalStatus,MonthlyIncome,MonthlyRate,NumCompaniesWorked,Over18,OverTime,PercentSalaryHike,PerformanceRating,RelationshipSatisfaction,StandardHours,StockOptionLevel,TotalWorkingYears,TrainingTimesLastYear,WorkLifeBalance,YearsAtCompany,YearsInCurrentRole,YearsSinceLastPromotion,YearsWithCurrManager
Models Created:
As our problem is a binary classification problem, we won't be using Linear Regression to create a Model.
1)	Logistic Regression:
        The very first model that we ran our dataset. Logistic Regression is used mostly for classification problems and returns the result in Binary form. It can be Yes/No or 0/1. If we have 3 output types, then we can use a multinomial Logistic Regression model. Right now, we have 2 output types so we will be using the Two-Class Logistic Regression model. 
2)	Decision Trees:
We also used decision trees for Attrition prediction, where the model is built in a tree-like structure and the prediction of whether an employee leaves an organization or not is done at leaf nodes. In decision Tree model splits the data recursively into smaller sub-sets. Decision Trees have high explainability as anyone can understand from it. Decision trees are useful tools for HR professionals looking to understand and reduce employee turnover since they are interpretable and can assist in uncovering important elements impacting attrition.
3)	Boosted Decision Trees:
    For classification and regression tasks in machine learning, boosted decision trees are a sort of ensemble learning technique. In general, decision trees are used to merge several weak learners into a single powerful prediction model. Boosting is an iterative process that constructs decision trees one after the other, each one focusing on fixing mistakes or incorrect classifications made by the prior trees. The basic goal of boosting is to combine the capabilities of various simple models to produce a robust and accurate model. We used a Boosted decision tree to overcome the overfitting problem as it is computationally more intensive.
4)	Neural Networks:
      The term "neural network" refers to a computer model that draws its inspiration from the structure and operation of the neural networks in the human brain in the context of artificial intelligence and machine learning. It is a layer-organized network of artificial neurons that can analyze input and learn from it. To perform a variety of tasks, including speech and image recognition, natural language processing, recommendation systems, and others, neural networks must be able to understand complicated patterns and representations in data.
5)	Genetic Algorithm:
The last model through which we ran our dataset is the Genetic Algorithm. A genetic algorithm (GA) is a search and optimization method that draws inspiration from the laws of genetics and natural selection. By imitating the laws of evolution, it is used to discover approximations of solutions to optimization and search issues. The larger category of evolutionary algorithms includes genetic algorithms. It is especially helpful when the search space is big, complicated, or not well known since they can effectively explore and utilize the solution space.                 
From the above comparison, we found the following observations:
(i)	Logistic Regression has the highest accuracy out of all the data models.
(ii)	Even though Neural Networks have Accuracy almost the same as Logistic Regression, we ruled it out by considering the fact of explainability factor of the Neural Network model.
(iii)	Even though Decision Trees have high explainability, we didn’t go with it as it has low accuracy compared to the Logistic Regression model.
(iv)	For the Genetic Algorithm the Accuracy is very low so we are not considering it.
Therefore, we are going with the Logistic Regression model for solving the Employee Attrition problem.
Recommendations and Insights:
Therefore, the most significant factors affecting the target variable according to the Logistic Regression analysis are Overtime, Job Satisfaction, Environment Satisfaction, and Marital Status. From this, we can derive the following advice and insights that can assist the business in lowering the employee attrition rate:
(i)	To ensure fair compensation for overtime work, increase the employee overtime allowance.
(ii)	Avoid discriminating against people based on their marital status and foster a climate of neutrality and fairness inside the organization.
(iii)	Utilize a comprehensive system that features both monetary and non-cash rewards to acknowledge and honor employee contributions.
(iv)	Make sure that employees receive pay and stock options at the same rates for comparable job titles and levels of involvement.
