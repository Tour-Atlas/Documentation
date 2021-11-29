[Go Touring API](GoTouringAPI.md)

# List Groups Sizes
This API will return a list of Group sizes.  


## URL
https://\<your base URL\>/api

## Header parameters
**function**: 5

## Results 
```
{
  "result": bool, 
  "data": [
    {        
        "id": integer,            
        "description": string          
    }
  ]
}
```

The group size id is required when searching for tours.