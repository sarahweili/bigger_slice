# BiggerSlice - Insight DE Project
*how to get a bigger slice of market in restaurant industry?*

## Problem
Competition in restaurant industry is very fierce. There are about 1 million restaurants in the US, with 60 thousands openings and 50 thousands closing every year. So it is very important for restaurateurs to know who they are competing with and how they are doing. However, internal data is usually hard to locate.

## Proposed Solution
Built a data pipeline for restaurant competitor analysis by integrating alternative data sources.
![solution](/img/solution.jpg)

## Data Sources (key attributes are listed)
- [Yelp Open Dataset](https://www.yelp.com/dataset)
	- Business
		- name
		- latitude
		- longtitude
		- address
		- postal_code
		- state
		- starts
	- Review
		- text
- [SafeGraph Dataset](https://www.safegraph.com/covid-19-data-consortium)
    - Core places
    	- location_name
    	- naics_code
    	- latitude
    	- longitude
    	- postal_code
    	- region
    	- category_tags
    - Monthly place pattern (foot traffic)
    	- raw_visit_counts: Number of visits to the POI during the date range.
    	- visitor_home_cbgs: A mapping of census block groups to the number of visitors to the POI whose home is in that census block group.

## Database Schema
![schema](/img/schema.jpg)

## Data Pipeline
![pipeline](/img/pipeline.jpg)


