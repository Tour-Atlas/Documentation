# List Brands
This API will return a list of supplier brands and there internal id.  

The brand id is required when searching for tours.

## URL
https://\<your base URL\>/api

## Header parameters
**function**: 1

## Results 
```
{
  "result": bool, 
  "data": [
    {        
        "brandid": integer,            
        "brandname": string          
    }
  ]
}
```

The brands listed will depend on what you have selected via the Administration portal.
