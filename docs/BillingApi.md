# MailSafePro::BillingApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**change_plan_billing_billing_change_plan_post**](BillingApi.md#change_plan_billing_billing_change_plan_post) | **POST** /billing/billing/change-plan | Change Plan |
| [**change_plan_billing_billing_change_plan_post_0**](BillingApi.md#change_plan_billing_billing_change_plan_post_0) | **POST** /billing/billing/change-plan | Change Plan |
| [**create_checkout_session_billing_billing_create_checkout_session_post**](BillingApi.md#create_checkout_session_billing_billing_create_checkout_session_post) | **POST** /billing/billing/create-checkout-session | Create Checkout Session |
| [**create_checkout_session_billing_billing_create_checkout_session_post_0**](BillingApi.md#create_checkout_session_billing_billing_create_checkout_session_post_0) | **POST** /billing/billing/create-checkout-session | Create Checkout Session |
| [**get_subscription_billing_billing_subscription_get**](BillingApi.md#get_subscription_billing_billing_subscription_get) | **GET** /billing/billing/subscription | Get Subscription |
| [**get_subscription_billing_billing_subscription_get_0**](BillingApi.md#get_subscription_billing_billing_subscription_get_0) | **GET** /billing/billing/subscription | Get Subscription |
| [**stripe_webhook_billing_billing_webhook_post**](BillingApi.md#stripe_webhook_billing_billing_webhook_post) | **POST** /billing/billing/webhook | Stripe Webhook |
| [**stripe_webhook_billing_billing_webhook_post_0**](BillingApi.md#stripe_webhook_billing_billing_webhook_post_0) | **POST** /billing/billing/webhook | Stripe Webhook |
| [**test_notification_billing_billing_test_notification_post**](BillingApi.md#test_notification_billing_billing_test_notification_post) | **POST** /billing/billing/test-notification | Test Notification |
| [**test_notification_billing_billing_test_notification_post_0**](BillingApi.md#test_notification_billing_billing_test_notification_post_0) | **POST** /billing/billing/test-notification | Test Notification |


## change_plan_billing_billing_change_plan_post

> Object change_plan_billing_billing_change_plan_post(body_change_plan_billing_billing_change_plan_post)

Change Plan

Cambiar el plan del usuario.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::BillingApi.new
body_change_plan_billing_billing_change_plan_post = MailSafePro::BodyChangePlanBillingBillingChangePlanPost.new({plan: 'plan_example'}) # BodyChangePlanBillingBillingChangePlanPost | 

begin
  # Change Plan
  result = api_instance.change_plan_billing_billing_change_plan_post(body_change_plan_billing_billing_change_plan_post)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->change_plan_billing_billing_change_plan_post: #{e}"
end
```

#### Using the change_plan_billing_billing_change_plan_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> change_plan_billing_billing_change_plan_post_with_http_info(body_change_plan_billing_billing_change_plan_post)

```ruby
begin
  # Change Plan
  data, status_code, headers = api_instance.change_plan_billing_billing_change_plan_post_with_http_info(body_change_plan_billing_billing_change_plan_post)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->change_plan_billing_billing_change_plan_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **body_change_plan_billing_billing_change_plan_post** | [**BodyChangePlanBillingBillingChangePlanPost**](BodyChangePlanBillingBillingChangePlanPost.md) |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## change_plan_billing_billing_change_plan_post_0

> Object change_plan_billing_billing_change_plan_post_0(body_change_plan_billing_billing_change_plan_post)

Change Plan

Cambiar el plan del usuario.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::BillingApi.new
body_change_plan_billing_billing_change_plan_post = MailSafePro::BodyChangePlanBillingBillingChangePlanPost.new({plan: 'plan_example'}) # BodyChangePlanBillingBillingChangePlanPost | 

begin
  # Change Plan
  result = api_instance.change_plan_billing_billing_change_plan_post_0(body_change_plan_billing_billing_change_plan_post)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->change_plan_billing_billing_change_plan_post_0: #{e}"
end
```

#### Using the change_plan_billing_billing_change_plan_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> change_plan_billing_billing_change_plan_post_0_with_http_info(body_change_plan_billing_billing_change_plan_post)

```ruby
begin
  # Change Plan
  data, status_code, headers = api_instance.change_plan_billing_billing_change_plan_post_0_with_http_info(body_change_plan_billing_billing_change_plan_post)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->change_plan_billing_billing_change_plan_post_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **body_change_plan_billing_billing_change_plan_post** | [**BodyChangePlanBillingBillingChangePlanPost**](BodyChangePlanBillingBillingChangePlanPost.md) |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## create_checkout_session_billing_billing_create_checkout_session_post

> <CheckoutSessionResponse> create_checkout_session_billing_billing_create_checkout_session_post(checkout_request)

Create Checkout Session

Crea una checkout session de Stripe para suscripción.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::BillingApi.new
checkout_request = MailSafePro::CheckoutRequest.new({plan: 'plan_example'}) # CheckoutRequest | 

begin
  # Create Checkout Session
  result = api_instance.create_checkout_session_billing_billing_create_checkout_session_post(checkout_request)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->create_checkout_session_billing_billing_create_checkout_session_post: #{e}"
end
```

#### Using the create_checkout_session_billing_billing_create_checkout_session_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CheckoutSessionResponse>, Integer, Hash)> create_checkout_session_billing_billing_create_checkout_session_post_with_http_info(checkout_request)

```ruby
begin
  # Create Checkout Session
  data, status_code, headers = api_instance.create_checkout_session_billing_billing_create_checkout_session_post_with_http_info(checkout_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CheckoutSessionResponse>
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->create_checkout_session_billing_billing_create_checkout_session_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **checkout_request** | [**CheckoutRequest**](CheckoutRequest.md) |  |  |

### Return type

[**CheckoutSessionResponse**](CheckoutSessionResponse.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## create_checkout_session_billing_billing_create_checkout_session_post_0

> <CheckoutSessionResponse> create_checkout_session_billing_billing_create_checkout_session_post_0(checkout_request)

Create Checkout Session

Crea una checkout session de Stripe para suscripción.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::BillingApi.new
checkout_request = MailSafePro::CheckoutRequest.new({plan: 'plan_example'}) # CheckoutRequest | 

begin
  # Create Checkout Session
  result = api_instance.create_checkout_session_billing_billing_create_checkout_session_post_0(checkout_request)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->create_checkout_session_billing_billing_create_checkout_session_post_0: #{e}"
end
```

#### Using the create_checkout_session_billing_billing_create_checkout_session_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<CheckoutSessionResponse>, Integer, Hash)> create_checkout_session_billing_billing_create_checkout_session_post_0_with_http_info(checkout_request)

```ruby
begin
  # Create Checkout Session
  data, status_code, headers = api_instance.create_checkout_session_billing_billing_create_checkout_session_post_0_with_http_info(checkout_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <CheckoutSessionResponse>
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->create_checkout_session_billing_billing_create_checkout_session_post_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **checkout_request** | [**CheckoutRequest**](CheckoutRequest.md) |  |  |

### Return type

[**CheckoutSessionResponse**](CheckoutSessionResponse.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## get_subscription_billing_billing_subscription_get

> <SubscriptionResponse> get_subscription_billing_billing_subscription_get(opts)

Get Subscription

Devuelve información de suscripción (plan y próxima fecha de cobro).

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::BillingApi.new
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Get Subscription
  result = api_instance.get_subscription_billing_billing_subscription_get(opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->get_subscription_billing_billing_subscription_get: #{e}"
end
```

#### Using the get_subscription_billing_billing_subscription_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SubscriptionResponse>, Integer, Hash)> get_subscription_billing_billing_subscription_get_with_http_info(opts)

```ruby
begin
  # Get Subscription
  data, status_code, headers = api_instance.get_subscription_billing_billing_subscription_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SubscriptionResponse>
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->get_subscription_billing_billing_subscription_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

[**SubscriptionResponse**](SubscriptionResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_subscription_billing_billing_subscription_get_0

> <SubscriptionResponse> get_subscription_billing_billing_subscription_get_0(opts)

Get Subscription

Devuelve información de suscripción (plan y próxima fecha de cobro).

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::BillingApi.new
opts = {
  x_api_key: 'x_api_key_example', # String | 
  authorization: 'authorization_example' # String | 
}

begin
  # Get Subscription
  result = api_instance.get_subscription_billing_billing_subscription_get_0(opts)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->get_subscription_billing_billing_subscription_get_0: #{e}"
end
```

#### Using the get_subscription_billing_billing_subscription_get_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<SubscriptionResponse>, Integer, Hash)> get_subscription_billing_billing_subscription_get_0_with_http_info(opts)

```ruby
begin
  # Get Subscription
  data, status_code, headers = api_instance.get_subscription_billing_billing_subscription_get_0_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <SubscriptionResponse>
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->get_subscription_billing_billing_subscription_get_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **x_api_key** | **String** |  | [optional] |
| **authorization** | **String** |  | [optional] |

### Return type

[**SubscriptionResponse**](SubscriptionResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## stripe_webhook_billing_billing_webhook_post

> <WebhookResponse> stripe_webhook_billing_billing_webhook_post

Stripe Webhook

Webhook de Stripe.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::BillingApi.new

begin
  # Stripe Webhook
  result = api_instance.stripe_webhook_billing_billing_webhook_post
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->stripe_webhook_billing_billing_webhook_post: #{e}"
end
```

#### Using the stripe_webhook_billing_billing_webhook_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebhookResponse>, Integer, Hash)> stripe_webhook_billing_billing_webhook_post_with_http_info

```ruby
begin
  # Stripe Webhook
  data, status_code, headers = api_instance.stripe_webhook_billing_billing_webhook_post_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebhookResponse>
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->stripe_webhook_billing_billing_webhook_post_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**WebhookResponse**](WebhookResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## stripe_webhook_billing_billing_webhook_post_0

> <WebhookResponse> stripe_webhook_billing_billing_webhook_post_0

Stripe Webhook

Webhook de Stripe.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::BillingApi.new

begin
  # Stripe Webhook
  result = api_instance.stripe_webhook_billing_billing_webhook_post_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->stripe_webhook_billing_billing_webhook_post_0: #{e}"
end
```

#### Using the stripe_webhook_billing_billing_webhook_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<WebhookResponse>, Integer, Hash)> stripe_webhook_billing_billing_webhook_post_0_with_http_info

```ruby
begin
  # Stripe Webhook
  data, status_code, headers = api_instance.stripe_webhook_billing_billing_webhook_post_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <WebhookResponse>
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->stripe_webhook_billing_billing_webhook_post_0_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**WebhookResponse**](WebhookResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## test_notification_billing_billing_test_notification_post

> <Hash<String, ResponseTestNotificationBillingBillingTestNotificationPostValue>> test_notification_billing_billing_test_notification_post(request_body)

Test Notification

Envía un email de prueba de cambio de plan.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::BillingApi.new
request_body = { key: 'inner_example'} # Hash<String, String> | 

begin
  # Test Notification
  result = api_instance.test_notification_billing_billing_test_notification_post(request_body)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->test_notification_billing_billing_test_notification_post: #{e}"
end
```

#### Using the test_notification_billing_billing_test_notification_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Hash<String, ResponseTestNotificationBillingBillingTestNotificationPostValue>>, Integer, Hash)> test_notification_billing_billing_test_notification_post_with_http_info(request_body)

```ruby
begin
  # Test Notification
  data, status_code, headers = api_instance.test_notification_billing_billing_test_notification_post_with_http_info(request_body)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Hash<String, ResponseTestNotificationBillingBillingTestNotificationPostValue>>
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->test_notification_billing_billing_test_notification_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **request_body** | [**Hash&lt;String, String&gt;**](String.md) |  |  |

### Return type

[**Hash&lt;String, ResponseTestNotificationBillingBillingTestNotificationPostValue&gt;**](ResponseTestNotificationBillingBillingTestNotificationPostValue.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## test_notification_billing_billing_test_notification_post_0

> <Hash<String, ResponseTestNotificationBillingBillingTestNotificationPostValue>> test_notification_billing_billing_test_notification_post_0(request_body)

Test Notification

Envía un email de prueba de cambio de plan.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::BillingApi.new
request_body = { key: 'inner_example'} # Hash<String, String> | 

begin
  # Test Notification
  result = api_instance.test_notification_billing_billing_test_notification_post_0(request_body)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->test_notification_billing_billing_test_notification_post_0: #{e}"
end
```

#### Using the test_notification_billing_billing_test_notification_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Hash<String, ResponseTestNotificationBillingBillingTestNotificationPostValue>>, Integer, Hash)> test_notification_billing_billing_test_notification_post_0_with_http_info(request_body)

```ruby
begin
  # Test Notification
  data, status_code, headers = api_instance.test_notification_billing_billing_test_notification_post_0_with_http_info(request_body)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Hash<String, ResponseTestNotificationBillingBillingTestNotificationPostValue>>
rescue MailSafePro::ApiError => e
  puts "Error when calling BillingApi->test_notification_billing_billing_test_notification_post_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **request_body** | [**Hash&lt;String, String&gt;**](String.md) |  |  |

### Return type

[**Hash&lt;String, ResponseTestNotificationBillingBillingTestNotificationPostValue&gt;**](ResponseTestNotificationBillingBillingTestNotificationPostValue.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

