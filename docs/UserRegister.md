# MailSafePro::UserRegister

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **email** | **String** | User email address |  |
| **password** | **String** | User password |  |
| **plan** | [**PlanEnum**](PlanEnum.md) | Subscription plan | [optional] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::UserRegister.new(
  email: null,
  password: null,
  plan: null
)
```

