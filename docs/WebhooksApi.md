# MailSafePro::WebhooksApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_webhook_webhooks_management_webhooks_post**](WebhooksApi.md#create_webhook_webhooks_management_webhooks_post) | **POST** /webhooks-management/webhooks/ | Create Webhook |
| [**delete_webhook_webhooks_management_webhooks_webhook_id_delete**](WebhooksApi.md#delete_webhook_webhooks_management_webhooks_webhook_id_delete) | **DELETE** /webhooks-management/webhooks/{webhook_id} | Delete Webhook |
| [**get_deliveries_webhooks_management_webhooks_webhook_id_deliveries_get**](WebhooksApi.md#get_deliveries_webhooks_management_webhooks_webhook_id_deliveries_get) | **GET** /webhooks-management/webhooks/{webhook_id}/deliveries | Get Deliveries |
| [**get_webhook_webhooks_management_webhooks_webhook_id_get**](WebhooksApi.md#get_webhook_webhooks_management_webhooks_webhook_id_get) | **GET** /webhooks-management/webhooks/{webhook_id} | Get Webhook |
| [**list_webhooks_webhooks_management_webhooks_get**](WebhooksApi.md#list_webhooks_webhooks_management_webhooks_get) | **GET** /webhooks-management/webhooks/ | List Webhooks |
| [**register_endpoint_webhooks_v1_webhooks_endpoints_register_post**](WebhooksApi.md#register_endpoint_webhooks_v1_webhooks_endpoints_register_post) | **POST** /webhooks/v1/webhooks/endpoints/register | Register Endpoint |
| [**register_endpoint_webhooks_v1_webhooks_endpoints_register_post_0**](WebhooksApi.md#register_endpoint_webhooks_v1_webhooks_endpoints_register_post_0) | **POST** /webhooks/v1/webhooks/endpoints/register | Register Endpoint |
| [**rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post**](WebhooksApi.md#rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post) | **POST** /webhooks/v1/webhooks/endpoints/rotate | Rotate Secret |
| [**rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_0**](WebhooksApi.md#rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_0) | **POST** /webhooks/v1/webhooks/endpoints/rotate | Rotate Secret |
| [**test_webhook_webhooks_management_webhooks_webhook_id_test_post**](WebhooksApi.md#test_webhook_webhooks_management_webhooks_webhook_id_test_post) | **POST** /webhooks-management/webhooks/{webhook_id}/test | Test Webhook |
| [**update_webhook_webhooks_management_webhooks_webhook_id_patch**](WebhooksApi.md#update_webhook_webhooks_management_webhooks_webhook_id_patch) | **PATCH** /webhooks-management/webhooks/{webhook_id} | Update Webhook |


## create_webhook_webhooks_management_webhooks_post

> Object create_webhook_webhooks_management_webhooks_post(webhook_create)

Create Webhook

Create a new webhook endpoint.  Events available: - validation.completed: Single email validation finished - batch.completed: Batch validation finished - usage.limit_reached: API usage limit reached (80%)

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::WebhooksApi.new
webhook_create = MailSafePro::WebhookCreate.new({url: 'url_example'}) # WebhookCreate | 

begin
  # Create Webhook
  result = api_instance.create_webhook_webhooks_management_webhooks_post(webhook_create)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->create_webhook_webhooks_management_webhooks_post: #{e}"
end
```

#### Using the create_webhook_webhooks_management_webhooks_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> create_webhook_webhooks_management_webhooks_post_with_http_info(webhook_create)

```ruby
begin
  # Create Webhook
  data, status_code, headers = api_instance.create_webhook_webhooks_management_webhooks_post_with_http_info(webhook_create)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->create_webhook_webhooks_management_webhooks_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **webhook_create** | [**WebhookCreate**](WebhookCreate.md) |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## delete_webhook_webhooks_management_webhooks_webhook_id_delete

> Object delete_webhook_webhooks_management_webhooks_webhook_id_delete(webhook_id)

Delete Webhook

Delete webhook.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::WebhooksApi.new
webhook_id = 'webhook_id_example' # String | 

begin
  # Delete Webhook
  result = api_instance.delete_webhook_webhooks_management_webhooks_webhook_id_delete(webhook_id)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->delete_webhook_webhooks_management_webhooks_webhook_id_delete: #{e}"
end
```

#### Using the delete_webhook_webhooks_management_webhooks_webhook_id_delete_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> delete_webhook_webhooks_management_webhooks_webhook_id_delete_with_http_info(webhook_id)

```ruby
begin
  # Delete Webhook
  data, status_code, headers = api_instance.delete_webhook_webhooks_management_webhooks_webhook_id_delete_with_http_info(webhook_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->delete_webhook_webhooks_management_webhooks_webhook_id_delete_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **webhook_id** | **String** |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_deliveries_webhooks_management_webhooks_webhook_id_deliveries_get

> Object get_deliveries_webhooks_management_webhooks_webhook_id_deliveries_get(webhook_id, opts)

Get Deliveries

Get delivery history for webhook.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::WebhooksApi.new
webhook_id = 'webhook_id_example' # String | 
opts = {
  limit: 56 # Integer | 
}

begin
  # Get Deliveries
  result = api_instance.get_deliveries_webhooks_management_webhooks_webhook_id_deliveries_get(webhook_id, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->get_deliveries_webhooks_management_webhooks_webhook_id_deliveries_get: #{e}"
end
```

#### Using the get_deliveries_webhooks_management_webhooks_webhook_id_deliveries_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> get_deliveries_webhooks_management_webhooks_webhook_id_deliveries_get_with_http_info(webhook_id, opts)

```ruby
begin
  # Get Deliveries
  data, status_code, headers = api_instance.get_deliveries_webhooks_management_webhooks_webhook_id_deliveries_get_with_http_info(webhook_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->get_deliveries_webhooks_management_webhooks_webhook_id_deliveries_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **webhook_id** | **String** |  |  |
| **limit** | **Integer** |  | [optional][default to 100] |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_webhook_webhooks_management_webhooks_webhook_id_get

> Object get_webhook_webhooks_management_webhooks_webhook_id_get(webhook_id)

Get Webhook

Get webhook details.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::WebhooksApi.new
webhook_id = 'webhook_id_example' # String | 

begin
  # Get Webhook
  result = api_instance.get_webhook_webhooks_management_webhooks_webhook_id_get(webhook_id)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->get_webhook_webhooks_management_webhooks_webhook_id_get: #{e}"
end
```

#### Using the get_webhook_webhooks_management_webhooks_webhook_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> get_webhook_webhooks_management_webhooks_webhook_id_get_with_http_info(webhook_id)

```ruby
begin
  # Get Webhook
  data, status_code, headers = api_instance.get_webhook_webhooks_management_webhooks_webhook_id_get_with_http_info(webhook_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->get_webhook_webhooks_management_webhooks_webhook_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **webhook_id** | **String** |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_webhooks_webhooks_management_webhooks_get

> Object list_webhooks_webhooks_management_webhooks_get

List Webhooks

List all webhooks for authenticated user.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::WebhooksApi.new

begin
  # List Webhooks
  result = api_instance.list_webhooks_webhooks_management_webhooks_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->list_webhooks_webhooks_management_webhooks_get: #{e}"
end
```

#### Using the list_webhooks_webhooks_management_webhooks_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> list_webhooks_webhooks_management_webhooks_get_with_http_info

```ruby
begin
  # List Webhooks
  data, status_code, headers = api_instance.list_webhooks_webhooks_management_webhooks_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->list_webhooks_webhooks_management_webhooks_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## register_endpoint_webhooks_v1_webhooks_endpoints_register_post

> Object register_endpoint_webhooks_v1_webhooks_endpoints_register_post(register_endpoint, opts)

Register Endpoint

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::WebhooksApi.new
register_endpoint = MailSafePro::RegisterEndpoint.new({callback_url: 'callback_url_example'}) # RegisterEndpoint | 
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Register Endpoint
  result = api_instance.register_endpoint_webhooks_v1_webhooks_endpoints_register_post(register_endpoint, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->register_endpoint_webhooks_v1_webhooks_endpoints_register_post: #{e}"
end
```

#### Using the register_endpoint_webhooks_v1_webhooks_endpoints_register_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> register_endpoint_webhooks_v1_webhooks_endpoints_register_post_with_http_info(register_endpoint, opts)

```ruby
begin
  # Register Endpoint
  data, status_code, headers = api_instance.register_endpoint_webhooks_v1_webhooks_endpoints_register_post_with_http_info(register_endpoint, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->register_endpoint_webhooks_v1_webhooks_endpoints_register_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **register_endpoint** | [**RegisterEndpoint**](RegisterEndpoint.md) |  |  |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## register_endpoint_webhooks_v1_webhooks_endpoints_register_post_0

> Object register_endpoint_webhooks_v1_webhooks_endpoints_register_post_0(register_endpoint, opts)

Register Endpoint

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::WebhooksApi.new
register_endpoint = MailSafePro::RegisterEndpoint.new({callback_url: 'callback_url_example'}) # RegisterEndpoint | 
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Register Endpoint
  result = api_instance.register_endpoint_webhooks_v1_webhooks_endpoints_register_post_0(register_endpoint, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->register_endpoint_webhooks_v1_webhooks_endpoints_register_post_0: #{e}"
end
```

#### Using the register_endpoint_webhooks_v1_webhooks_endpoints_register_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> register_endpoint_webhooks_v1_webhooks_endpoints_register_post_0_with_http_info(register_endpoint, opts)

```ruby
begin
  # Register Endpoint
  data, status_code, headers = api_instance.register_endpoint_webhooks_v1_webhooks_endpoints_register_post_0_with_http_info(register_endpoint, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->register_endpoint_webhooks_v1_webhooks_endpoints_register_post_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **register_endpoint** | [**RegisterEndpoint**](RegisterEndpoint.md) |  |  |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post

> Object rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post(rotate_secret, opts)

Rotate Secret

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::WebhooksApi.new
rotate_secret = MailSafePro::RotateSecret.new({endpoint_id: 'endpoint_id_example'}) # RotateSecret | 
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Rotate Secret
  result = api_instance.rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post(rotate_secret, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post: #{e}"
end
```

#### Using the rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_with_http_info(rotate_secret, opts)

```ruby
begin
  # Rotate Secret
  data, status_code, headers = api_instance.rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_with_http_info(rotate_secret, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **rotate_secret** | [**RotateSecret**](RotateSecret.md) |  |  |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_0

> Object rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_0(rotate_secret, opts)

Rotate Secret

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::WebhooksApi.new
rotate_secret = MailSafePro::RotateSecret.new({endpoint_id: 'endpoint_id_example'}) # RotateSecret | 
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Rotate Secret
  result = api_instance.rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_0(rotate_secret, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_0: #{e}"
end
```

#### Using the rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_0_with_http_info(rotate_secret, opts)

```ruby
begin
  # Rotate Secret
  data, status_code, headers = api_instance.rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_0_with_http_info(rotate_secret, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->rotate_secret_webhooks_v1_webhooks_endpoints_rotate_post_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **rotate_secret** | [**RotateSecret**](RotateSecret.md) |  |  |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## test_webhook_webhooks_management_webhooks_webhook_id_test_post

> Object test_webhook_webhooks_management_webhooks_webhook_id_test_post(webhook_id)

Test Webhook

Send test event to webhook.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::WebhooksApi.new
webhook_id = 'webhook_id_example' # String | 

begin
  # Test Webhook
  result = api_instance.test_webhook_webhooks_management_webhooks_webhook_id_test_post(webhook_id)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->test_webhook_webhooks_management_webhooks_webhook_id_test_post: #{e}"
end
```

#### Using the test_webhook_webhooks_management_webhooks_webhook_id_test_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> test_webhook_webhooks_management_webhooks_webhook_id_test_post_with_http_info(webhook_id)

```ruby
begin
  # Test Webhook
  data, status_code, headers = api_instance.test_webhook_webhooks_management_webhooks_webhook_id_test_post_with_http_info(webhook_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->test_webhook_webhooks_management_webhooks_webhook_id_test_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **webhook_id** | **String** |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## update_webhook_webhooks_management_webhooks_webhook_id_patch

> Object update_webhook_webhooks_management_webhooks_webhook_id_patch(webhook_id, webhook_update)

Update Webhook

Update webhook configuration.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::WebhooksApi.new
webhook_id = 'webhook_id_example' # String | 
webhook_update = MailSafePro::WebhookUpdate.new # WebhookUpdate | 

begin
  # Update Webhook
  result = api_instance.update_webhook_webhooks_management_webhooks_webhook_id_patch(webhook_id, webhook_update)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->update_webhook_webhooks_management_webhooks_webhook_id_patch: #{e}"
end
```

#### Using the update_webhook_webhooks_management_webhooks_webhook_id_patch_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> update_webhook_webhooks_management_webhooks_webhook_id_patch_with_http_info(webhook_id, webhook_update)

```ruby
begin
  # Update Webhook
  data, status_code, headers = api_instance.update_webhook_webhooks_management_webhooks_webhook_id_patch_with_http_info(webhook_id, webhook_update)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling WebhooksApi->update_webhook_webhooks_management_webhooks_webhook_id_patch_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **webhook_id** | **String** |  |  |
| **webhook_update** | [**WebhookUpdate**](WebhookUpdate.md) |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

