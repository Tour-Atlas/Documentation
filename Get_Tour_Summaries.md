[Go Touring API](GoTouringAPI.md)

# Get Tour Summarys
This API will return a list of summary tour details for the provided arrray of tourid's.   The tour information returned is basic is used to fill a results page of the search.


## URL
https://\<your base URL\>/api

## Header parameters
**function**: 7

**tours**: csv of toruid's ie. 87955,87962

Note:  Faster results are returned for fewer tourid's.  Try and restrict calls to 30 or less tourid's.

## Results 
```
{
  "result": bool, 
  "data": [
    {
		"duration": integer,
		"rank": integer,
		"num_reviews": integer,
		"country_code": string,
		"isnew": bool,
		"agemin": integer,
		"agemax": 3integer,
		"groupsizemin": integer,
		"groupsizemax": integer,
		"ja_show": bool,
		"discount_rrp": decimal,
		"discount_price_label": string,
		"promotion_internaletitle": string,
		"promotion_internalenotes": string,
		"tourid": integer,
		"code": string,
		"numberofdays": integer,
		"rrp": decimal,
		"mapurl": string,
		"january": bool,
		"february": bool,
		"march": bool,
		"april": bool,
		"may": bool,
		"june": bool,
		"july": bool,
		"august": bool,
		"september": bool,
		"october": bool,
		"november": bool,
		"december": bool,
		"includesflights": bool,
		"startcity": string,
		"endcity": string,
		"title": string,
		"preferredprovider": integer, -- not used
		"companyname": string,  -- Brand name
		"startcountry": string,
		"endcountry": string,
		"style": string,
		"physicality": integer,
		"isadvertisement": integer, -- not used
		"themenames": null,  -- not used
		"description": null,  -- not used
		"tourimage": csv string of URL's,
		"tour_type": string,
		"from_price": "$3,285",
		"start_location": string,
		"end_location": string,
		"physicality_string": string,
		"RRP_Price": string, -- Formatted dollar amount
		"Price": string, -- Formatted dollar amount will any discounts applied
		"totalfound": integer
	}
  ]
}
```

