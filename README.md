# Task1
#1. Import dataset

import pandas as pd
df = pd.read_excel("Products_Sales_Data.xlsx")  

2. Remove duplicate values 

df_clean = df.drop_duplicates()

print(df_clean)

3. Converting YYYY-MM-DD to DD-MM-YYYY

df['Date'] = df['Date'].dt.strftime('%d-%m-%Y')
