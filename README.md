# genesis-devops-shool-docker-workshop

### Get all events:
```
curl -X GET 'http://localhost:8080/api/v1/events
```
### Create an event:
```
curl -X POST \
  http://localhost:8080/api/v1/event \
  -H 'content-type: application/json' \
  -d '{
    "name": "Search",
    "description": "google",
    "slot": {
        "start_time": "2021-12-11T09:00:00+05:30",
        "end_time": "2021-12-11T15:00:00+05:30"
    },
    "website": "https://www.google.com/",
    "address": "Google corp"
}';
```

### DELETE event on id:

```
http://localhost:8080/api/v1/event?id=1655225549-0907818717-6730914582
```
