# MailSafePro::SMTPInfo

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **checked** | **Boolean** | SMTP check was performed |  |
| **mailbox_exists** | **Boolean** |  | [optional] |
| **mx_server** | **String** |  | [optional] |
| **response_time** | **Float** |  | [optional] |
| **error_message** | **String** |  | [optional] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::SMTPInfo.new(
  checked: null,
  mailbox_exists: null,
  mx_server: null,
  response_time: null,
  error_message: null
)
```

