# MailSafePro::JobResultEntry

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **email** | **String** |  |  |
| **valid** | **Boolean** |  |  |
| **riskscore** | **Float** |  | [optional] |
| **qualityscore** | **Float** |  | [optional] |
| **provider** | **String** |  | [optional] |
| **reputation** | **Float** |  | [optional] |
| **smtp** | **Object** |  | [optional] |
| **dns** | **Object** |  | [optional] |
| **metadata** | **Object** |  | [optional] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::JobResultEntry.new(
  email: null,
  valid: null,
  riskscore: null,
  qualityscore: null,
  provider: null,
  reputation: null,
  smtp: null,
  dns: null,
  metadata: null
)
```

