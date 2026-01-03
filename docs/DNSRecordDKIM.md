# MailSafePro::DNSRecordDKIM

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **status** | **String** |  | [optional] |
| **selector** | **String** |  | [optional] |
| **key_type** | **String** |  | [optional] |
| **key_length** | **Integer** |  | [optional] |
| **record** | **String** |  | [optional] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::DNSRecordDKIM.new(
  status: null,
  selector: null,
  key_type: null,
  key_length: null,
  record: null
)
```

