# MailSafePro::JobsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_job_jobs_v1_jobs_post**](JobsApi.md#create_job_jobs_v1_jobs_post) | **POST** /jobs/v1/jobs | Create validation job |
| [**create_job_jobs_v1_jobs_post_0**](JobsApi.md#create_job_jobs_v1_jobs_post_0) | **POST** /jobs/v1/jobs | Create validation job |
| [**get_job_results_jobs_v1_jobs_job_id_results_get**](JobsApi.md#get_job_results_jobs_v1_jobs_job_id_results_get) | **GET** /jobs/v1/jobs/{job_id}/results | Get job results (paged) |
| [**get_job_results_jobs_v1_jobs_job_id_results_get_0**](JobsApi.md#get_job_results_jobs_v1_jobs_job_id_results_get_0) | **GET** /jobs/v1/jobs/{job_id}/results | Get job results (paged) |
| [**get_job_status_jobs_v1_jobs_job_id_get**](JobsApi.md#get_job_status_jobs_v1_jobs_job_id_get) | **GET** /jobs/v1/jobs/{job_id} | Get job status |
| [**get_job_status_jobs_v1_jobs_job_id_get_0**](JobsApi.md#get_job_status_jobs_v1_jobs_job_id_get_0) | **GET** /jobs/v1/jobs/{job_id} | Get job status |


## create_job_jobs_v1_jobs_post

> <JobCreateResponse> create_job_jobs_v1_jobs_post(job_create_request, opts)

Create validation job

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::JobsApi.new
job_create_request = MailSafePro::JobCreateRequest.new({source: 'source_example'}) # JobCreateRequest | 
opts = {
  x_idempotency_key: 'x_idempotency_key_example', # String | 
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Create validation job
  result = api_instance.create_job_jobs_v1_jobs_post(job_create_request, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling JobsApi->create_job_jobs_v1_jobs_post: #{e}"
end
```

#### Using the create_job_jobs_v1_jobs_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobCreateResponse>, Integer, Hash)> create_job_jobs_v1_jobs_post_with_http_info(job_create_request, opts)

```ruby
begin
  # Create validation job
  data, status_code, headers = api_instance.create_job_jobs_v1_jobs_post_with_http_info(job_create_request, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobCreateResponse>
rescue MailSafePro::ApiError => e
  puts "Error when calling JobsApi->create_job_jobs_v1_jobs_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **job_create_request** | [**JobCreateRequest**](JobCreateRequest.md) |  |  |
| **x_idempotency_key** | **String** |  | [optional] |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

[**JobCreateResponse**](JobCreateResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## create_job_jobs_v1_jobs_post_0

> <JobCreateResponse> create_job_jobs_v1_jobs_post_0(job_create_request, opts)

Create validation job

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::JobsApi.new
job_create_request = MailSafePro::JobCreateRequest.new({source: 'source_example'}) # JobCreateRequest | 
opts = {
  x_idempotency_key: 'x_idempotency_key_example', # String | 
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Create validation job
  result = api_instance.create_job_jobs_v1_jobs_post_0(job_create_request, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling JobsApi->create_job_jobs_v1_jobs_post_0: #{e}"
end
```

#### Using the create_job_jobs_v1_jobs_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobCreateResponse>, Integer, Hash)> create_job_jobs_v1_jobs_post_0_with_http_info(job_create_request, opts)

```ruby
begin
  # Create validation job
  data, status_code, headers = api_instance.create_job_jobs_v1_jobs_post_0_with_http_info(job_create_request, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobCreateResponse>
rescue MailSafePro::ApiError => e
  puts "Error when calling JobsApi->create_job_jobs_v1_jobs_post_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **job_create_request** | [**JobCreateRequest**](JobCreateRequest.md) |  |  |
| **x_idempotency_key** | **String** |  | [optional] |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

[**JobCreateResponse**](JobCreateResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## get_job_results_jobs_v1_jobs_job_id_results_get

> <JobResultsPage> get_job_results_jobs_v1_jobs_job_id_results_get(job_id, opts)

Get job results (paged)

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::JobsApi.new
job_id = 'job_id_example' # String | 
opts = {
  page: 56, # Integer | 
  size: 56, # Integer | 
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Get job results (paged)
  result = api_instance.get_job_results_jobs_v1_jobs_job_id_results_get(job_id, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling JobsApi->get_job_results_jobs_v1_jobs_job_id_results_get: #{e}"
end
```

#### Using the get_job_results_jobs_v1_jobs_job_id_results_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobResultsPage>, Integer, Hash)> get_job_results_jobs_v1_jobs_job_id_results_get_with_http_info(job_id, opts)

```ruby
begin
  # Get job results (paged)
  data, status_code, headers = api_instance.get_job_results_jobs_v1_jobs_job_id_results_get_with_http_info(job_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobResultsPage>
rescue MailSafePro::ApiError => e
  puts "Error when calling JobsApi->get_job_results_jobs_v1_jobs_job_id_results_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **job_id** | **String** |  |  |
| **page** | **Integer** |  | [optional][default to 1] |
| **size** | **Integer** |  | [optional][default to 500] |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

[**JobResultsPage**](JobResultsPage.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_job_results_jobs_v1_jobs_job_id_results_get_0

> <JobResultsPage> get_job_results_jobs_v1_jobs_job_id_results_get_0(job_id, opts)

Get job results (paged)

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::JobsApi.new
job_id = 'job_id_example' # String | 
opts = {
  page: 56, # Integer | 
  size: 56, # Integer | 
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Get job results (paged)
  result = api_instance.get_job_results_jobs_v1_jobs_job_id_results_get_0(job_id, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling JobsApi->get_job_results_jobs_v1_jobs_job_id_results_get_0: #{e}"
end
```

#### Using the get_job_results_jobs_v1_jobs_job_id_results_get_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobResultsPage>, Integer, Hash)> get_job_results_jobs_v1_jobs_job_id_results_get_0_with_http_info(job_id, opts)

```ruby
begin
  # Get job results (paged)
  data, status_code, headers = api_instance.get_job_results_jobs_v1_jobs_job_id_results_get_0_with_http_info(job_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobResultsPage>
rescue MailSafePro::ApiError => e
  puts "Error when calling JobsApi->get_job_results_jobs_v1_jobs_job_id_results_get_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **job_id** | **String** |  |  |
| **page** | **Integer** |  | [optional][default to 1] |
| **size** | **Integer** |  | [optional][default to 500] |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

[**JobResultsPage**](JobResultsPage.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_job_status_jobs_v1_jobs_job_id_get

> <JobStatusResponse> get_job_status_jobs_v1_jobs_job_id_get(job_id, opts)

Get job status

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::JobsApi.new
job_id = 'job_id_example' # String | 
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Get job status
  result = api_instance.get_job_status_jobs_v1_jobs_job_id_get(job_id, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling JobsApi->get_job_status_jobs_v1_jobs_job_id_get: #{e}"
end
```

#### Using the get_job_status_jobs_v1_jobs_job_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobStatusResponse>, Integer, Hash)> get_job_status_jobs_v1_jobs_job_id_get_with_http_info(job_id, opts)

```ruby
begin
  # Get job status
  data, status_code, headers = api_instance.get_job_status_jobs_v1_jobs_job_id_get_with_http_info(job_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobStatusResponse>
rescue MailSafePro::ApiError => e
  puts "Error when calling JobsApi->get_job_status_jobs_v1_jobs_job_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **job_id** | **String** |  |  |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

[**JobStatusResponse**](JobStatusResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_job_status_jobs_v1_jobs_job_id_get_0

> <JobStatusResponse> get_job_status_jobs_v1_jobs_job_id_get_0(job_id, opts)

Get job status

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::JobsApi.new
job_id = 'job_id_example' # String | 
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Get job status
  result = api_instance.get_job_status_jobs_v1_jobs_job_id_get_0(job_id, opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling JobsApi->get_job_status_jobs_v1_jobs_job_id_get_0: #{e}"
end
```

#### Using the get_job_status_jobs_v1_jobs_job_id_get_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<JobStatusResponse>, Integer, Hash)> get_job_status_jobs_v1_jobs_job_id_get_0_with_http_info(job_id, opts)

```ruby
begin
  # Get job status
  data, status_code, headers = api_instance.get_job_status_jobs_v1_jobs_job_id_get_0_with_http_info(job_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <JobStatusResponse>
rescue MailSafePro::ApiError => e
  puts "Error when calling JobsApi->get_job_status_jobs_v1_jobs_job_id_get_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **job_id** | **String** |  |  |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

[**JobStatusResponse**](JobStatusResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

