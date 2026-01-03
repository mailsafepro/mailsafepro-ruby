# MailSafePro::HealthApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**basic_health_health_get**](HealthApi.md#basic_health_health_get) | **GET** /health | Basic health check |
| [**basic_health_health_get_0**](HealthApi.md#basic_health_health_get_0) | **GET** /health | Basic health check |
| [**circuit_breaker_status_admin_circuit_breaker_status_get**](HealthApi.md#circuit_breaker_status_admin_circuit_breaker_status_get) | **GET** /admin/circuit-breaker-status | Circuit Breaker Status |
| [**detailed_health_health_detailed_get**](HealthApi.md#detailed_health_health_detailed_get) | **GET** /health/detailed | Detailed health check |
| [**detailed_health_health_detailed_get_0**](HealthApi.md#detailed_health_health_detailed_get_0) | **GET** /health/detailed | Detailed health check |
| [**healthcheck_healthcheck_get**](HealthApi.md#healthcheck_healthcheck_get) | **GET** /healthcheck | Healthcheck |
| [**healthcheck_healthcheck_head**](HealthApi.md#healthcheck_healthcheck_head) | **HEAD** /healthcheck | Healthcheck |
| [**liveness_check_health_liveness_get**](HealthApi.md#liveness_check_health_liveness_get) | **GET** /health/liveness | Liveness Check |
| [**liveness_health_live_get**](HealthApi.md#liveness_health_live_get) | **GET** /health/live | Liveness probe (Kubernetes) |
| [**liveness_health_live_get_0**](HealthApi.md#liveness_health_live_get_0) | **GET** /health/live | Liveness probe (Kubernetes) |
| [**readiness_check_health_readiness_get**](HealthApi.md#readiness_check_health_readiness_get) | **GET** /health/readiness | Readiness Check |
| [**readiness_health_ready_get**](HealthApi.md#readiness_health_ready_get) | **GET** /health/ready | Readiness probe (Kubernetes) |
| [**readiness_health_ready_get_0**](HealthApi.md#readiness_health_ready_get_0) | **GET** /health/ready | Readiness probe (Kubernetes) |
| [**service_status_status_get**](HealthApi.md#service_status_status_get) | **GET** /status | Service Status |
| [**startup_check_health_startup_get**](HealthApi.md#startup_check_health_startup_get) | **GET** /health/startup | Startup Check |


## basic_health_health_get

> Object basic_health_health_get

Basic health check

Basic health check for load balancers.  Returns 200 if service is running. Fast response, no dependency checks.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Basic health check
  result = api_instance.basic_health_health_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->basic_health_health_get: #{e}"
end
```

#### Using the basic_health_health_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> basic_health_health_get_with_http_info

```ruby
begin
  # Basic health check
  data, status_code, headers = api_instance.basic_health_health_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->basic_health_health_get_with_http_info: #{e}"
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


## basic_health_health_get_0

> Object basic_health_health_get_0

Basic health check

Basic health check for load balancers.  Returns 200 if service is running. Fast response, no dependency checks.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Basic health check
  result = api_instance.basic_health_health_get_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->basic_health_health_get_0: #{e}"
end
```

#### Using the basic_health_health_get_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> basic_health_health_get_0_with_http_info

```ruby
begin
  # Basic health check
  data, status_code, headers = api_instance.basic_health_health_get_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->basic_health_health_get_0_with_http_info: #{e}"
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


## circuit_breaker_status_admin_circuit_breaker_status_get

> Object circuit_breaker_status_admin_circuit_breaker_status_get

Circuit Breaker Status

✅ Circuit breaker status for all services. Shows state of Redis, SMTP, DNS, and other circuit breakers.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Circuit Breaker Status
  result = api_instance.circuit_breaker_status_admin_circuit_breaker_status_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->circuit_breaker_status_admin_circuit_breaker_status_get: #{e}"
end
```

#### Using the circuit_breaker_status_admin_circuit_breaker_status_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> circuit_breaker_status_admin_circuit_breaker_status_get_with_http_info

```ruby
begin
  # Circuit Breaker Status
  data, status_code, headers = api_instance.circuit_breaker_status_admin_circuit_breaker_status_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->circuit_breaker_status_admin_circuit_breaker_status_get_with_http_info: #{e}"
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


## detailed_health_health_detailed_get

> Object detailed_health_health_detailed_get

Detailed health check

Detailed health check with all component statuses.  Returns comprehensive health information for monitoring.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Detailed health check
  result = api_instance.detailed_health_health_detailed_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->detailed_health_health_detailed_get: #{e}"
end
```

#### Using the detailed_health_health_detailed_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> detailed_health_health_detailed_get_with_http_info

```ruby
begin
  # Detailed health check
  data, status_code, headers = api_instance.detailed_health_health_detailed_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->detailed_health_health_detailed_get_with_http_info: #{e}"
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


## detailed_health_health_detailed_get_0

> Object detailed_health_health_detailed_get_0

Detailed health check

Detailed health check with all component statuses.  Returns comprehensive health information for monitoring.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Detailed health check
  result = api_instance.detailed_health_health_detailed_get_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->detailed_health_health_detailed_get_0: #{e}"
end
```

#### Using the detailed_health_health_detailed_get_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> detailed_health_health_detailed_get_0_with_http_info

```ruby
begin
  # Detailed health check
  data, status_code, headers = api_instance.detailed_health_health_detailed_get_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->detailed_health_health_detailed_get_0_with_http_info: #{e}"
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


## healthcheck_healthcheck_get

> Object healthcheck_healthcheck_get

Healthcheck

Basic health check endpoint (backward compatibility)

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Healthcheck
  result = api_instance.healthcheck_healthcheck_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->healthcheck_healthcheck_get: #{e}"
end
```

#### Using the healthcheck_healthcheck_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> healthcheck_healthcheck_get_with_http_info

```ruby
begin
  # Healthcheck
  data, status_code, headers = api_instance.healthcheck_healthcheck_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->healthcheck_healthcheck_get_with_http_info: #{e}"
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


## healthcheck_healthcheck_head

> Object healthcheck_healthcheck_head

Healthcheck

Basic health check endpoint (backward compatibility)

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Healthcheck
  result = api_instance.healthcheck_healthcheck_head
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->healthcheck_healthcheck_head: #{e}"
end
```

#### Using the healthcheck_healthcheck_head_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> healthcheck_healthcheck_head_with_http_info

```ruby
begin
  # Healthcheck
  data, status_code, headers = api_instance.healthcheck_healthcheck_head_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->healthcheck_healthcheck_head_with_http_info: #{e}"
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


## liveness_check_health_liveness_get

> Object liveness_check_health_liveness_get

Liveness Check

✅ MEJORA: Kubernetes liveness probe  Returns 200 if the application is alive (not deadlocked) Used by Kubernetes to restart the pod if unhealthy

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Liveness Check
  result = api_instance.liveness_check_health_liveness_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->liveness_check_health_liveness_get: #{e}"
end
```

#### Using the liveness_check_health_liveness_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> liveness_check_health_liveness_get_with_http_info

```ruby
begin
  # Liveness Check
  data, status_code, headers = api_instance.liveness_check_health_liveness_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->liveness_check_health_liveness_get_with_http_info: #{e}"
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


## liveness_health_live_get

> Object liveness_health_live_get

Liveness probe (Kubernetes)

Kubernetes liveness probe.  Returns 200 if the application is running. Should restart pod if this fails.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Liveness probe (Kubernetes)
  result = api_instance.liveness_health_live_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->liveness_health_live_get: #{e}"
end
```

#### Using the liveness_health_live_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> liveness_health_live_get_with_http_info

```ruby
begin
  # Liveness probe (Kubernetes)
  data, status_code, headers = api_instance.liveness_health_live_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->liveness_health_live_get_with_http_info: #{e}"
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


## liveness_health_live_get_0

> Object liveness_health_live_get_0

Liveness probe (Kubernetes)

Kubernetes liveness probe.  Returns 200 if the application is running. Should restart pod if this fails.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Liveness probe (Kubernetes)
  result = api_instance.liveness_health_live_get_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->liveness_health_live_get_0: #{e}"
end
```

#### Using the liveness_health_live_get_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> liveness_health_live_get_0_with_http_info

```ruby
begin
  # Liveness probe (Kubernetes)
  data, status_code, headers = api_instance.liveness_health_live_get_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->liveness_health_live_get_0_with_http_info: #{e}"
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


## readiness_check_health_readiness_get

> Object readiness_check_health_readiness_get

Readiness Check

✅ MEJORA: Kubernetes readiness probe  Returns 200 if the application is ready to serve traffic Checks all critical dependencies (PostgreSQL, Redis, ARQ)

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Readiness Check
  result = api_instance.readiness_check_health_readiness_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->readiness_check_health_readiness_get: #{e}"
end
```

#### Using the readiness_check_health_readiness_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> readiness_check_health_readiness_get_with_http_info

```ruby
begin
  # Readiness Check
  data, status_code, headers = api_instance.readiness_check_health_readiness_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->readiness_check_health_readiness_get_with_http_info: #{e}"
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


## readiness_health_ready_get

> Object readiness_health_ready_get

Readiness probe (Kubernetes)

Kubernetes readiness probe.  Returns 200 if service is ready to accept traffic. Checks critical dependencies (Redis).

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Readiness probe (Kubernetes)
  result = api_instance.readiness_health_ready_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->readiness_health_ready_get: #{e}"
end
```

#### Using the readiness_health_ready_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> readiness_health_ready_get_with_http_info

```ruby
begin
  # Readiness probe (Kubernetes)
  data, status_code, headers = api_instance.readiness_health_ready_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->readiness_health_ready_get_with_http_info: #{e}"
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


## readiness_health_ready_get_0

> Object readiness_health_ready_get_0

Readiness probe (Kubernetes)

Kubernetes readiness probe.  Returns 200 if service is ready to accept traffic. Checks critical dependencies (Redis).

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Readiness probe (Kubernetes)
  result = api_instance.readiness_health_ready_get_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->readiness_health_ready_get_0: #{e}"
end
```

#### Using the readiness_health_ready_get_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> readiness_health_ready_get_0_with_http_info

```ruby
begin
  # Readiness probe (Kubernetes)
  data, status_code, headers = api_instance.readiness_health_ready_get_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->readiness_health_ready_get_0_with_http_info: #{e}"
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


## service_status_status_get

> Object service_status_status_get

Service Status

✅ MEJORA: Detailed service status with feature flags  Shows which features are available and which are running in degraded mode

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Service Status
  result = api_instance.service_status_status_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->service_status_status_get: #{e}"
end
```

#### Using the service_status_status_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> service_status_status_get_with_http_info

```ruby
begin
  # Service Status
  data, status_code, headers = api_instance.service_status_status_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->service_status_status_get_with_http_info: #{e}"
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


## startup_check_health_startup_get

> Object startup_check_health_startup_get

Startup Check

✅ MEJORA: Kubernetes startup probe  Returns 200 once the application has completed startup Used to delay readiness checks until startup is complete

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::HealthApi.new

begin
  # Startup Check
  result = api_instance.startup_check_health_startup_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->startup_check_health_startup_get: #{e}"
end
```

#### Using the startup_check_health_startup_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> startup_check_health_startup_get_with_http_info

```ruby
begin
  # Startup Check
  data, status_code, headers = api_instance.startup_check_health_startup_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling HealthApi->startup_check_health_startup_get_with_http_info: #{e}"
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

