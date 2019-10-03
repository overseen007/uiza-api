# Sample Use Case


**Step 1** - Use API to Create an event

cURL
```json
POST /api/v5/live/entities HTTP/1.1
Host: https://v5.dev.uizadev.io
Content-Type: application/json
Postman-Token: bdb18545-136c-4682-825b-bafa24c9c9b9,73388e62-e49c-4e55-ae78-7cd98d1b9329
cache-control: no-cache,no-cache
User-Agent: PostmanRuntime/7.17.1
Accept: */*
Host: 18.139.66.78:8080
Accept-Encoding: gzip, deflate
Content-Length: 181
Connection: keep-alive
 
{
    "name": "Yann event",
    "region": "asia-southeast-1",
    "description": "Event for Test",
    "app_id": "uiza",
    "user_id": "uiza"
}
```

**Step 2** - Get the Stream key & Stream URL