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


## Supported Endpoints
- List Brands
- List age groups
- List group sizes
- List travel types
- List start locations
- Search for tours
- Get tour summaries
- Get tour details





