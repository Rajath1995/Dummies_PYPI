How to use package

from Multiple_dummies import Mdummies

create an object of Mdummies and provide dataframe name and column name as arguments.

The various support format are :

For instance 

example 1 :host_verifications is a column with values  ['email', 'phone', 'reviews', 'kba'] and we need to create dummy column separately for each feature.

example 2 :amenites is  a column with values {TV,"Cable TV",Internet,"Wireless Internet"} and we need to create dummy column separately for each feature.

The above two senarious are examples where this package can be used to get dummy columns embeded with original dataframe for further applicaiton of machine learning.

Code to execute:

dummies=Mdummies(airbnb_seatle_lis,'amenities')

dummies.create_dummies()

The output will be the dataframe with all the dummy columns attached to the original dataframe and the original column with multiple values will be dropped.