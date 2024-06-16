![Data Science ](https://github.com/Negar86/Project2/assets/160590005/8610cf7f-01b8-4c62-a522-5fa74723a8af)
# Data Science Job Salaries
## EDA & Machine learning
---

## Introduction:
Data Scientist job market trends over the past four years (2020-2024). In this project, we delve into a comprehensive dataset sourced from <b>Kaggle</b>, which provides a detailed overview of various aspects of the Data Scientist job market. Our goal is to uncover significant trends, insights, and patterns that have emerged in this rapidly evolving field. 

Dataset columns:
- Job Title     
- Experience Level   
- Employment Type   
- Remote Ratio   
- Company Size   
- Company Location   
- Employee Residence   
- Salary
---
## EDA (Exploratory Data Analysis)
#### Number of Job Titles and Average Salary Over Years (2020-2024)
<img width="648" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/83d139b4-a646-46d1-984d-187878b3fe55">

---
### Salary Distribution
<img width="655" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/9d15fcac-7401-48c3-929a-c83224ba4aa4">


<img width="118" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/09961904-2431-4a68-8489-7f9b70bb9972">


---
### Experience Level
<img width="207" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/5c1f6e4a-73c0-4e19-9b0f-6c2289e13224">


<img width="385" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/7038c74b-6e0e-4a47-8fc4-3a8b54f9c0d7">


---
### Job titles 
<img width="669" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/c4dbddf6-a765-4dc2-bb29-509a77df3fc0">

<img width="646" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/4deb590f-ecd2-43bc-a4a9-c8471133bfd2">

---

### Salary Distribution by Job titles and experience level 
![image](https://github.com/Negar86/Project2/assets/160590005/effb78a8-c04b-414c-ac41-201a207e8e2c)


---
### Remote Ratio

<img width="653" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/27f9d0d2-57a4-40a3-8867-ce98a0b5eb54">


<img width="721" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/24cb9063-a825-4f88-8a02-52de94d76432">

----
### Distribution of Company Size by Experience level
<img width="549" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/0cf5867c-7ec9-4b8a-aceb-eeece52281a7">

Chi2: 167.7140   
P-value: 1.3733   
Cramer’s V: 0.0856126   

There is association between the Company size & Exp level but the correlation is not strong.  

---

### Company Country
<img width="663" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/bea37ae2-d847-4ccc-bbbb-2f6deba0232b">

<img width="699" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/c67533b2-fd0c-4276-a8b3-cbe998b86f62">

<img width="641" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/55d73326-72e4-49a3-91e7-fb21138c2dd9">
---

## ML (Machine Learning)
For predicting salay below models are tested and results are as below table:
![image](https://github.com/Negar86/Project2/assets/160590005/6bcf290e-fa82-4b3f-9def-111df992d769)

The Ridge regression model explains around 27.33% of the variance in salary prices (R² = 0.2733). However, the prediction errors are relatively large, with an average absolute error of about 41,987 Euro(MAE) and a typical prediction error of about 58,756 Euro (RMSE). The high MSE value also indicates significant prediction errors. These metrics suggest that while the model provides some predictive capability, its accuracy and explanatory power are limited, indicating room for improvement.

<img width="585" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/4780857c-5ec2-4e6e-9bce-611d2431ce8e">

----
### Dealing with outliers:


After removing the outliers based on the first and third quartiles of the salary data:

- The model's explanatory power has improved, with R² increasing to 32.69% from 27.33%.      
- The prediction errors have reduced, as indicated by lower RMSE, MSE, and MAE values. The typical prediction error (RMSE) has decreased by approximately 11,204 Euro, and the average absolute error (MAE) has decreased by around 3,965 Euro.   
These improvements suggest that removing the outliers has resulted in a more accurate and reliable model for predicting salary prices, though there is still room for further enhancement.

<img width="574" alt="image" src="https://github.com/Negar86/Project2/assets/160590005/e04e820e-a908-4212-bbd3-dda1059b827b">

