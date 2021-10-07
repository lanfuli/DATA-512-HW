# DATA-512-HW

A1: Data Curation Assignment

# Goal:
To construct, analyze, and publish a dataset of monthly traffic
on English Wikipedia from Dec. 1 2007 through Sept. 30 2021.

Use API:
https://wikimedia.org/api/rest_v1/#/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end
https://wikimedia.org/api/rest_v1/#/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end

Refer code link:
https://public.paws.wmcloud.org/User:Jtmorgan/data512_a1_example.ipynb
https://public.paws.wmcloud.org/User:Jtmorgan/data512_a1_example.ipynb?format=raw

# Step 1 Data Acquisition
a. Connect two wikimedia apis(legacy pagecounts and pageview) start from 2007/12 to 2021/09

b. Legacy page count data comes from old api start from 2007/12 to 2016/07

c. Page view data comes from the new api start from 2015/01 to 2021/09

d. Call these two apis, get the 5 separate JSON and one file per API query type

e. The new api comes with a agent filter, so we need to filter user only to avoid third party misuse


# Step 2: Data Processing
a. We need to convert all json data type to list data type 

b. Create dataframe for each list data 

c. Combine all of dataframe into one dataframe

d. Export a csv file


# Step 3: Graph and analysis
a. There are one year overlap from 2015/07 to 2016/07 between two api

b. Choose pageview_all_views(new api data) for this overlapping period time due to the agent can filter user 

c. Choose the pagecount_all_views data(old api data) from  2007/12 to 2015/05, pageview_all_views from 2015/07 to 2021/09

d. create two dataframes(pagecount and pageview), then combine them together

e. Plot the dataframe by using pandas build in tool
