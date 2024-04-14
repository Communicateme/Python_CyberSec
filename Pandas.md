1. df=pd.read_table('https[:]//link to the .TSV file') ----> for reading/loading the data from URL if the raw data is in Tabs Seperated Value format.
2. df=pd.read_table('https.....com', sep='|', header=None, names=user_cols) ---> for reading the data which has values seperated by pipe "|". Also it tells that file has no header and names of the columns is under the list 'user_cols'
   user_cols = ['Name','age','surname'] ---> List of user's name used above.
3. **"Series"** --- 1d Array or the Row of a dataframe
**   "Dataframe"** --- 2d Array or the table.
4. **type(df)** = pandas.core.frame.DataFrame --- tells the type of Data Frame
5. **df.shape **-- provides the size of the table in the formt - (#rows, #columns)
6. df.head() -- present top 5 rows from Tbale.
7. df.describe() -- provides statistics values for numberical column
8. df.dtypes -- provides data types of columns
9. df.rename(coulmns = {'Name':'stunden_name',"age'='student_age'}) -- for renaming the columns in tables
10. List=['City','colors_reported','state']
    df.columns =  List --- this will change the cloumns name.
11. df = df.columns.str.replace('-','_') -- replaces the dash with backslash in columns name.
12. df.drop('Name', axis=1, inplace=True) -- Remove the column called name from Table. ***"axis=1" means Column | "axis=0" means Rows***
13. df.drop(['Name','age',], axis=1, inplace=True) -- Remove multiple columns
14. df.drop(([0,1], axis=0, inplace=True) -- Remove row from index 0 & 1.
15. df.sort_values('Name', ascending=false) -- sort the column to decending order. Default is ascending
16. **Filtering**
 - https://youtu.be/2AFGPdNn4FM?list=PL5-da3qGB5ICCsgW1MxlZ0Hq8LL5U3u9y&t=606
 - https://youtu.be/YPItfQ87qjM?list=PL5-da3qGB5ICCsgW1MxlZ0Hq8LL5U3u9y&t=375
 - https://youtu.be/YPItfQ87qjM?list=PL5-da3qGB5ICCsgW1MxlZ0Hq8LL5U3u9y&t=542
17. import pandas as pd - # Assuming df is your DataFrame and 'url' is your column with URLs
mask = df['url'].str.contains('microsoft.com')
filtered_df = df[mask]

