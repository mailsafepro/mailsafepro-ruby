# MailSafePro::BatchEmailResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **count** | **Integer** | Total emails processed |  |
| **valid_count** | **Integer** | Number of valid emails |  |
| **invalid_count** | **Integer** | Number of invalid emails |  |
| **processing_time** | **Float** | Total processing time in seconds |  |
| **average_time** | **Float** | Average processing time per email |  |
| **results** | [**Array&lt;EmailResponse&gt;**](EmailResponse.md) | Individual validation results |  |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::BatchEmailResponse.new(
  count: null,
  valid_count: null,
  invalid_count: null,
  processing_time: null,
  average_time: null,
  results: null
)
```

