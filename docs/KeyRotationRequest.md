# MailSafePro::KeyRotationRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **old_key** | **String** | Current API key to rotate from |  |
| **new_key** | **String** | New API key to rotate to |  |
| **grace_period** | **Integer** | Grace period in seconds (max 30 days) | [optional][default to 86400] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::KeyRotationRequest.new(
  old_key: null,
  new_key: null,
  grace_period: null
)
```

