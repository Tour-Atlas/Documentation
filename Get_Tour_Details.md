[Go Touring API](GoTouringAPI.md)

# Get Tour SDetails
This API will return the full details for a given tour id.


## URL
https://\<your base URL\>/api

## Header parameters
**function**: 8

**tourid**: integer ie. 87955

 
## Results 
```
{
  "result": bool, 
	"data": {
		"touritinerary_en": [
			{
				"itineraryid": integer,
				"title": string,
				"description": string
			}
		],
		"touritinerary_cn": [  -- Not used
			{
				"itineraryid": integer,
				"title": string,
				"description": string
			}
		],
		"symbol": string,
		"tourid": integer,
		"code": string,
		"numberofdays": integer,
		"rrp": decimal,
		"discount_rrp": decimal,
		"discount_price_label": string,
		"Price": string,
		"startcountry": string,
		"startcity": string,
		"endcountry": string,
		"endcity": string,
		"agemin": integer, -- 0 indicates avegare age using the agemax value
		"agemax": integer,
		"groupsizemin": integer,
		"groupsizemax": integer,
		"website": string,
		"january": false,
		"february": false,
		"march": false,
		"april": true,
		"may": true,
		"june": true,
		"july": true,
		"august": true,
		"september": true,
		"october": false,
		"november": false,
		"december": false,
		"mapid": integer, -- not used
		"companyid": integer,
		"style": integer,
		"physicality": integer,
		"title_en": string,
		"extra_en": string,
		"keywords_en": string,
		"inclusions_en": string,
		"title_cn": string,
		"extra_cn": string,
		"keywords_cn": string,
		"inclusions_cn": string,
		"CompanyName": string,
		"styledescription": string,
		"themenames": string,
		"isadvertisement": integer, -- not used
		"preferredprovider": integer, -- not used
		"includesflights": false,
		"jp_note": string, -- not used
		"jp_departure": null, -- not used
		"rrpperday": decimal,
		"mapurl": string,
		"brandname": string,
		"rrp_nz": decimal,
		"rrp_nzperday": decimal,
		"rrp_gb": decimal,
		"rrp_gbperday": decimal,
		"rrp_usd": decimal,
		"rrp_usdperday": decimal,
		"tourdepatures": [
			{
				"startdate": date, -- yyyy-MM-dd 
				"enddate": date, -- yyyy-MM-dd 
				"availability": string,
				"rrp": decimal,
				"base_rrp": decimal,
				"yesterday_rrp": decimal,
				"haschanged": true,
				"allowtosell": true
			}
		],
		"showagerange": bool,
		"images": string,
		"image_list": [
			string
		],
		"promotion_internaletitle": string,
		"promotion_internalenotes": string,
		"tour_type": string,-- not used
		"start_date": null,-- not used
		"end_date": null,-- not used
		"termsandconditions": null,-- not used
		"tourids": null,-- not used
		"product_type": string,
		"hero_image": string -- not used
	}
}
```

