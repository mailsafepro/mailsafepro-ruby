# MailSafePro::APIKeyCreateRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** |  | [optional] |
| **scopes** | **Array&lt;String&gt;** | Access scopes for the API Key | [optional] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::APIKeyCreateRequest.new(
  name: null,
  scopes: null
)
```

