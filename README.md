# DATA-512-HW
# Step 1 Data Acquisition
a. Connect two wikimedia apis start from 2007/12 to 2021/09
b. Legacy view data comes from old api start from 2007/12 to 2016/07
c. Page view api comes from the new api start from 2015/01 to 2021/09
d. Call these two api, get the data and save to json file

# Step 2: Data Processing
a. convert all json to list type 
b. create dataframe for each json
c. combine all of them into one dataframe
d. export into a csv file

# Step 3: Graph and analysis
a. there are one year overlap from 2015/07 to 2016/07 between api
b. choose pageview_all_views(new api data) for this period time due to the agent can choose user
c. choose the pagecount_all_views data from  2007/12 to 2015/05, pageview_all_views from 2015/07 to 2021/09
d. create two dataframes(pagecount and pageview), then combine them together then plot
