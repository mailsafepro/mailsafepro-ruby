# MailSafePro::EmailResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **email** | **String** | Validated email address |  |
| **valid** | **Boolean** | Overall validation result |  |
| **detail** | **String** | Validation details summary | [optional][default to &#39;&#39;] |
| **processing_time** | **Float** |  | [optional] |
| **provider** | **String** |  | [optional] |
| **reputation** | **Float** |  | [optional] |
| **fingerprint** | **String** |  | [optional] |
| **quality_score** | **Float** |  | [optional] |
| **risk_level** | [**RiskLevelEnum**](RiskLevelEnum.md) |  | [optional] |
| **suggestions** | **Array&lt;String&gt;** | Improvement suggestions | [optional] |
| **smtp** | [**SMTPInfo**](SMTPInfo.md) |  | [optional] |
| **dns** | [**DNSInfo**](DNSInfo.md) |  | [optional] |
| **risk_score** | **Float** |  | [optional] |
| **validation_tier** | **String** |  | [optional] |
| **suggested_action** | **String** |  | [optional] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::EmailResponse.new(
  email: null,
  valid: null,
  detail: null,
  processing_time: null,
  provider: null,
  reputation: null,
  fingerprint: null,
  quality_score: null,
  risk_level: null,
  suggestions: null,
  smtp: null,
  dns: null,
  risk_score: null,
  validation_tier: null,
  suggested_action: null
)
```

