# MailSafePro::EmailValidationApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**batch_validate_emails_validate_batch_post**](EmailValidationApi.md#batch_validate_emails_validate_batch_post) | **POST** /validate/batch | Batch Email Validation |
| [**batch_validate_upload_validate_batch_upload_post**](EmailValidationApi.md#batch_validate_upload_validate_batch_upload_post) | **POST** /validate/batch/upload | Batch Email Validation via File Upload |
| [**get_cache_stats_validate_stats_cache_get**](EmailValidationApi.md#get_cache_stats_validate_stats_cache_get) | **GET** /validate/stats/cache | Get Cache Stats |
| [**get_usage_stats_validate_stats_usage_get**](EmailValidationApi.md#get_usage_stats_validate_stats_usage_get) | **GET** /validate/stats/usage | Get Usage Stats |
| [**health_check_validate_health_get**](EmailValidationApi.md#health_check_validate_health_get) | **GET** /validate/health | Health Check |
| [**health_check_validate_health_head**](EmailValidationApi.md#health_check_validate_health_head) | **HEAD** /validate/health | Health Check |
| [**validate_email_endpoint_validate_email_post**](EmailValidationApi.md#validate_email_endpoint_validate_email_post) | **POST** /validate/email | Validate Email Endpoint |


## batch_validate_emails_validate_batch_post

> <BatchEmailResponse> batch_validate_emails_validate_batch_post(batch_validation_request, opts)

Batch Email Validation

Valida múltiples direcciones de email en una sola solicitud.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::EmailValidationApi.new
batch_validation_request = MailSafePro::BatchValidationRequest.new({emails: ['emails_example']}) # BatchValidationRequest | 
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Batch Email Validation
  result = api_instance.batch_validate_emails_validate_batch_post(batch_validation_request, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->batch_validate_emails_validate_batch_post: #{e}"
end
```

#### Using the batch_validate_emails_validate_batch_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BatchEmailResponse>, Integer, Hash)> batch_validate_emails_validate_batch_post_with_http_info(batch_validation_request, opts)

```ruby
begin
  # Batch Email Validation
  data, status_code, headers = api_instance.batch_validate_emails_validate_batch_post_with_http_info(batch_validation_request, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BatchEmailResponse>
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->batch_validate_emails_validate_batch_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **batch_validation_request** | [**BatchValidationRequest**](BatchValidationRequest.md) |  |  |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

[**BatchEmailResponse**](BatchEmailResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## batch_validate_upload_validate_batch_upload_post

> Object batch_validate_upload_validate_batch_upload_post(file, opts)

Batch Email Validation via File Upload

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::EmailValidationApi.new
file = File.new('/path/to/some/file') # File | 
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example', # String | 
  column: 'column_example', # String | 
  include_raw_dns: true, # Boolean | 
  check_smtp: true # Boolean | 
}

begin
  # Batch Email Validation via File Upload
  result = api_instance.batch_validate_upload_validate_batch_upload_post(file, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->batch_validate_upload_validate_batch_upload_post: #{e}"
end
```

#### Using the batch_validate_upload_validate_batch_upload_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> batch_validate_upload_validate_batch_upload_post_with_http_info(file, opts)

```ruby
begin
  # Batch Email Validation via File Upload
  data, status_code, headers = api_instance.batch_validate_upload_validate_batch_upload_post_with_http_info(file, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->batch_validate_upload_validate_batch_upload_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **file** | **File** |  |  |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |
| **column** | **String** |  | [optional] |
| **include_raw_dns** | **Boolean** |  | [optional][default to false] |
| **check_smtp** | **Boolean** |  | [optional][default to false] |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json


## get_cache_stats_validate_stats_cache_get

> Object get_cache_stats_validate_stats_cache_get

Get Cache Stats

Obtiene estadísticas de cache del sistema.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::EmailValidationApi.new

begin
  # Get Cache Stats
  result = api_instance.get_cache_stats_validate_stats_cache_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->get_cache_stats_validate_stats_cache_get: #{e}"
end
```

#### Using the get_cache_stats_validate_stats_cache_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> get_cache_stats_validate_stats_cache_get_with_http_info

```ruby
begin
  # Get Cache Stats
  data, status_code, headers = api_instance.get_cache_stats_validate_stats_cache_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->get_cache_stats_validate_stats_cache_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_usage_stats_validate_stats_usage_get

> Object get_usage_stats_validate_stats_usage_get(opts)

Get Usage Stats

Obtiene estadísticas de uso del cliente actual.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::EmailValidationApi.new
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Get Usage Stats
  result = api_instance.get_usage_stats_validate_stats_usage_get(opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->get_usage_stats_validate_stats_usage_get: #{e}"
end
```

#### Using the get_usage_stats_validate_stats_usage_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> get_usage_stats_validate_stats_usage_get_with_http_info(opts)

```ruby
begin
  # Get Usage Stats
  data, status_code, headers = api_instance.get_usage_stats_validate_stats_usage_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->get_usage_stats_validate_stats_usage_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## health_check_validate_health_get

> Object health_check_validate_health_get

Health Check

Health check completo del servicio de validación.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::EmailValidationApi.new

begin
  # Health Check
  result = api_instance.health_check_validate_health_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->health_check_validate_health_get: #{e}"
end
```

#### Using the health_check_validate_health_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> health_check_validate_health_get_with_http_info

```ruby
begin
  # Health Check
  data, status_code, headers = api_instance.health_check_validate_health_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->health_check_validate_health_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## health_check_validate_health_head

> Object health_check_validate_health_head

Health Check

Health check completo del servicio de validación.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::EmailValidationApi.new

begin
  # Health Check
  result = api_instance.health_check_validate_health_head
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->health_check_validate_health_head: #{e}"
end
```

#### Using the health_check_validate_health_head_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> health_check_validate_health_head_with_http_info

```ruby
begin
  # Health Check
  data, status_code, headers = api_instance.health_check_validate_health_head_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->health_check_validate_health_head_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## validate_email_endpoint_validate_email_post

> Object validate_email_endpoint_validate_email_post(email_validation_request, opts)

Validate Email Endpoint

✅ Endpoint de validación de email con timeout y fallback robusto.  Cambios principales: - Timeout explícito por plan (FREE: 15s, PREMIUM: 45s, ENTERPRISE: 60s) - Fallback BASIC seguro si se vence - SIEMPRE retorna JSONResponse válida - client_plan en TODAS las respuestas - spam_trap_check ejecutado ANTES del timeout para estar disponible en fallback - Manejo de errores con ResponseBuilder - ✅ NUEVO: Soporte para TLD .test en testing_mode

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::EmailValidationApi.new
email_validation_request = MailSafePro::EmailValidationRequest.new({email: 'email_example'}) # EmailValidationRequest | 
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Validate Email Endpoint
  result = api_instance.validate_email_endpoint_validate_email_post(email_validation_request, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->validate_email_endpoint_validate_email_post: #{e}"
end
```

#### Using the validate_email_endpoint_validate_email_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> validate_email_endpoint_validate_email_post_with_http_info(email_validation_request, opts)

```ruby
begin
  # Validate Email Endpoint
  data, status_code, headers = api_instance.validate_email_endpoint_validate_email_post_with_http_info(email_validation_request, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling EmailValidationApi->validate_email_endpoint_validate_email_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **email_validation_request** | [**EmailValidationRequest**](EmailValidationRequest.md) |  |  |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

