**Register or sign in**

### Api Endpoint
`/api/sign_in/`

### Methods
`POST`

### Header Parameters
Key | Value | Consideration
---- | ------- | --------
Content-Type | application/json | Required

### Post Json Payload Format
Parameter| Type    | Description
---------|---------|----------------
firebase_id_token | String  |

### Response
*   Status code : 200

```json
    {
        "success": true,
        "api_key" : "fadsfa777afdsfa"
    }
```

### Response
*   Status code : 400

```json
    {
        "message": "Bad Request"
    }
```

### Response
*   Status code : 401

```json
    {
        "message": "Invalid token"
    }
```

### Response
*   Status code : 405

```json
    {
        "message": "Request method is not allowed"
    }
```

### Response 2
*   Status code : 500

```json
    {
        "message": "Server error"
    }
```


        
