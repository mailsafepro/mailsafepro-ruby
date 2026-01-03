# MailSafePro::APIKeyListResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **keys** | [**Array&lt;APIKeyMeta&gt;**](APIKeyMeta.md) | List of API keys |  |
| **total_count** | **Integer** | Total number of keys |  |
| **active_count** | **Integer** | Number of active keys |  |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::APIKeyListResponse.new(
  keys: null,
  total_count: null,
  active_count: null
)
```

