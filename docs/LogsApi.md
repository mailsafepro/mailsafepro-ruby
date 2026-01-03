# MailSafePro::LogsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**clear_request_logs_logs_logs_requests_delete**](LogsApi.md#clear_request_logs_logs_logs_requests_delete) | **DELETE** /logs/logs/requests | Clear Request Logs |
| [**get_request_logs_logs_logs_requests_get**](LogsApi.md#get_request_logs_logs_logs_requests_get) | **GET** /logs/logs/requests | Get Request Logs |


## clear_request_logs_logs_logs_requests_delete

> Object clear_request_logs_logs_logs_requests_delete

Clear Request Logs

Clear all request logs for current user.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::LogsApi.new

begin
  # Clear Request Logs
  result = api_instance.clear_request_logs_logs_logs_requests_delete
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling LogsApi->clear_request_logs_logs_logs_requests_delete: #{e}"
end
```

#### Using the clear_request_logs_logs_logs_requests_delete_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> clear_request_logs_logs_logs_requests_delete_with_http_info

```ruby
begin
  # Clear Request Logs
  data, status_code, headers = api_instance.clear_request_logs_logs_logs_requests_delete_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling LogsApi->clear_request_logs_logs_logs_requests_delete_with_http_info: #{e}"
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


## get_request_logs_logs_logs_requests_get

> Object get_request_logs_logs_logs_requests_get(opts)

Get Request Logs

Get request logs for authenticated user.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::LogsApi.new
opts = {
  limit: 56, # Integer | Max results to return
  status_code: 56, # Integer | Filter by HTTP status code
  endpoint: 'endpoint_example', # String | Filter by endpoint path
  method: 'method_example', # String | Filter by HTTP method (GET, POST, etc)
  since: Time.parse('2013-10-20T19:20:30+01:00') # Time | Filter by timestamp (ISO 8601)
}

begin
  # Get Request Logs
  result = api_instance.get_request_logs_logs_logs_requests_get(opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling LogsApi->get_request_logs_logs_logs_requests_get: #{e}"
end
```

#### Using the get_request_logs_logs_logs_requests_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> get_request_logs_logs_logs_requests_get_with_http_info(opts)

```ruby
begin
  # Get Request Logs
  data, status_code, headers = api_instance.get_request_logs_logs_logs_requests_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling LogsApi->get_request_logs_logs_logs_requests_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **limit** | **Integer** | Max results to return | [optional][default to 100] |
| **status_code** | **Integer** | Filter by HTTP status code | [optional] |
| **endpoint** | **String** | Filter by endpoint path | [optional] |
| **method** | **String** | Filter by HTTP method (GET, POST, etc) | [optional] |
| **since** | **Time** | Filter by timestamp (ISO 8601) | [optional] |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

