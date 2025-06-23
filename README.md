# work-with-following-functions-in-series-and-data-frames-using-pandas

import pandas as pd

data={'Name':['alice','bob','charlie','david','eve'],

'Age':[25,30,35,40,28],

'Salary':[50000,60000,55000,70000,62000],

'Allowences':[2000,3000,2000,2000,4000]

}

df=pd.DataFrame(data)

print("sorts by a column:\n",df.sort_values('Salary',ascending=True))

print("sorts by multiple columns:\n",df.sort_values(['Salary','Name']))

print("sets a column as index:\n",df.set_index('Age'))

print("resets index:\n",df.reset_index())

O/P:

sorts by a column:

Name Age Salary Allowences

0 alice 25 50000 2000

2 charlie 35 55000 2000

1 bob 30 60000 3000

4 eve 28 62000 4000

3 david 40 70000 2000

sorts by multiple columns:

Name Age Salary Allowences

0 alice 25 50000 2000

2 charlie 35 55000 2000

1 bob 30 60000 3000
4 eve 28 62000 4000

3 david 40 70000 2000

sets a column as index:

Name Salary Allowences

Age

25 alice 50000 2000

30 bob 60000 3000

35 charlie 55000 2000

40 david 70000 2000

28 eve 62000 4000

resets index:

index Name Age Salary Allowences

0 0 alice 25 50000 2000

1 1 bob 30 60000 3000

2 2 charlie 35 55000 2000

3 3 david 40 70000 2000

4 4 eve 28 62000 4000# Work-with-following-functions-in-series-and-data-frames-using-pandas
