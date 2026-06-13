# Bored API

Free REST API that suggests random activities to do when bored, filterable by type, number of participants, price range, and accessibility. A teaching tool by The App Brewery with no authentication required.

**Documentation:** https://bored-api.appbrewery.com/

## Endpoints

- `GET /random` — Returns a randomly selected activity
- `GET /filter` — Returns activities filtered by type and/or participant count
- `GET /activity/{key}` — Returns the activity with the specified unique key

## Activity Types

education, recreational, social, charity, cooking, relaxation, busywork

## Response Fields

- `activity` — Description of the activity
- `availability` — Availability score (0.0–1.0)
- `type` — Category of activity
- `participants` — Number of participants (1, 2, 3, 4, 5, 6, 8)
- `price` — Cost estimate (0.0–1.0 scale)
- `accessibility` — Accessibility level description
- `duration` — Time scale (minutes, hours, days)
- `kidFriendly` — Whether activity is appropriate for children
- `link` — Optional external resource link
- `key` — Unique activity identifier

## Rate Limits

100 requests per 15 minutes. No authentication required.

## License

Source code: MIT License (https://github.com/drewthoennes/Bored-API)
