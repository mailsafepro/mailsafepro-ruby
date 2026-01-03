# MailSafePro::JobStatusResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **job_id** | **String** |  |  |
| **status** | **String** |  |  |
| **counts** | **Hash&lt;String, Integer&gt;** |  | [optional] |
| **started_at** | **String** |  | [optional] |
| **finished_at** | **String** |  | [optional] |
| **error** | **String** |  | [optional] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::JobStatusResponse.new(
  job_id: null,
  status: null,
  counts: null,
  started_at: null,
  finished_at: null,
  error: null
)
```

