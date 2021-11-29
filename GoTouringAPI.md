[Go Touring](GoTouring.md)
# Go Touring API
## Overview
The Go Touring API is a set of API endpoints that allow for the online access of Go Touring data.  The endpoints are **not** a REST compliant interface .  THey are HTTPS endpoints that are licensed by URL and require the support of HTTP Headers to supply paramters.

## Security 
All requests must come from a predefined URL which is linked to your account.  Sub-pages under the pre-defined URl are supported.

## Support for development enviroments
Go Touring API supports the use of endpoints from a development enviroment.  You must provide the following Header keys with your HTTPS POSTS

**devmode**

Set this value to true

**sitebaseurl**

This is your base URL as defined on your account

**Please Note**:  In dev mode text valuesfield have there characters randomly replaced.

## Postman project
If you are using postman (https://www.postman.com/) you can use the following project file to test the API endpoints.
- [Postman project](Go_Touring_API.postman_collection.zip)

## Header Parameters
Depending on the API endpoint you will be required to provide HTTP Header values.  All endpoints require the following header parameter
**function**

This is a value from 1 to 8 which designates what request is being called

## Post results
As long as you supply the required paramters in the HTTP Header you will always get a value response from the API endpoint.

This response will be a JSON object with two fields.

**result**:  true or false.  Any false result means that while the POST worked then parameters were incorrect.  

**data**: This wil be a JSON object with the results from the call.  The exact results returned will depend on the function called.


## Supported Endpoints
- [List Brands](List_Brands.md).   
- [List age groups](List_Age_Groups.md).  
- [List group sizes](List_Group_Sizes.md).   
- [List travel types](List_Travel_Types.md).   
- [List start locations](List_Locations.md).   
- [Search for tours](Search_for_Tours.md).  
- [Get tour summaries](Get_Tour_Summaries.md).  
- [Get tour details](Get_Tour_Details.md).   





