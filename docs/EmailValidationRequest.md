# MailSafePro::EmailValidationRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **email** | **String** | Email address to validate (RFC 5321 compliant) |  |
| **check_smtp** | **Boolean** | Enable SMTP mailbox verification | [optional][default to false] |
| **include_raw_dns** | **Boolean** | Include raw DNS records | [optional][default to false] |
| **testing_mode** | **Boolean** | Enable testing mode (allows special TLDs like .test, .example, etc.) | [optional][default to false] |
| **priority** | [**PriorityEnum**](PriorityEnum.md) | Validation priority level | [optional] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::EmailValidationRequest.new(
  email: null,
  check_smtp: null,
  include_raw_dns: null,
  testing_mode: null,
  priority: null
)
```

