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
12. 
