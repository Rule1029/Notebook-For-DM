# Notebook-For-DM

### Iterate each columns in a row to find specific value

```
for index,row in corr_matrix['LOS'].iteritems():
    if(corr_matrix['LOS'][index] < 0.01):
        train_var = train_var.drop([index],axis=1)
        print(index, corr_matrix['LOS'][index])

### Iterate each columns to drop which has null value more than xxx

```
for index, row in train.iteritems():
    if(train[index].isnull().sum()>xxx):
        train = train.drop([index],axis=1)

### Drop those rows or columns which are all null values

```
train = train.dropna(axis=1, how='all') # by columns
train = train.dropna(axis=0, how='all') # by rows
