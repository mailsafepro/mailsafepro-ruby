# MailSafePro::JobCreateRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **source** | **String** | Origen de los datos |  |
| **emails** | **Array&lt;String&gt;** |  | [optional] |
| **file_token** | **String** |  | [optional] |
| **checksmtp** | **Boolean** |  | [optional][default to false] |
| **includerawdns** | **Boolean** |  | [optional][default to false] |
| **callback_url** | **String** |  | [optional] |
| **sandbox** | **Boolean** |  | [optional][default to false] |
| **metadata** | **Object** |  | [optional] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::JobCreateRequest.new(
  source: null,
  emails: null,
  file_token: null,
  checksmtp: null,
  includerawdns: null,
  callback_url: null,
  sandbox: null,
  metadata: null
)
```

