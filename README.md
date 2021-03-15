# Sample API Docs.
sample_api_docs


## Avalible API's

### Login API

##### Request Info
`POST` : `http://localhost:8000/v1/login/`

##### Request Headers
```json {"Content-type": "application/json"} ```

##### Request Response
```json
{
  "status": true,
  "payload": [
    {
      "_id": 1,
      "name": "NAME",
      "email": "EMAIL",
      "token": "GENERATED_USER_TOKEN",
      "_created": "2021-03-14 12:32:59.998882",
      "_updated": "2021-03-14 12:32:59.998909"
    }
  ],
  "message": "Login Api view"
}
```

##### Error Response
In case request is missing a key
```json
{
  "status": false,
  "payload": null,
  "message": "Missing Key 'KEY_NAME' in request data",
  "error": {
    "code": 400
  }
}
```
