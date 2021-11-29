[Go Touring API](GoTouringAPI.md)

# Search for Tours
This API will return a list of tours that match the search parameter.   The tour information returned is very basic and allows for a level of sorting and filtering.


## URL
https://\<your base URL\>/api

## Header parameters
**function**: 6

**start_location**: One of the starting locations from the locations API. Text i.e Alice Springs

**travel_type**: One of the travel types from the API . i.e 0 = All types.

**SearchText**
**start_date**
**end_date**
**age_range**
**group_size**
**brands**
**price_min**
**price_max**
**days_min**
**days_max**






## Results 
```
{
  "result": bool, 
  "data": [
    string
  ]
}
```

The location returned are based on all the active tours in the database.

