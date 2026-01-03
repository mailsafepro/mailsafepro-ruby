# MailSafePro::WebhookCreate

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **url** | **String** |  |  |
| **events** | **Array&lt;String&gt;** |  | [optional] |
| **secret** | **String** |  | [optional] |
| **description** | **String** |  | [optional] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::WebhookCreate.new(
  url: null,
  events: null,
  secret: null,
  description: null
)
```

