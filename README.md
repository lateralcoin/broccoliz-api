# Broccoliz<sup>&reg;</sup> (BZ 2.0): Rest API Documentation for Institutional Investors
**Warning**: Broccoliz (BZ 2.0) is a trading algorithm developed by LateralCoin Limited (Singapore) for INSTITUTIONAL use ONLY. **Broccoliz (BZ 2.0) is NOT for sale**. Beware of scams using the name of our company, algorithms or developers. 
<hr />

## Rest API for Broccoliz<sup>&reg;</sup> BCZ 2.0 (2021-01-29)

### General API Information
* The base endpoint is: **https://api.lateralcoin.com/broccoliz/api**
* If there are performance issues with the endpoint above, these API clusters are also available:
  * **https://api1.lateralcoin.com/broccoliz/api**
  * **https://api2.lateralcoin.com/broccoliz/api**
  * **https://api3.lateralcoin.com/broccoliz/api**
* All endpoints return either a JSON object or array.

### HTTP Return Codes

* HTTP `4XX` return codes are used for malformed requests;
  the issue is on the sender's side.
* HTTP `403` return code is used when the WAF Limit (Web Application Firewall) has been violated.
* HTTP `429` return code is used when breaking a request rate limit.
* HTTP `418` return code is used when an IP has been auto-banned for continuing to send requests after receiving `429` codes.
* HTTP `5XX` return codes are used for internal errors; the issue is on
  LateralCoin's side.
  
## General Information on Endpoints
* For `GET` endpoints, parameters must be sent as a `query string`.
* Parameters may be sent in any order.

 ## Endpoint Security Type
 * Each endpoint has a security type that determines the how you will interact with it.
 * API-keys are passed into the Rest API by sending an `api_key` parameter via the query string.
 * API-keys and Secret-keys are **case sensitive**.
 
Security Type | Description
------------ | ------------
NONE | Endpoint can be accessed freely.
APIKEY_ONLY | Endpoint requires sending a valid `API-Key`.
SIGNED | Endpoint requires sending a valid `API-Key` and `Signature`.
 
 
 
 
 
 
 
 
  
  
