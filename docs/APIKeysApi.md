# MailSafePro::APIKeysApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_api_key_api_keys_post**](APIKeysApi.md#create_api_key_api_keys_post) | **POST** /api-keys | Create Api Key |
| [**create_api_key_api_keys_post_0**](APIKeysApi.md#create_api_key_api_keys_post_0) | **POST** /api-keys | Create Api Key |
| [**force_sync_api_keys_force_sync_post**](APIKeysApi.md#force_sync_api_keys_force_sync_post) | **POST** /api-keys/force-sync | Force Sync |
| [**force_sync_api_keys_force_sync_post_0**](APIKeysApi.md#force_sync_api_keys_force_sync_post_0) | **POST** /api-keys/force-sync | Force Sync |
| [**get_api_key_value_api_keys_key_hash_value_get**](APIKeysApi.md#get_api_key_value_api_keys_key_hash_value_get) | **GET** /api-keys/{key_hash}/value | Get Api Key Value |
| [**get_api_key_value_api_keys_key_hash_value_get_0**](APIKeysApi.md#get_api_key_value_api_keys_key_hash_value_get_0) | **GET** /api-keys/{key_hash}/value | Get Api Key Value |
| [**get_usage_api_keys_usage_get**](APIKeysApi.md#get_usage_api_keys_usage_get) | **GET** /api-keys/usage | Get Usage |
| [**get_usage_api_keys_usage_get_0**](APIKeysApi.md#get_usage_api_keys_usage_get_0) | **GET** /api-keys/usage | Get Usage |
| [**list_api_keys_api_keys_get**](APIKeysApi.md#list_api_keys_api_keys_get) | **GET** /api-keys | List Api Keys |
| [**list_api_keys_api_keys_get_0**](APIKeysApi.md#list_api_keys_api_keys_get_0) | **GET** /api-keys | List Api Keys |
| [**repair_user_data_endpoint_api_keys_repair_data_post**](APIKeysApi.md#repair_user_data_endpoint_api_keys_repair_data_post) | **POST** /api-keys/repair-data | Repair User Data Endpoint |
| [**repair_user_data_endpoint_api_keys_repair_data_post_0**](APIKeysApi.md#repair_user_data_endpoint_api_keys_repair_data_post_0) | **POST** /api-keys/repair-data | Repair User Data Endpoint |
| [**revoke_api_key_api_keys_key_hash_revoke_delete**](APIKeysApi.md#revoke_api_key_api_keys_key_hash_revoke_delete) | **DELETE** /api-keys/{key_hash}/revoke | Revoke Api Key |
| [**revoke_api_key_api_keys_key_hash_revoke_delete_0**](APIKeysApi.md#revoke_api_key_api_keys_key_hash_revoke_delete_0) | **DELETE** /api-keys/{key_hash}/revoke | Revoke Api Key |
| [**rotate_api_key_api_keys_key_hash_rotate_post**](APIKeysApi.md#rotate_api_key_api_keys_key_hash_rotate_post) | **POST** /api-keys/{key_hash}/rotate | Rotate Api Key |
| [**rotate_api_key_api_keys_key_hash_rotate_post_0**](APIKeysApi.md#rotate_api_key_api_keys_key_hash_rotate_post_0) | **POST** /api-keys/{key_hash}/rotate | Rotate Api Key |
| [**sync_plan_keys_api_keys_sync_plan_keys_post**](APIKeysApi.md#sync_plan_keys_api_keys_sync_plan_keys_post) | **POST** /api-keys/sync-plan-keys | Sync Plan Keys |
| [**sync_plan_keys_api_keys_sync_plan_keys_post_0**](APIKeysApi.md#sync_plan_keys_api_keys_sync_plan_keys_post_0) | **POST** /api-keys/sync-plan-keys | Sync Plan Keys |


## create_api_key_api_keys_post

> Object create_api_key_api_keys_post(api_key_create_request)

Create Api Key

Create a new API key with atomic transaction. Generates cryptographically secure API keys with proper scoping based on user's current plan. Enforces maximum key limits.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new
api_key_create_request = MailSafePro::APIKeyCreateRequest.new # APIKeyCreateRequest | 

begin
  # Create Api Key
  result = api_instance.create_api_key_api_keys_post(api_key_create_request)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->create_api_key_api_keys_post: #{e}"
end
```

#### Using the create_api_key_api_keys_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> create_api_key_api_keys_post_with_http_info(api_key_create_request)

```ruby
begin
  # Create Api Key
  data, status_code, headers = api_instance.create_api_key_api_keys_post_with_http_info(api_key_create_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->create_api_key_api_keys_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_key_create_request** | [**APIKeyCreateRequest**](APIKeyCreateRequest.md) |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## create_api_key_api_keys_post_0

> Object create_api_key_api_keys_post_0(api_key_create_request)

Create Api Key

Create a new API key with atomic transaction. Generates cryptographically secure API keys with proper scoping based on user's current plan. Enforces maximum key limits.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new
api_key_create_request = MailSafePro::APIKeyCreateRequest.new # APIKeyCreateRequest | 

begin
  # Create Api Key
  result = api_instance.create_api_key_api_keys_post_0(api_key_create_request)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->create_api_key_api_keys_post_0: #{e}"
end
```

#### Using the create_api_key_api_keys_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> create_api_key_api_keys_post_0_with_http_info(api_key_create_request)

```ruby
begin
  # Create Api Key
  data, status_code, headers = api_instance.create_api_key_api_keys_post_0_with_http_info(api_key_create_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->create_api_key_api_keys_post_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_key_create_request** | [**APIKeyCreateRequest**](APIKeyCreateRequest.md) |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## force_sync_api_keys_force_sync_post

> Object force_sync_api_keys_force_sync_post

Force Sync

Force synchronization of user data with rate limiting. Synchronizes API keys with current plan and clears relevant caches. Limited to one sync per 5 minutes per user.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new

begin
  # Force Sync
  result = api_instance.force_sync_api_keys_force_sync_post
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->force_sync_api_keys_force_sync_post: #{e}"
end
```

#### Using the force_sync_api_keys_force_sync_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> force_sync_api_keys_force_sync_post_with_http_info

```ruby
begin
  # Force Sync
  data, status_code, headers = api_instance.force_sync_api_keys_force_sync_post_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->force_sync_api_keys_force_sync_post_with_http_info: #{e}"
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


## force_sync_api_keys_force_sync_post_0

> Object force_sync_api_keys_force_sync_post_0

Force Sync

Force synchronization of user data with rate limiting. Synchronizes API keys with current plan and clears relevant caches. Limited to one sync per 5 minutes per user.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new

begin
  # Force Sync
  result = api_instance.force_sync_api_keys_force_sync_post_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->force_sync_api_keys_force_sync_post_0: #{e}"
end
```

#### Using the force_sync_api_keys_force_sync_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> force_sync_api_keys_force_sync_post_0_with_http_info

```ruby
begin
  # Force Sync
  data, status_code, headers = api_instance.force_sync_api_keys_force_sync_post_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->force_sync_api_keys_force_sync_post_0_with_http_info: #{e}"
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


## get_api_key_value_api_keys_key_hash_value_get

> Object get_api_key_value_api_keys_key_hash_value_get(key_hash)

Get Api Key Value

Retrieve API key metadata (security-safe). Returns key information without exposing the actual key value. Used for key management and verification purposes.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new
key_hash = 'key_hash_example' # String | 

begin
  # Get Api Key Value
  result = api_instance.get_api_key_value_api_keys_key_hash_value_get(key_hash)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->get_api_key_value_api_keys_key_hash_value_get: #{e}"
end
```

#### Using the get_api_key_value_api_keys_key_hash_value_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> get_api_key_value_api_keys_key_hash_value_get_with_http_info(key_hash)

```ruby
begin
  # Get Api Key Value
  data, status_code, headers = api_instance.get_api_key_value_api_keys_key_hash_value_get_with_http_info(key_hash)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->get_api_key_value_api_keys_key_hash_value_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **key_hash** | **String** |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_api_key_value_api_keys_key_hash_value_get_0

> Object get_api_key_value_api_keys_key_hash_value_get_0(key_hash)

Get Api Key Value

Retrieve API key metadata (security-safe). Returns key information without exposing the actual key value. Used for key management and verification purposes.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new
key_hash = 'key_hash_example' # String | 

begin
  # Get Api Key Value
  result = api_instance.get_api_key_value_api_keys_key_hash_value_get_0(key_hash)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->get_api_key_value_api_keys_key_hash_value_get_0: #{e}"
end
```

#### Using the get_api_key_value_api_keys_key_hash_value_get_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> get_api_key_value_api_keys_key_hash_value_get_0_with_http_info(key_hash)

```ruby
begin
  # Get Api Key Value
  data, status_code, headers = api_instance.get_api_key_value_api_keys_key_hash_value_get_0_with_http_info(key_hash)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->get_api_key_value_api_keys_key_hash_value_get_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **key_hash** | **String** |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_usage_api_keys_usage_get

> Object get_usage_api_keys_usage_get(opts)

Get Usage

Get current API usage statistics. Returns usage count, limits, and remaining requests for today. Works with both API keys and JWT tokens.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::APIKeysApi.new
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Get Usage
  result = api_instance.get_usage_api_keys_usage_get(opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->get_usage_api_keys_usage_get: #{e}"
end
```

#### Using the get_usage_api_keys_usage_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> get_usage_api_keys_usage_get_with_http_info(opts)

```ruby
begin
  # Get Usage
  data, status_code, headers = api_instance.get_usage_api_keys_usage_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->get_usage_api_keys_usage_get_with_http_info: #{e}"
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


## get_usage_api_keys_usage_get_0

> Object get_usage_api_keys_usage_get_0(opts)

Get Usage

Get current API usage statistics. Returns usage count, limits, and remaining requests for today. Works with both API keys and JWT tokens.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::APIKeysApi.new
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Get Usage
  result = api_instance.get_usage_api_keys_usage_get_0(opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->get_usage_api_keys_usage_get_0: #{e}"
end
```

#### Using the get_usage_api_keys_usage_get_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> get_usage_api_keys_usage_get_0_with_http_info(opts)

```ruby
begin
  # Get Usage
  data, status_code, headers = api_instance.get_usage_api_keys_usage_get_0_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->get_usage_api_keys_usage_get_0_with_http_info: #{e}"
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


## list_api_keys_api_keys_get

> <APIKeyListResponse> list_api_keys_api_keys_get

List Api Keys

List all API keys for current user with consistent IDs. Returns comprehensive key metadata including status, scopes, and usage information. Handles corrupted key data gracefully.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new

begin
  # List Api Keys
  result = api_instance.list_api_keys_api_keys_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->list_api_keys_api_keys_get: #{e}"
end
```

#### Using the list_api_keys_api_keys_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<APIKeyListResponse>, Integer, Hash)> list_api_keys_api_keys_get_with_http_info

```ruby
begin
  # List Api Keys
  data, status_code, headers = api_instance.list_api_keys_api_keys_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <APIKeyListResponse>
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->list_api_keys_api_keys_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**APIKeyListResponse**](APIKeyListResponse.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_api_keys_api_keys_get_0

> <APIKeyListResponse> list_api_keys_api_keys_get_0

List Api Keys

List all API keys for current user with consistent IDs. Returns comprehensive key metadata including status, scopes, and usage information. Handles corrupted key data gracefully.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new

begin
  # List Api Keys
  result = api_instance.list_api_keys_api_keys_get_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->list_api_keys_api_keys_get_0: #{e}"
end
```

#### Using the list_api_keys_api_keys_get_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<APIKeyListResponse>, Integer, Hash)> list_api_keys_api_keys_get_0_with_http_info

```ruby
begin
  # List Api Keys
  data, status_code, headers = api_instance.list_api_keys_api_keys_get_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <APIKeyListResponse>
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->list_api_keys_api_keys_get_0_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**APIKeyListResponse**](APIKeyListResponse.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## repair_user_data_endpoint_api_keys_repair_data_post

> Hash&lt;String, String&gt; repair_user_data_endpoint_api_keys_repair_data_post

Repair User Data Endpoint

Emergency data repair endpoint - ADMINISTRATORS ONLY WARNING: Critical operation; relies on admin scope verification at runtime.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new

begin
  # Repair User Data Endpoint
  result = api_instance.repair_user_data_endpoint_api_keys_repair_data_post
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->repair_user_data_endpoint_api_keys_repair_data_post: #{e}"
end
```

#### Using the repair_user_data_endpoint_api_keys_repair_data_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Hash&lt;String, String&gt;, Integer, Hash)> repair_user_data_endpoint_api_keys_repair_data_post_with_http_info

```ruby
begin
  # Repair User Data Endpoint
  data, status_code, headers = api_instance.repair_user_data_endpoint_api_keys_repair_data_post_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Hash&lt;String, String&gt;
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->repair_user_data_endpoint_api_keys_repair_data_post_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

**Hash&lt;String, String&gt;**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## repair_user_data_endpoint_api_keys_repair_data_post_0

> Hash&lt;String, String&gt; repair_user_data_endpoint_api_keys_repair_data_post_0

Repair User Data Endpoint

Emergency data repair endpoint - ADMINISTRATORS ONLY WARNING: Critical operation; relies on admin scope verification at runtime.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new

begin
  # Repair User Data Endpoint
  result = api_instance.repair_user_data_endpoint_api_keys_repair_data_post_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->repair_user_data_endpoint_api_keys_repair_data_post_0: #{e}"
end
```

#### Using the repair_user_data_endpoint_api_keys_repair_data_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Hash&lt;String, String&gt;, Integer, Hash)> repair_user_data_endpoint_api_keys_repair_data_post_0_with_http_info

```ruby
begin
  # Repair User Data Endpoint
  data, status_code, headers = api_instance.repair_user_data_endpoint_api_keys_repair_data_post_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Hash&lt;String, String&gt;
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->repair_user_data_endpoint_api_keys_repair_data_post_0_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

**Hash&lt;String, String&gt;**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## revoke_api_key_api_keys_key_hash_revoke_delete

> Object revoke_api_key_api_keys_key_hash_revoke_delete(key_hash)

Revoke Api Key

Revoke an API key with atomic transaction. Immediately invalidates the key and removes it from active sets. Provides audit trail for security compliance.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new
key_hash = 'key_hash_example' # String | 

begin
  # Revoke Api Key
  result = api_instance.revoke_api_key_api_keys_key_hash_revoke_delete(key_hash)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->revoke_api_key_api_keys_key_hash_revoke_delete: #{e}"
end
```

#### Using the revoke_api_key_api_keys_key_hash_revoke_delete_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> revoke_api_key_api_keys_key_hash_revoke_delete_with_http_info(key_hash)

```ruby
begin
  # Revoke Api Key
  data, status_code, headers = api_instance.revoke_api_key_api_keys_key_hash_revoke_delete_with_http_info(key_hash)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->revoke_api_key_api_keys_key_hash_revoke_delete_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **key_hash** | **String** |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## revoke_api_key_api_keys_key_hash_revoke_delete_0

> Object revoke_api_key_api_keys_key_hash_revoke_delete_0(key_hash)

Revoke Api Key

Revoke an API key with atomic transaction. Immediately invalidates the key and removes it from active sets. Provides audit trail for security compliance.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new
key_hash = 'key_hash_example' # String | 

begin
  # Revoke Api Key
  result = api_instance.revoke_api_key_api_keys_key_hash_revoke_delete_0(key_hash)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->revoke_api_key_api_keys_key_hash_revoke_delete_0: #{e}"
end
```

#### Using the revoke_api_key_api_keys_key_hash_revoke_delete_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> revoke_api_key_api_keys_key_hash_revoke_delete_0_with_http_info(key_hash)

```ruby
begin
  # Revoke Api Key
  data, status_code, headers = api_instance.revoke_api_key_api_keys_key_hash_revoke_delete_0_with_http_info(key_hash)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->revoke_api_key_api_keys_key_hash_revoke_delete_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **key_hash** | **String** |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## rotate_api_key_api_keys_key_hash_rotate_post

> Object rotate_api_key_api_keys_key_hash_rotate_post(key_hash)

Rotate Api Key

Rotate API key with grace period. Generates a new key while keeping the old one active for 7 days to allow for smooth transition in client applications.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new
key_hash = 'key_hash_example' # String | 

begin
  # Rotate Api Key
  result = api_instance.rotate_api_key_api_keys_key_hash_rotate_post(key_hash)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->rotate_api_key_api_keys_key_hash_rotate_post: #{e}"
end
```

#### Using the rotate_api_key_api_keys_key_hash_rotate_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> rotate_api_key_api_keys_key_hash_rotate_post_with_http_info(key_hash)

```ruby
begin
  # Rotate Api Key
  data, status_code, headers = api_instance.rotate_api_key_api_keys_key_hash_rotate_post_with_http_info(key_hash)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->rotate_api_key_api_keys_key_hash_rotate_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **key_hash** | **String** |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## rotate_api_key_api_keys_key_hash_rotate_post_0

> Object rotate_api_key_api_keys_key_hash_rotate_post_0(key_hash)

Rotate Api Key

Rotate API key with grace period. Generates a new key while keeping the old one active for 7 days to allow for smooth transition in client applications.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new
key_hash = 'key_hash_example' # String | 

begin
  # Rotate Api Key
  result = api_instance.rotate_api_key_api_keys_key_hash_rotate_post_0(key_hash)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->rotate_api_key_api_keys_key_hash_rotate_post_0: #{e}"
end
```

#### Using the rotate_api_key_api_keys_key_hash_rotate_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> rotate_api_key_api_keys_key_hash_rotate_post_0_with_http_info(key_hash)

```ruby
begin
  # Rotate Api Key
  data, status_code, headers = api_instance.rotate_api_key_api_keys_key_hash_rotate_post_0_with_http_info(key_hash)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->rotate_api_key_api_keys_key_hash_rotate_post_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **key_hash** | **String** |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## sync_plan_keys_api_keys_sync_plan_keys_post

> Object sync_plan_keys_api_keys_sync_plan_keys_post

Sync Plan Keys

Synchronize current plan with all user API keys. Ensures all existing keys have the correct scopes and permissions based on the user's current subscription plan.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new

begin
  # Sync Plan Keys
  result = api_instance.sync_plan_keys_api_keys_sync_plan_keys_post
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->sync_plan_keys_api_keys_sync_plan_keys_post: #{e}"
end
```

#### Using the sync_plan_keys_api_keys_sync_plan_keys_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> sync_plan_keys_api_keys_sync_plan_keys_post_with_http_info

```ruby
begin
  # Sync Plan Keys
  data, status_code, headers = api_instance.sync_plan_keys_api_keys_sync_plan_keys_post_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->sync_plan_keys_api_keys_sync_plan_keys_post_with_http_info: #{e}"
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


## sync_plan_keys_api_keys_sync_plan_keys_post_0

> Object sync_plan_keys_api_keys_sync_plan_keys_post_0

Sync Plan Keys

Synchronize current plan with all user API keys. Ensures all existing keys have the correct scopes and permissions based on the user's current subscription plan.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::APIKeysApi.new

begin
  # Sync Plan Keys
  result = api_instance.sync_plan_keys_api_keys_sync_plan_keys_post_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->sync_plan_keys_api_keys_sync_plan_keys_post_0: #{e}"
end
```

#### Using the sync_plan_keys_api_keys_sync_plan_keys_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> sync_plan_keys_api_keys_sync_plan_keys_post_0_with_http_info

```ruby
begin
  # Sync Plan Keys
  data, status_code, headers = api_instance.sync_plan_keys_api_keys_sync_plan_keys_post_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling APIKeysApi->sync_plan_keys_api_keys_sync_plan_keys_post_0_with_http_info: #{e}"
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

