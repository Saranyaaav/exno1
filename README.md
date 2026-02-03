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

science = pd.read_csv("/content/SAMPLEIDS.csv")
science
<img width="1315" height="697" alt="image" src="https://github.com/user-attachments/assets/f56e9277-c5d6-49cd-a70d-1a9090e5aef9" />
science.head()
<img width="954" height="211" alt="image" src="https://github.com/user-attachments/assets/10816be4-576d-42ab-a08e-5357d0f518fd" />
science.tail()
<img width="1206" height="205" alt="image" src="https://github.com/user-attachments/assets/4c6bfe5a-479e-4da7-82d0-c3f8e653d598" />


# Result
          <<include your Result here>>
