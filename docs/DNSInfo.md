# MailSafePro::DNSInfo

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **spf** | [**DNSRecordSPF**](DNSRecordSPF.md) |  | [optional] |
| **dkim** | [**DNSRecordDKIM**](DNSRecordDKIM.md) |  | [optional] |
| **dmarc** | [**DNSRecordDMARC**](DNSRecordDMARC.md) |  | [optional] |
| **mx_records** | **Array&lt;String&gt;** | MX records | [optional] |
| **ns_records** | **Array&lt;String&gt;** | Name servers | [optional] |

## Example

```ruby
require 'mailsafepro'

instance = MailSafePro::DNSInfo.new(
  spf: null,
  dkim: null,
  dmarc: null,
  mx_records: null,
  ns_records: null
)
```

