
### APIs

1. api/v1/google-retrieval/
- Input:
  - Url: Required
  - Keywords: Required(1 - 5 words)
  - location: default current location,
  - engine: 'google'
- Output:
  - JSON:
  ```
  {
    "status": "Success",
    "total_results": 500,
    "location_used": "Japan",
    "location_requested": "Japan",
    "engine": "google",
    [
      {
        "key_word": "会社概要"
        "rank": 1,
      },
      {
        "key_word": "サービス"
        "rank": 4
      },
    ]
  }
  ```

2. api/v1/yahoo-retrieval/
- Input:
  - Url: Required
  - Keywords: Required(1 - 5 words)
  - location: default current location
  - engine: 'yahoo'
- Output:
  - JSON:
  ```
  {
    "status": "Success",
    "location_used": "Japan",
    "location_requested": "Japan",
    "engine": "yahoo",
    [
      {
        "key_word": "会社概要"
        "rank": 1,
      },
      {
        "key_word": "サービス"
        "rank": 10
      },
    ]
  }
  ```