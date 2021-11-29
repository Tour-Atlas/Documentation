[Go Touring API](GoTouringAPI.md)

# Search for Tours
This API will return a list of tours that match the search parameter.   The tour information returned is very basic and allows for a level of sorting and filtering.


## URL
https://\<your base URL\>/api

## Header parameters
**function**: 6

**start_location**: One of the starting locations from the locations API. Text i.e Alice Springs

**travel_type**: One of the travel types from the API . i.e 0 = All types.

**SearchText**: Text used for the search.  If the words are surrounded by double quotes the search is a phase search i.e. Lakes or "Salt Lakes"

**start_date**: Date used for departure start filter. Start dates greater to or equal to this date will be returned. Date format must be yyyy-MM-dd

**end_date**: Date used for departure start filter.  Start dates less than or equal to this date will be returned. Date format must be yyyy-MM-dd

**age_range**:  One of the age range id from the API .

**group_size**:  Group size ID from the API.

**brands**: An array of brand id's .  Tours will be return from these brands.

**price_min**: Min price of tours, use 0 as default.

**price_max**: Max price for tours, use 999999 as default.

**days_min**: Min number of days for a tour, use 0 as default.

**days_max**: Max number of days for a tour, use 999999 as default.



## Results 
```
{
  "result": bool, 
  "data": [
    {
		"tourid": integer,
		"rrp": decimal,
		"days": integer,
		"rank": integer (Larger the number the better the match),
		"isnew": integer (0 or 1)
	}
  ]
}
```

This API will return an array of all matched tours.  Use this array to sort your results.  Call the Get Tour Summary API to get the summary listing for a group of tours. 

