# Go Touring API
## Overview
The Go Touring API is a set of API endpoints that allow for the online access of Go Touring data.  The endpoints are **not** a REST compliant interface .  THey are HTTPS endpoints that are licensed by URL and require the support of HTTP Headers to supply paramters.

## Security 
All requests must come from a predefined URL which is linked to your account.  Sub-pages under teh pre-defined URl are supported.

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

## Supported Endpoints
- [List Brands](List_Brands.md).  Function: 1
- List age groups.  Function: 2
- List group sizes.  Function: 3
- List travel types.  Function: 4
- List start locations.  Function: 5
- Search for tours.  Function: 6
- Get tour summaries.  Function: 7
- Get tour details.  Function: 8





