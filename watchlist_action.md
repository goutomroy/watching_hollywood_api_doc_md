## Public Api
**It returns 100 hollywood movies recently popular in theatres**

### Api Endpoint
`/api/watchlist_action/`

### Methods
`POST`

### Header Parameters
Key | Value | Consideration
---- | ------- | --------
Content-Type | application/json | Required
Authorization | Token `api_key` | Required

# Post Json Payload Format
Parameter| Type    | Description
---------|---------|----------------
movie_id | String  | This is firebase id token.
action_type  | Integer | 1 for adding, 0 for removing from watchlisy


### Response Type 1
*   Status code : 200
```json
{
    "total_results": 3,
    "total_pages": 1,
    "page": "1",
    "previous": null,
    "next": null,
    "results": [
        {
            "id": 526,
            "tmdb_id": 238636,
            "tmdb_data": {
                "id": 238636,
                "adult": false,
                "title": "The Purge: Anarchy",
                "video": false,
                "overview": "One night per year, the government sanctions a 12-hour period in which citizens can commit any crime they wish -- including murder -- without fear of punishment or imprisonment. Leo, a sergeant who lost his son, plans a vigilante mission of revenge during the mayhem. However, instead of a death-dealing avenger, he becomes the unexpected protector of four innocent strangers who desperately need his help if they are to survive the night.",
                "genre_ids": [
                    27,
                    53
                ],
                "popularity": 41.057,
                "vote_count": 3038,
                "poster_path": "/l1DRl40x2OWUoPP42v8fjKdS1Z3.jpg",
                "release_date": "2014-07-17",
                "vote_average": 6.6,
                "backdrop_path": "/zWGAnbxjjwY3xFGuOeR26LGbBlG.jpg",
                "original_title": "The Purge: Anarchy",
                "original_language": "en"
            }
        }
    ],
    "success": true
}

```

### Response Type 2
*   Status code : 200

```json
    {
        "success": false,
        "message": "Something went wrong.Please try again later."
    }
```

### Response Type 3
*   Status code : 200

```json
    {
        "success": true,
        "message": "Already in Watchlist"
    }
```

### Response Type 4
*   Status code : 200

```json
    {
        "success": true,
        "message": "Not in Watchlist to remove"
    }
```

### Response Type 5
*   Status code : 200

```json
    {
        "success": true,
        "message": "Removed from watchlist"
    }
```


### Response Type 6
*   Status code : 200

```json
    {
        "success": true,
        "message": "Something went wrong.Please try again later."
    }
```

### Response Type 7
*   Status code : 400

```json
    {
        "message": "Bad Request"
    }
```

### Response Type 8
*   Status code : 401

```json
    {
        "message": "Invalid token"
    }
```

### Response Type 9
*   Status code : 405

```json
    {
        "message": "Request method is not allowed"
    }
```




        
