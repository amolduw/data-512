# Data 512A course assignment A1 

This readme file provides step by step instructions for Data 512A course A1 assignment  to construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from January 1 2008 through August 30 2020. 

**Project goal:**

The goal of this project is to construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from January 1 2008 through August 30 2020. 

**Data Source:**

In order to measure Wikipedia traffic from 2008-2020, we collected data from two different API endpoints, the Legacy Pagecounts API and the Pageviews API.

The Legacy Pagecounts API ([endpoint](https://wikimedia.org/api/rest_v1/#!/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end), [documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts))

The Pageviews API ([endpoint](https://wikimedia.org/api/rest_v1/#!/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end), [documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews))

Wikimedia Foundation REST API terms of use: https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions 

**Data Fields in final processed file:**

Combine all data into a single CSV file with the following headers:

Column     Value

| Column | Value |
| ------ | ------ |
| year | YYYY |
| month | MM |
| pagecount_all_views | num_views |
| pagecount_desktop_views | num_views |
| pagecount_mobile_views | num_views |
| pageview_all_views | num_views |
| pageview_desktop_views | num_views |
| pageview_mobile_views | num_views |
| month | num_views |


**Special Considerations:**
- Data from the Pageview API excludes spiders/crawlers, while data from the Pagecounts API does not.
- There is about 1 year overlap between Pageview API and Pagecounts API

**Analysis Reproduction steps:**
Analysis steps are detailed documented in Jupyter notebook for better understanding alongwith code. At high level below steps were followed.
- Gathering the data
- Processing the data
- Analyzing the data (Explore and Visualize)
- Document the process






