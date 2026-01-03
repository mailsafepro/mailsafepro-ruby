# MailSafePro::BatchValidationRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **emails** | **Array&lt;String&gt;** | List of email addresses to validate (can include invalid formats) |  |
| **check_smtp** | **Boolean** | Perform SMTP verification for all emails | [optional][default to false] |
| **include_raw_dns** | **Boolean** | Include raw DNS records in responses | [optional][default to false] |
| **batch_size** | **Integer** | Number of emails to process in each batch | [optional][default to 100] |
| **concurrent_requests** | **Integer** | Maximum concurrent validation requests | [optional][default to 5] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::BatchValidationRequest.new(
  emails: null,
  check_smtp: null,
  include_raw_dns: null,
  batch_size: null,
  concurrent_requests: null
)
```

