# List Age Groups
This API will return a list of age group and their internal id.  



## URL
https://\<your base URL\>/api

## Header parameters
**function**: 4

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

The age group id is required when searching for tours.