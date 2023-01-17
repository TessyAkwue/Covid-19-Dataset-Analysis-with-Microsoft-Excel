# Project Name: Covid-19-Dataset-Analysis-with-Microsoft-Excel
 ![image](https://user-images.githubusercontent.com/102609359/212904621-63c5b5eb-ec73-49f1-b7d9-75c98fd952cd.png)

Covid 19 is an infectious disease caused by SARS-CoV-2 virus.This can cause mild to severe respiratory illness, including death.

---
# Project Objective: Problem Statment
Covid 19 has led to great loss of lives around the world, therefore the aim of this project is to drive insights using the dataset to visualize its impact around the globe. In the process of ascertaing the cases confirmed, recovered and deaths, with the countries that were mostly affected, its impacts can be measured.

---
# Data Souring
The Covid 19 Dataset was gotten from github through web scrapping. Microsoft Excel has a feature that allows one to import a data frpm the web.
The global confirmed cases was imported into Excel using the URL address of the web page. This was done taking the folling steps:

Clicked on the time series covid 19 confirmed global csv file
![2](https://user-images.githubusercontent.com/102609359/212884943-b154e507-de19-4327-a57d-f212e8677f76.png)

Clicked on View raw
![3_LI](https://user-images.githubusercontent.com/102609359/212885222-604b4124-ede0-4547-9f93-d73a61e71392.jpg)

Copied the URL address
![4](https://user-images.githubusercontent.com/102609359/212885902-72730c57-d434-4e89-8b46-f2fdc15aa204.png)


Then i went to my opened Microsoft Excel sheet and clicked on the data tab, followed the steps in the below image and clicked on 'From web'
![5b](https://user-images.githubusercontent.com/102609359/212886435-a2c4f7b6-6d42-4761-8c8e-505818f7b180.png)

Pasted the URL address and clicked OK.
![6b](https://user-images.githubusercontent.com/102609359/212886612-2fb568b1-4018-4d85-98e6-eacee47693f1.png)

Click on Transform data
![7](https://user-images.githubusercontent.com/102609359/212888099-86dff8d5-9d8d-42ff-bf0a-f97315d8ce31.png)

This took me to Power Query Editor, where i transformed my data.

---
# Data Transformation
This is the point where the dataset was cleaned. 
![8](https://user-images.githubusercontent.com/102609359/212888825-4ff817cb-c73b-4835-9e1b-b7ef2fa6e703.png)

 # The follwing steps were taken to transform the dataset.
1. All firt rows were upgraded to headers, by clicking on the table icon on the left hand side to select 'use fist row as hearders'
![8b](https://user-images.githubusercontent.com/102609359/212889859-a997c2ca-0734-44c2-9985-92ed1faf2aec.png)

2. Went to 'source' and deleted the number of 'columns'from the formula bar. This was to enable refreshing of the data in real time.
![9_LI](https://user-images.githubusercontent.com/102609359/212891243-b646bb4e-03af-405e-abd1-dc82ed183624.jpg)

3. Renamed the time series table to confirmed cases
![9b](https://user-images.githubusercontent.com/102609359/212891956-e5be8b86-8f85-4687-8843-886793f492a7.png)

4.The data format was changed from wide to long data by unpivoting the date columns.This was done by holding down the 'control' key to select the column of interest and then right click and select 'unpivot other columns'.
![10](https://user-images.githubusercontent.com/102609359/212892985-3ee383a4-241f-4c60-99ac-11be29586148.png)

5. Renamed the Attribute and Value columns to Date and Confirmed cases respectively. The data types were changed.
![10b](https://user-images.githubusercontent.com/102609359/212893448-ed1c1a66-a8b8-4825-86fe-780f994f26d2.png)

6. The confirmed cases table was duplicated twice and renamed to death and recovered cases.
![11](https://user-images.githubusercontent.com/102609359/212894141-04526642-bf92-4a84-908f-3a309bea602e.png)

7. To repeat the above steps for death and recovered cases respectively, click on source settings
![12_LI](https://user-images.githubusercontent.com/102609359/212895257-dfb783d9-4dca-4203-944b-000fef433dd1.jpg)
A comma separated box will pop up, then delete the former url and paste the url for death or recovered cases, then click ok.
![12b](https://user-images.githubusercontent.com/102609359/212895741-cc0914d3-b24e-47a1-99a7-70426068ca53.png)

After applying the same transformation to death and recovered cases respectively, the three tables were merged as one ( named 'ConsolidatedData') and returned to Excel.
8. Go to the 'confirmed cases' table and choose "Merge Queries as New"
![13](https://user-images.githubusercontent.com/102609359/212897154-fbfc2a6d-1b74-469d-b01c-da4334c31878.png)
![14b](https://user-images.githubusercontent.com/102609359/212897239-66a2a71c-bce1-4e64-9abc-e345d88022a5.png)

Below is how the transformed data appeared before returning to Excel.
![15](https://user-images.githubusercontent.com/102609359/212897300-6d2f7f17-c639-45ea-8c05-8768f709d7ab.png)

The date column was expanded into 'year', 'month' and 'day' columns using Excel text functions before the data was summarized using pivot table.
![17](https://user-images.githubusercontent.com/102609359/212898729-adec7a5f-3b41-43c9-8221-4ba8eaa71f58.png)

---

# Data Visualization
The dataset was visualized using pivote tables and pivot charts. Adashboard was created by bringing together relevant charts and tables that gave insights on th data set.
Below is the visualized board.
![DB1](https://user-images.githubusercontent.com/102609359/212900235-fcd706b6-0d15-4b4e-a478-55dd640c2ed1.png)
![DB2](https://user-images.githubusercontent.com/102609359/212900281-01c0ec56-2923-4203-851f-bf3e04f9ddc4.png)

---
# Findings 

It was observed that covid 19 virus led to a great loss of lives around the globe and recognized as a highly infectious disease as seen in the number of toatl confirmed cases. More than  3 billion lives was lost as a result of this virus. About 23 billion of confiremed cases were recovered; this could be as a result of the medical intervention and care that was given to the patients.
The Top 5 countires that were greatly affected were: US, India, Brazil, France and United Kingdom while North Korea,Tuvalu, Antartica, MS Zaanadam and Holy See are countries with lowest prevalence.

---
# Recommendation
More cases are yet to be recovered as this can be seen in the number gap between confirmed and recovered cases.
Therfore more medical interventions, vaccine production and research should be carried out and made accessible to help curb and eradicate the prevalence of covid 19. Looking at the great number of confirmed cases, more experienced medical personnels should be employed, as they are needed to assist in the medicalcare and proper administration of medical intervention. 

