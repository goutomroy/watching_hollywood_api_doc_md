**Add or remove movie from your watchlist**

### Api Endpoint
`/api/watchlist_action/`

### Methods
`POST`

### Header Parameters
Key | Value | Consideration
---- | ------- | --------
Content-Type | application/json | Required
Authorization | Token `api_key` | Required

### Post Json Payload Format
Parameter| Type    | Description
---------|---------|----------------
movie_id | Long  |
action_type  | Integer | 1 for adding, 0 for removing from watchlist

### Response
*   Status code : 200

```json
    {
        "success": false,
        "message": "Movie not found."
    }
```

### Response
*   Status code : 200

```json
    {
        "success": true,
        "message": "Already in Watchlist"
    }
```

### Response
*   Status code : 200

```json
    {
        "success": true,
        "message": "Added to Watchlist"
    }
```

### Response
*   Status code : 200

```json
    {
        "success": true,
        "message": "Not in Watchlist to remove"
    }
```

### Response
*   Status code : 200

```json
    {
        "success": true,
        "message": "Removed from watchlist"
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


        
