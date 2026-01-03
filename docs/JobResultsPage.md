# MailSafePro::JobResultsPage

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **job_id** | **String** |  |  |
| **page** | **Integer** |  |  |
| **size** | **Integer** |  |  |
| **total_pages** | **Integer** |  |  |
| **results** | [**Array&lt;JobResultEntry&gt;**](JobResultEntry.md) |  |  |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::JobResultsPage.new(
  job_id: null,
  page: null,
  size: null,
  total_pages: null,
  results: null
)
```

