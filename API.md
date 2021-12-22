# API interface documentation 

The short link can be generated in a programmable way by calling the API interface 

### Interface call address 

Self-deployed CloudFlare Worker address, for example: https://url.dem0.workers.dev or self-bound domain name

### Calling method: HTTP POST request format: JSON 
Example:
```
{
	"url": "https://example.com"
}
```

### Request parameters:

| Parameter name | Type | Description |Is it necessary|Example| 
| :----:| :----: | :----: | :----: | :----: |
| url | string | URL (must include http:// or https://) |Required|https://example.com| 

### Example response (JSON): 

```
{
    "status": 200,
    "key": "/demo"
}
```

### Response parameters:
| Parameter name | Type | Description | Example|
| :----:| :----: | :----: | :----: |
|status|int| Status code: 200 means the call is successful|200|
|key|string| Short link suffix: Need to add domain name prefix by yourself|/xxxxxx|

Note: The interface will only return the key value corresponding to the short link. In actual use, you need to add the corresponding domain name prefix. For example, if the key parameter returned in the example is "/demo", we need to add "https://url.dem0." Workers.dev" as the prefix, you can use it by completing it into a complete url, namely: https://url.dem0.workers.dev/demo 
