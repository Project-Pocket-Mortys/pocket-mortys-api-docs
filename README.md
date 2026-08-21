# Pocket Mortys API

Documentation and reference implementation of the Pocket Mortys backend API.

## API Endpoints

### `GET https://newc137.bps-pmnet.com/time`

Returns the current server time.

**Response**
```json
{
  "time": "2026-08-21T03:58:00Z"
}
```

### `GET https://newc137.conspiracyrick.com/is-gdpr/`

Returns the privacy/regulatory-region check.

**Response**
```json
{
	"countryCode": "US",
	"GDPR": true,
	"CCPA": true
}
```

### `GET https://rat.game.bps-pmnet.com/inappdeletion/get-account-data-storage-time`

Returns the account-data deletion / retention.

**Response**
```json
{
	"time_anyUnits": 12
}
```

### `POST https://rat.game.bps-pmnet.com/inappdeletion/request-account-deletion`

Returns the account-data deletion / retention.

**Request**
```json
{
  "uuid": "12345678-abcd-1234-abcd-123456789abc"
}
```
**Response**
```markdown
12345678-abcd-1234-abcd-123456789abc
```
