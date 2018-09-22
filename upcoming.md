## Public Api
**It returns 100 hollywood movies upcoming in theatres**

### Api Endpoint
`/api/upcoming/`

### Methods
`GET`

### Header Parameters
Key | Value | Consideration
---- | ------- | --------
Content-Type | application/json | Required

### Response Type 1
*   Status code : 200

```json
{
    "success": true,
    "results": [
        {
            "id": 281,
            "tmdb_id": 353081,
            "tmdb_data": {
                "vote_count": 1297,
                "id": 353081,
                "video": false,
                "vote_average": 7.3,
                "title": "Mission: Impossible - Fallout",
                "popularity": 150.504,
                "poster_path": "/AkJQpZp9WoNdj7pLYSj1L0RcMMN.jpg",
                "original_language": "en",
                "original_title": "Mission: Impossible - Fallout",
                "genre_ids": [
                    12,
                    28,
                    53
                ],
                "backdrop_path": "/5qxePyMYDisLe8rJiBYX8HKEyv2.jpg",
                "adult": false,
                "overview": "When an IMF mission ends badly, the world is faced with dire consequences. As Ethan Hunt takes it upon himself to fulfil his original briefing, the CIA begin to question his loyalty and his motives. The IMF team find themselves in a race against time, hunted by assassins while trying to prevent a global catastrophe.",
                "release_date": "2018-07-25"
            }
        }]
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
        
