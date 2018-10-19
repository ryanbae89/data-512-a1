# data-512-a1

UW DATA512 Fall 2018 assignment 1 repo

Creator: Ryan Bae

Date: October 18th, 2018

## Goal
The goal of this project is to perform an exercise in data curation and analysis reproducibility by obtaining data from Wikimedia's API to download monthly Wikipedia page views data and generate a plot. The idea is that any user can look at this repo and reproduce the results from this exercise without difficulty. 

## Final Data Schema
Final `en-wikipedia_traffic_200712-201809.csv` file  has the following schema:

* year (int)
* month (int)
* pagecount_all_views (int)
* pagecount_desktop_views (int)
* pagecount_mobile_views (int)
* pageview_all_views (int)
* pageview_desktop_views (int)
* pageview_mobile_views (int)

## Data Considerations
There are few considerations to take into account when reproducing the results. There are some differenes between the two API's used to obtain the data.

* **Legacy Pageview API Data**
  * Includes web spiders/crawlers

* **Current Pagecounts API Data**
  * Does not include web spiders/crawlers
  * Further divides mobile data into mobile-app and mobile-web data

## API Documentation

Also look at the following resources for API documentation:

[Wikimedia REST API](https://www.mediawiki.org/wiki/REST_API)

[Legacy Pagecounts API Documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts)

[Legacy Pagecounts API Endpoint](https://wikimedia.org/api/rest_v1/#!/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end)

[Pageviews API Documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews)

[Pageviews API Endpoint](https://wikimedia.org/api/rest_v1/#!/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end)

## License/Terms of Use and Documentation

When reproducing the results, please take a look at the following link terms of use information:

[Wikimedia Terms of Use](https://foundation.wikimedia.org/wiki/Terms_of_Use/en)

The content accessed via Wikimedia's API is licensed under the [CC-BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) and [GFDL](https://www.gnu.org/copyleft/fdl.html) licenses, and you irrevocably agree to release modifications or additions made through this API under these licenses.
