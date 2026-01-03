# MailSafePro::SubscriptionResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **plan** | **String** |  |  |
| **next_billing_date** | **String** |  | [optional] |
| **status** | **String** |  | [optional][default to &#39;active&#39;] |
| **customer_id** | **String** |  | [optional] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::SubscriptionResponse.new(
  plan: null,
  next_billing_date: null,
  status: null,
  customer_id: null
)
```

