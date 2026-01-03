# MailSafePro::DefaultApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**ask_gemini_gemini_get**](DefaultApi.md#ask_gemini_gemini_get) | **GET** /gemini | Ask Gemini |
| [**run_audit_admin_audit_project_post**](DefaultApi.md#run_audit_admin_audit_project_post) | **POST** /admin/audit_project | Run Audit |


## ask_gemini_gemini_get

> Object ask_gemini_gemini_get(prompt)

Ask Gemini

Llama a Gemini para generar texto a partir de un prompt

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::DefaultApi.new
prompt = 'prompt_example' # String | 

begin
  # Ask Gemini
  result = api_instance.ask_gemini_gemini_get(prompt)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling DefaultApi->ask_gemini_gemini_get: #{e}"
end
```

#### Using the ask_gemini_gemini_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> ask_gemini_gemini_get_with_http_info(prompt)

```ruby
begin
  # Ask Gemini
  data, status_code, headers = api_instance.ask_gemini_gemini_get_with_http_info(prompt)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling DefaultApi->ask_gemini_gemini_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **prompt** | **String** |  |  |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## run_audit_admin_audit_project_post

> Object run_audit_admin_audit_project_post(opts)

Run Audit

Lanza auditoría en path (ruta absoluta o relativa a la raíz del proyecto). Header obligatorio: X-Audit-Token: <AUDIT_SECRET>

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::DefaultApi.new
opts = {
  path: 'path_example', # String | 
  x_audit_token: 'x_audit_token_example' # String | 
}

begin
  # Run Audit
  result = api_instance.run_audit_admin_audit_project_post(opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling DefaultApi->run_audit_admin_audit_project_post: #{e}"
end
```

#### Using the run_audit_admin_audit_project_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> run_audit_admin_audit_project_post_with_http_info(opts)

```ruby
begin
  # Run Audit
  data, status_code, headers = api_instance.run_audit_admin_audit_project_post_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling DefaultApi->run_audit_admin_audit_project_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **path** | **String** |  | [optional][default to &#39;.&#39;] |
| **x_audit_token** | **String** |  | [optional] |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

