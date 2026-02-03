# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
```
import pandas as pd
```
```
science = pd.read_csv("/content/SAMPLEIDS.csv")
science
```
<img width="1315" height="697" alt="image" src="https://github.com/user-attachments/assets/f56e9277-c5d6-49cd-a70d-1a9090e5aef9" />

```
science.head()
```
<img width="954" height="211" alt="image" src="https://github.com/user-attachments/assets/10816be4-576d-42ab-a08e-5357d0f518fd" />

```
science.tail()
```
<img width="1206" height="205" alt="image" src="https://github.com/user-attachments/assets/4c6bfe5a-479e-4da7-82d0-c3f8e653d598" />

```
science.info()
```
<img width="659" height="344" alt="image" src="https://github.com/user-attachments/assets/4871907a-d2e9-48a3-8ec8-83982ff870cc" />

```
science.describe()
```
<img width="1022" height="296" alt="image" src="https://github.com/user-attachments/assets/75139492-4985-47dd-9226-e74e9dceb078" />

```
science.isnull()
```
<img width="978" height="664" alt="image" src="https://github.com/user-attachments/assets/e8cbcd8e-2194-47e4-9d7b-48ff8efd313d" />

```
science.notnull()
```
<img width="981" height="668" alt="image" src="https://github.com/user-attachments/assets/b808295d-9592-46b6-b598-89f549bed4b8" />

```
science.isnull().sum()
```
<img width="228" height="421" alt="image" src="https://github.com/user-attachments/assets/d310a2e0-0d91-46f8-a57c-0ff35650feaa" />

```
science.isnull().any()
```
<img width="349" height="425" alt="image" src="https://github.com/user-attachments/assets/6a2a6504-9a12-42cf-a1ef-e1fd64522e9a" />

```
science.dropna()
```
<img width="941" height="422" alt="image" src="https://github.com/user-attachments/assets/21a0dd42-b387-438c-9868-76415097f32c" />

```
science.dropna(axis=1)
```
<img width="363" height="658" alt="image" src="https://github.com/user-attachments/assets/4e2337a8-3eef-4b3a-b2ff-ffa5265bf191" />

```
science.fillna(5)
```
<img width="945" height="657" alt="image" src="https://github.com/user-attachments/assets/4805ba61-cd37-4777-9897-0cee40615525" />

```
science.fillna(method='ffill')
```
<img width="1282" height="683" alt="image" src="https://github.com/user-attachments/assets/a8269a05-2b38-4bb3-9a19-6af8b2d84c2d" />

```
science.fillna(method='bfill')
```
<img width="1278" height="684" alt="image" src="https://github.com/user-attachments/assets/dc43cde6-bda7-414a-be9f-455cb7e99810" />

```
num = pd.read_csv("/content/iris.csv")
num
```
<img width="640" height="383" alt="image" src="https://github.com/user-attachments/assets/ea958124-e400-4e7c-976e-46bc091566af" />

```
num.head()
```
<img width="608" height="186" alt="image" src="https://github.com/user-attachments/assets/960860dd-899e-4aa6-bd1a-343cda681492" />

```
num.tail()
```
<img width="641" height="186" alt="image" src="https://github.com/user-attachments/assets/48e0597b-3624-469e-b26b-a2b9668b5eaa" />

```
num.info()
```
<img width="513" height="200" alt="image" src="https://github.com/user-attachments/assets/00798fbf-06f2-4dd7-8277-f7473e2d5f46" />

```
num.describe()
```
<img width="565" height="276" alt="image" src="https://github.com/user-attachments/assets/af030ed9-6fda-4360-af78-7b0e77b357cf" />

```
num.isnull().sum()
```
<img width="218" height="221" alt="image" src="https://github.com/user-attachments/assets/dcbb1ada-5261-492d-b881-19da637873d0" />

```
num.isnull()
```
<img width="671" height="389" alt="image" src="https://github.com/user-attachments/assets/b7dd3dc1-a50d-4674-99a3-69c3c70ecd6d" />

```
num.isnull().any()
```
<img width="298" height="221" alt="image" src="https://github.com/user-attachments/assets/447118ba-0a3a-4c05-88b9-5722873749ee" />

```
num.notnull()
```
<img width="615" height="393" alt="image" src="https://github.com/user-attachments/assets/7a0f0a28-6eb4-4e31-be0f-28c79aed13db" />

```
num.dropna()
```
<img width="822" height="397" alt="image" src="https://github.com/user-attachments/assets/cc702d40-138a-441c-b0af-6e717acf6177" />

```
num.dropna(axis=1)
```
<img width="741" height="390" alt="image" src="https://github.com/user-attachments/assets/c06fcd8c-58b0-4098-8acf-065e9325641f" />

```
num.fillna(2)
```
<img width="929" height="398" alt="image" src="https://github.com/user-attachments/assets/74661dd4-bbdc-4200-9cda-7736e141b92e" />

```
num.fillna(method='ffill')
```
<img width="1380" height="423" alt="image" src="https://github.com/user-attachments/assets/b12959e2-fa50-439f-92fe-cf10a284989a" />

```
num.fillna(method='bfill')
```
<img width="1402" height="424" alt="image" src="https://github.com/user-attachments/assets/aefe1600-29e1-471e-ae40-2bcf0cd6b642" />

```
import seaborn as sns
```
```
sns.boxplot(x='sepal_width',data=num)
```
<img width="530" height="425" alt="image" src="https://github.com/user-attachments/assets/5374da47-66ed-419e-9c9a-f315d4f569b7" />

```
Q1 =num.sepal_width.quantile(0.25)
Q3 = num.sepal_width.quantile(0.75)
(IQR)=Q3-Q1
print(IQR)
```
<img width="966" height="20" alt="image" src="https://github.com/user-attachments/assets/a5d5a4ec-c0b0-423f-93ff-b29fd9dac67e" />

```
ran = num[((num.sepal_width<(Q1-1.5*IQR))|(num.sepal_width>(Q3+1.5*IQR)))]
ran['sepal_width']
```
<img width="711" height="193" alt="image" src="https://github.com/user-attachments/assets/102fba93-6c66-4938-869a-b30edb534a0f" />

```
ran = num[~((num.sepal_width<(Q1-1.5*IQR))|(num.sepal_width>(Q3+1.5*IQR)))]
ran['sepal_width']
```
<img width="309" height="422" alt="image" src="https://github.com/user-attachments/assets/eb4246c9-5d0d-457c-9be8-fb09ab981ec5" />

# Result
Thus, the program is executed successfully.
