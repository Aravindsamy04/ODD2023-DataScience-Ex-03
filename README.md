# ODD2023-DataScience-Ex-03

### Aim:
To read the given data and perform the univariate analysis with different types of plots.

Explanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

### Algorithm:
Step1
Read the given data.

Step2
Get the information about the data.

Step3
Remove the null values from the data.

Step4
Mention the datatypes from the data.

Step5
Count the values from the data.

Program:
```
Developed By : ARAVIND SAMY P
Register number: 212222230011

# Superstore.csv:
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('SuperStore.csv')
print(df)
df.head()
df.info()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
df.describe()

### Diabetes.csv:
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
df.kurtosis()

### employeesal.csv:

import pandas as pd
df=pd.read_csv("/content/employeesal.csv")
df
df.info()
df.dtypes
df['Salary'].value_counts()
df.describe()
import seaborn as sns
sns.boxplot(x='Experience_Years',data=df)
sns.countplot(x="Experience_Years",data=df)
sns.distplot(df['Experience_Years'])
sns.histplot(x="Experience_Years",data=df)
df.skew()
sns.histplot(x='Salary',data=df)
sns.distplot(df['ID'])
df.kurtosis()
sns.boxplot(x='Salary',data=df)
sns.boxplot(x='Experience_Years',data=df)
```
## Output:

### Superstore.csv:

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/281a0659-c9b2-4d95-91de-33540c853bd1)

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/42f6da91-760a-489d-99c4-758785f5467c)

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/274d5f69-0e5a-49af-a6e5-54c627e81234)

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/418809b8-1921-435a-8614-6170a8235472)

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/418a705e-613d-4db7-ab00-e0eea0c8015d)

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/df21227b-a33d-400a-adde-ab13c891247e)


![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/57ee4d74-0ce9-4993-a9b5-efeb75a8eb73)

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/1cd58b20-e7a4-4f9d-b148-8309b23901b5)


![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/7c8d28e5-4aa4-4f08-aa8f-701451dcf0d2)


### Diabetes.csv:

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/419e9958-ebfc-4655-a1a8-2c454cb74850)

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/f9f618de-821f-4f83-8a3c-39ec10b2daa1)



![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/ec99b681-0d52-44fc-9856-8497f1b364f1)


![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/faeeeb7f-8c98-4aac-831d-4290b13a37af)

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/f057cb51-05ad-4be5-8f47-ade851937a7b)

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/92ac30ae-0008-4782-a978-51a18375c6cf)

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/8d94b215-755f-4463-b31a-3e621c6c9737)


![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/149d2c19-839e-4036-9fcf-3a1504b31d9f)


![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/78a8a86f-59d3-478c-a43f-824bfef018b5)

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/d81a742e-ac55-4f8e-94b6-1d6756337d4f)

### employeesal.csv:

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/62ea18d6-80fe-4226-a2bf-e8ac7b7be70f)

![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/22ff195d-7803-4bb8-b327-75d552c0bc11)


![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/adbf097c-c021-4022-908f-c3560d4ef3d8)


![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/69709fbf-cb55-479c-9c2c-72998f2534da)


![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/622006e5-1c9d-4476-8b79-6d25cc3038c6)


![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/02b56aec-5b8f-4b85-b109-62fe7b327140)


![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/a05cd1a9-cbac-412c-879f-696686b088d4)




![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/95f17453-ae0b-4a2f-8630-06c03517c0f9)


![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/f4fe5542-468a-42b5-b0bb-9a1eef28d63f)


![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/57d88365-43f0-4a7a-a0b7-276cb5af4c44)


![image](https://github.com/Aravindsamy04/ODD2023-DataScience-Ex-03/assets/113497037/57275b31-53fa-4f65-aa89-3daa20daa89d)






RESULT:

Hence the univariate analysis is verified





