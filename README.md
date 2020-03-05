# Notebook-For-DM

### Iterate each colums in a row to find specific value

```
for index,row in corr_matrix['LOS'].iteritems():
    if(corr_matrix['LOS'][index] < 0.01):
        train_var = train_var.drop([index],axis=1)
        print(index, corr_matrix['LOS'][index])

```
