# MailSafePro::APIKeyMeta

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** | Unique key identifier |  |
| **key_hash** | **String** | Hashed key value |  |
| **plan** | [**PlanEnum**](PlanEnum.md) | Associated plan |  |
| **created_at** | **Time** | Creation timestamp |  |
| **revoked** | **Boolean** | Revocation status |  |
| **revoked_at** | **Time** |  | [optional] |
| **scopes** | **Array&lt;String&gt;** | Access scopes | [optional] |
| **name** | **String** |  | [optional] |
| **last_used** | **Time** |  | [optional] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::APIKeyMeta.new(
  id: null,
  key_hash: null,
  plan: null,
  created_at: null,
  revoked: null,
  revoked_at: null,
  scopes: null,
  name: null,
  last_used: null
)
```

