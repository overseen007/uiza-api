# Uiza 5.1.0 Document Guideline

**Version Highlight**

This version Release the new Live Stream with bringing the

**Intuitive:** it's just worked to bring you to the first feeling about the Uiza quickly, to reduce the time on investigating and find in a large information.

**Reliability:** we focus on stability with clear product specifications, to make sure that you can trust 100% percent when using the Uiza

**Scalability:** unpredictable about your product plan is not a problem, we provide the scaleability automatically to keep the product always on 

>So with the new definition, there's a new meaning about the event 

**Entity (id):** the event is created at the beginning, and there's only 2 status

| Status       |      Meaning    |  
| ------------- | ----------- | 
|  **init**     | The event has been created and still waiting for the resource allocated |
| **ready**  | The event is ready to stream |

```json
{
    "id": "9902dbe5-75a8-4bb0-a4a5-4deef6e88295",
    "user_id": "uiza",
    "app_id": "uiza",
    "name": "Test Event",
    "description": "Event for Test",
    "region": "asia-southeast-1",
    "status": "init",
    "created_at": "2019-10-03T11:22:14Z",
    "updated_at": "2019-10-03T11:22:14Z"
}
```

> When an entity changed to ready, you can send the input signal anytime, and every time you send, it'll create a session

**Session:** created right after you send the input signal & end right after to stop the capturing software
When you stop the Signal on the Capture software, the session will auto update the Live Duration

```json
  {
    "data": [
        {
            "id": "ce69f971-9895-4d82-9424-a45290f41c0f",
            "entity_id": "e11ed326-0237-4e09-9a24-60d5682fa5b6",
            "stream_key": "live_2Zk0F0ocLW",
            "created_at": "2019-10-03T11:53:58Z",
            "updated_at": "2019-10-03T11:53:58Z"
        },
        {
            "id": "781027f5-fe34-4e7d-8955-6e5c05d22fa9",
            "entity_id": "e11ed326-0237-4e09-9a24-60d5682fa5b6",
            "stream_key": "live_2Zk0F0ocLW",
            "created_at": "2019-10-03T11:37:35Z",
            "updated_at": "2019-10-03T11:37:35Z"
        },
        {
            "id": "90978e32-8fd6-479b-b6e9-4846e35bc60b",
            "entity_id": "e11ed326-0237-4e09-9a24-60d5682fa5b6",
            "stream_key": "live_2Zk0F0ocLW",
            "created_at": "2019-10-03T11:32:26Z",
            "updated_at": "2019-10-03T11:32:26Z"
        }
    ],
    "total_records": 3
}

