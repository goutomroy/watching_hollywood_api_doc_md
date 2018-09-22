**Get your watchlist**

### Api Endpoint
`/api/watchlist/`

### Methods
`GET`

### Header Parameters
Key | Value | Consideration
---- | ------- | --------
Content-Type | application/json | Required
Authorization | Token `api_key` | Required

### Url Parameters
Parameter| Type    | Description
---------|---------|----------------
page | Int  | default is 1


### Response
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


        
