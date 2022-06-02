# Goolge Logging



# QuickStart using Logging Tools

- Write log entries by using the Google Cloud CLI.
- List log entries by using the gcloud CLI.
- List log entries by using the Logging API.
- View and query log entries by using the Logs Explorer.
- Clean up
## Write log entries by using the Google Cloud CLI.

```bash
gcloud logging write my-test-log "A simple entry."

gcloud logging write --payload-type=json my-test-log '{ "message": "My second entry", "weather": "partly cloudy"}'
```

## List log entries by using the gcloud CLI.

```bash
gcloud logging read "resource.type=global"
```

```yaml
---
insertId: 1j7z2nmfw6454l
logName: projects/sign-in-21-ccf/logs/my-test-log
receiveTimestamp: '2022-05-17T02:11:07.355586874Z'
resource:
  labels:
    project_id: sign-in-21-ccf
  type: global
textPayload: A simple entry.
timestamp: '2022-05-17T02:11:07.355586874Z'
```

## List log entries by using the Logging API.

*request*
```json
{
  "resourceNames": [
    "projects/sign-in-21-ccf"
  ],
  "filter": "resource.type=global",
  "orderBy": "timestamp desc"
}
```

*response*
```json
{
  "entries": [
    {
      "textPayload": "A simple entry.",
      "insertId": "1j7z2nmfw6454l",
      "resource": {
        "type": "global",
        "labels": {
          "project_id": "sign-in-21-ccf"
        }
      },
      "timestamp": "2022-05-17T02:11:07.355586874Z",
      "logName": "projects/sign-in-21-ccf/logs/my-test-log",
      "receiveTimestamp": "2022-05-17T02:11:07.355586874Z"
    }
  ],
  "nextPageToken": "EAE4oIeKpdvUg9UtShQiEiICCgAqDAj_0d-TBhD_k-vcA1IHCM3zmbO5HmD4s9-JtuLswukBahwKDAitioyUBhChitmXAxIICAUQrMi83QEYASAA"
}
```

## View and query log entries by using the Logs Explorer.

Go to Logs Explorer

## Clean up

```bash
gcloud logging logs delete my-test-log
```

