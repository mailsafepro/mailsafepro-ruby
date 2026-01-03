# MailSafePro::AuthenticationApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**auth_health_check_auth_health_auth_get**](AuthenticationApi.md#auth_health_check_auth_health_auth_get) | **GET** /auth/health/auth | Auth Health Check |
| [**auth_health_check_auth_health_auth_get_0**](AuthenticationApi.md#auth_health_check_auth_health_auth_get_0) | **GET** /auth/health/auth | Auth Health Check |
| [**auth_health_check_auth_health_auth_head**](AuthenticationApi.md#auth_health_check_auth_health_auth_head) | **HEAD** /auth/health/auth | Auth Health Check |
| [**auth_health_check_auth_health_auth_head_0**](AuthenticationApi.md#auth_health_check_auth_health_auth_head_0) | **HEAD** /auth/health/auth | Auth Health Check |
| [**delete_account_auth_delete_delete**](AuthenticationApi.md#delete_account_auth_delete_delete) | **DELETE** /auth/delete | Delete Account |
| [**delete_account_auth_delete_delete_0**](AuthenticationApi.md#delete_account_auth_delete_delete_0) | **DELETE** /auth/delete | Delete Account |
| [**get_current_user_auth_me_get**](AuthenticationApi.md#get_current_user_auth_me_get) | **GET** /auth/me | Get Current User |
| [**get_current_user_auth_me_get_0**](AuthenticationApi.md#get_current_user_auth_me_get_0) | **GET** /auth/me | Get Current User |
| [**login_web_user_auth_login_post**](AuthenticationApi.md#login_web_user_auth_login_post) | **POST** /auth/login | Login Web User |
| [**login_web_user_auth_login_post_0**](AuthenticationApi.md#login_web_user_auth_login_post_0) | **POST** /auth/login | Login Web User |
| [**logout_auth_logout_post**](AuthenticationApi.md#logout_auth_logout_post) | **POST** /auth/logout | Logout |
| [**logout_auth_logout_post_0**](AuthenticationApi.md#logout_auth_logout_post_0) | **POST** /auth/logout | Logout |
| [**refresh_token_auth_refresh_post**](AuthenticationApi.md#refresh_token_auth_refresh_post) | **POST** /auth/refresh | Refresh Token |
| [**refresh_token_auth_refresh_post_0**](AuthenticationApi.md#refresh_token_auth_refresh_post_0) | **POST** /auth/refresh | Refresh Token |
| [**register_web_user_auth_register_post**](AuthenticationApi.md#register_web_user_auth_register_post) | **POST** /auth/register | Register Web User |
| [**register_web_user_auth_register_post_0**](AuthenticationApi.md#register_web_user_auth_register_post_0) | **POST** /auth/register | Register Web User |
| [**rotate_api_key_auth_rotate_key_post**](AuthenticationApi.md#rotate_api_key_auth_rotate_key_post) | **POST** /auth/rotate-key | Rotate Api Key |
| [**rotate_api_key_auth_rotate_key_post_0**](AuthenticationApi.md#rotate_api_key_auth_rotate_key_post_0) | **POST** /auth/rotate-key | Rotate Api Key |


## auth_health_check_auth_health_auth_get

> Object auth_health_check_auth_health_auth_get

Auth Health Check

Health check para autenticación: Redis, JWT y hashing.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::AuthenticationApi.new

begin
  # Auth Health Check
  result = api_instance.auth_health_check_auth_health_auth_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->auth_health_check_auth_health_auth_get: #{e}"
end
```

#### Using the auth_health_check_auth_health_auth_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> auth_health_check_auth_health_auth_get_with_http_info

```ruby
begin
  # Auth Health Check
  data, status_code, headers = api_instance.auth_health_check_auth_health_auth_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->auth_health_check_auth_health_auth_get_with_http_info: #{e}"
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


## auth_health_check_auth_health_auth_get_0

> Object auth_health_check_auth_health_auth_get_0

Auth Health Check

Health check para autenticación: Redis, JWT y hashing.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::AuthenticationApi.new

begin
  # Auth Health Check
  result = api_instance.auth_health_check_auth_health_auth_get_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->auth_health_check_auth_health_auth_get_0: #{e}"
end
```

#### Using the auth_health_check_auth_health_auth_get_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> auth_health_check_auth_health_auth_get_0_with_http_info

```ruby
begin
  # Auth Health Check
  data, status_code, headers = api_instance.auth_health_check_auth_health_auth_get_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->auth_health_check_auth_health_auth_get_0_with_http_info: #{e}"
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


## auth_health_check_auth_health_auth_head

> Object auth_health_check_auth_health_auth_head

Auth Health Check

Health check para autenticación: Redis, JWT y hashing.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::AuthenticationApi.new

begin
  # Auth Health Check
  result = api_instance.auth_health_check_auth_health_auth_head
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->auth_health_check_auth_health_auth_head: #{e}"
end
```

#### Using the auth_health_check_auth_health_auth_head_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> auth_health_check_auth_health_auth_head_with_http_info

```ruby
begin
  # Auth Health Check
  data, status_code, headers = api_instance.auth_health_check_auth_health_auth_head_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->auth_health_check_auth_health_auth_head_with_http_info: #{e}"
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


## auth_health_check_auth_health_auth_head_0

> Object auth_health_check_auth_health_auth_head_0

Auth Health Check

Health check para autenticación: Redis, JWT y hashing.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::AuthenticationApi.new

begin
  # Auth Health Check
  result = api_instance.auth_health_check_auth_health_auth_head_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->auth_health_check_auth_health_auth_head_0: #{e}"
end
```

#### Using the auth_health_check_auth_health_auth_head_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> auth_health_check_auth_health_auth_head_0_with_http_info

```ruby
begin
  # Auth Health Check
  data, status_code, headers = api_instance.auth_health_check_auth_health_auth_head_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->auth_health_check_auth_health_auth_head_0_with_http_info: #{e}"
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


## delete_account_auth_delete_delete

> Object delete_account_auth_delete_delete

Delete Account

Elimina la cuenta del usuario autenticado y todos sus datos relacionados.  ⚠️ ADVERTENCIA: Esta operación es IRREVERSIBLE.  Elimina: - Datos del usuario - Todas las API keys - Usage/quota - Suscripciones - Rate limits - Tokens relacionados  Security: - Solo el usuario puede eliminarse a sí mismo (o admin) - Requiere autenticación válida - Registra la acción en logs para auditoría - Rate limited para prevenir abuse

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::AuthenticationApi.new

begin
  # Delete Account
  result = api_instance.delete_account_auth_delete_delete
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->delete_account_auth_delete_delete: #{e}"
end
```

#### Using the delete_account_auth_delete_delete_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> delete_account_auth_delete_delete_with_http_info

```ruby
begin
  # Delete Account
  data, status_code, headers = api_instance.delete_account_auth_delete_delete_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->delete_account_auth_delete_delete_with_http_info: #{e}"
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


## delete_account_auth_delete_delete_0

> Object delete_account_auth_delete_delete_0

Delete Account

Elimina la cuenta del usuario autenticado y todos sus datos relacionados.  ⚠️ ADVERTENCIA: Esta operación es IRREVERSIBLE.  Elimina: - Datos del usuario - Todas las API keys - Usage/quota - Suscripciones - Rate limits - Tokens relacionados  Security: - Solo el usuario puede eliminarse a sí mismo (o admin) - Requiere autenticación válida - Registra la acción en logs para auditoría - Rate limited para prevenir abuse

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::AuthenticationApi.new

begin
  # Delete Account
  result = api_instance.delete_account_auth_delete_delete_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->delete_account_auth_delete_delete_0: #{e}"
end
```

#### Using the delete_account_auth_delete_delete_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> delete_account_auth_delete_delete_0_with_http_info

```ruby
begin
  # Delete Account
  data, status_code, headers = api_instance.delete_account_auth_delete_delete_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->delete_account_auth_delete_delete_0_with_http_info: #{e}"
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


## get_current_user_auth_me_get

> Object get_current_user_auth_me_get

Get Current User

Devuelve información básica del usuario actual.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::AuthenticationApi.new

begin
  # Get Current User
  result = api_instance.get_current_user_auth_me_get
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->get_current_user_auth_me_get: #{e}"
end
```

#### Using the get_current_user_auth_me_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> get_current_user_auth_me_get_with_http_info

```ruby
begin
  # Get Current User
  data, status_code, headers = api_instance.get_current_user_auth_me_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->get_current_user_auth_me_get_with_http_info: #{e}"
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


## get_current_user_auth_me_get_0

> Object get_current_user_auth_me_get_0

Get Current User

Devuelve información básica del usuario actual.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::AuthenticationApi.new

begin
  # Get Current User
  result = api_instance.get_current_user_auth_me_get_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->get_current_user_auth_me_get_0: #{e}"
end
```

#### Using the get_current_user_auth_me_get_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> get_current_user_auth_me_get_0_with_http_info

```ruby
begin
  # Get Current User
  data, status_code, headers = api_instance.get_current_user_auth_me_get_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->get_current_user_auth_me_get_0_with_http_info: #{e}"
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


## login_web_user_auth_login_post

> Object login_web_user_auth_login_post(user_login)

Login Web User

Login de usuario para panel web.  Security features: - Rate limiting por email + IP - Timing attack protection - Generic error messages - PII masking en logs

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::AuthenticationApi.new
user_login = MailSafePro::UserLogin.new({email: 'email_example', password: 'password_example'}) # UserLogin | 

begin
  # Login Web User
  result = api_instance.login_web_user_auth_login_post(user_login)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->login_web_user_auth_login_post: #{e}"
end
```

#### Using the login_web_user_auth_login_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> login_web_user_auth_login_post_with_http_info(user_login)

```ruby
begin
  # Login Web User
  data, status_code, headers = api_instance.login_web_user_auth_login_post_with_http_info(user_login)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->login_web_user_auth_login_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_login** | [**UserLogin**](UserLogin.md) |  |  |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## login_web_user_auth_login_post_0

> Object login_web_user_auth_login_post_0(user_login)

Login Web User

Login de usuario para panel web.  Security features: - Rate limiting por email + IP - Timing attack protection - Generic error messages - PII masking en logs

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::AuthenticationApi.new
user_login = MailSafePro::UserLogin.new({email: 'email_example', password: 'password_example'}) # UserLogin | 

begin
  # Login Web User
  result = api_instance.login_web_user_auth_login_post_0(user_login)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->login_web_user_auth_login_post_0: #{e}"
end
```

#### Using the login_web_user_auth_login_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> login_web_user_auth_login_post_0_with_http_info(user_login)

```ruby
begin
  # Login Web User
  data, status_code, headers = api_instance.login_web_user_auth_login_post_0_with_http_info(user_login)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->login_web_user_auth_login_post_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_login** | [**UserLogin**](UserLogin.md) |  |  |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## logout_auth_logout_post

> Object logout_auth_logout_post

Logout

Logout idempotente: - Si el access token es válido, lo añade a la blacklist. - Si el access token está expirado, responde 200 indicando que ya estaba expirado. - Solo devuelve 401 si el token es completamente inválido (firma/claims corruptos). - Intenta revocar el refresh token si se proporciona.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::AuthenticationApi.new

begin
  # Logout
  result = api_instance.logout_auth_logout_post
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->logout_auth_logout_post: #{e}"
end
```

#### Using the logout_auth_logout_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> logout_auth_logout_post_with_http_info

```ruby
begin
  # Logout
  data, status_code, headers = api_instance.logout_auth_logout_post_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->logout_auth_logout_post_with_http_info: #{e}"
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


## logout_auth_logout_post_0

> Object logout_auth_logout_post_0

Logout

Logout idempotente: - Si el access token es válido, lo añade a la blacklist. - Si el access token está expirado, responde 200 indicando que ya estaba expirado. - Solo devuelve 401 si el token es completamente inválido (firma/claims corruptos). - Intenta revocar el refresh token si se proporciona.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::AuthenticationApi.new

begin
  # Logout
  result = api_instance.logout_auth_logout_post_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->logout_auth_logout_post_0: #{e}"
end
```

#### Using the logout_auth_logout_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> logout_auth_logout_post_0_with_http_info

```ruby
begin
  # Logout
  data, status_code, headers = api_instance.logout_auth_logout_post_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->logout_auth_logout_post_0_with_http_info: #{e}"
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


## refresh_token_auth_refresh_post

> Object refresh_token_auth_refresh_post

Refresh Token

Crea un nuevo par de tokens a partir de un refresh token válido y no revocado.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::AuthenticationApi.new

begin
  # Refresh Token
  result = api_instance.refresh_token_auth_refresh_post
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->refresh_token_auth_refresh_post: #{e}"
end
```

#### Using the refresh_token_auth_refresh_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> refresh_token_auth_refresh_post_with_http_info

```ruby
begin
  # Refresh Token
  data, status_code, headers = api_instance.refresh_token_auth_refresh_post_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->refresh_token_auth_refresh_post_with_http_info: #{e}"
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


## refresh_token_auth_refresh_post_0

> Object refresh_token_auth_refresh_post_0

Refresh Token

Crea un nuevo par de tokens a partir de un refresh token válido y no revocado.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::AuthenticationApi.new

begin
  # Refresh Token
  result = api_instance.refresh_token_auth_refresh_post_0
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->refresh_token_auth_refresh_post_0: #{e}"
end
```

#### Using the refresh_token_auth_refresh_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> refresh_token_auth_refresh_post_0_with_http_info

```ruby
begin
  # Refresh Token
  data, status_code, headers = api_instance.refresh_token_auth_refresh_post_0_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->refresh_token_auth_refresh_post_0_with_http_info: #{e}"
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


## register_web_user_auth_register_post

> Object register_web_user_auth_register_post(user_register)

Register Web User

Registro de usuario para panel web: crea usuario, API key y tokens.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::AuthenticationApi.new
user_register = MailSafePro::UserRegister.new({email: 'email_example', password: 'password_example'}) # UserRegister | 

begin
  # Register Web User
  result = api_instance.register_web_user_auth_register_post(user_register)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->register_web_user_auth_register_post: #{e}"
end
```

#### Using the register_web_user_auth_register_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> register_web_user_auth_register_post_with_http_info(user_register)

```ruby
begin
  # Register Web User
  data, status_code, headers = api_instance.register_web_user_auth_register_post_with_http_info(user_register)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->register_web_user_auth_register_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_register** | [**UserRegister**](UserRegister.md) |  |  |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## register_web_user_auth_register_post_0

> Object register_web_user_auth_register_post_0(user_register)

Register Web User

Registro de usuario para panel web: crea usuario, API key y tokens.

### Examples

```ruby
require 'time'
require 'mailsafepro'

api_instance = MailSafePro::AuthenticationApi.new
user_register = MailSafePro::UserRegister.new({email: 'email_example', password: 'password_example'}) # UserRegister | 

begin
  # Register Web User
  result = api_instance.register_web_user_auth_register_post_0(user_register)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->register_web_user_auth_register_post_0: #{e}"
end
```

#### Using the register_web_user_auth_register_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> register_web_user_auth_register_post_0_with_http_info(user_register)

```ruby
begin
  # Register Web User
  data, status_code, headers = api_instance.register_web_user_auth_register_post_0_with_http_info(user_register)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->register_web_user_auth_register_post_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **user_register** | [**UserRegister**](UserRegister.md) |  |  |

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## rotate_api_key_auth_rotate_key_post

> Object rotate_api_key_auth_rotate_key_post(key_rotation_request)

Rotate Api Key

Rotación de API keys con período de gracia; acceso restringido a admin.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::AuthenticationApi.new
key_rotation_request = MailSafePro::KeyRotationRequest.new({old_key: 'old_key_example', new_key: 'new_key_example'}) # KeyRotationRequest | 

begin
  # Rotate Api Key
  result = api_instance.rotate_api_key_auth_rotate_key_post(key_rotation_request)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->rotate_api_key_auth_rotate_key_post: #{e}"
end
```

#### Using the rotate_api_key_auth_rotate_key_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> rotate_api_key_auth_rotate_key_post_with_http_info(key_rotation_request)

```ruby
begin
  # Rotate Api Key
  data, status_code, headers = api_instance.rotate_api_key_auth_rotate_key_post_with_http_info(key_rotation_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->rotate_api_key_auth_rotate_key_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **key_rotation_request** | [**KeyRotationRequest**](KeyRotationRequest.md) |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## rotate_api_key_auth_rotate_key_post_0

> Object rotate_api_key_auth_rotate_key_post_0(key_rotation_request)

Rotate Api Key

Rotación de API keys con período de gracia; acceso restringido a admin.

### Examples

```ruby
require 'time'
require 'mailsafepro'
# setup authorization
MailSafePro.configure do |config|
  # Configure Bearer authorization (JWT): Bearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = MailSafePro::AuthenticationApi.new
key_rotation_request = MailSafePro::KeyRotationRequest.new({old_key: 'old_key_example', new_key: 'new_key_example'}) # KeyRotationRequest | 

begin
  # Rotate Api Key
  result = api_instance.rotate_api_key_auth_rotate_key_post_0(key_rotation_request)
  p result
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->rotate_api_key_auth_rotate_key_post_0: #{e}"
end
```

#### Using the rotate_api_key_auth_rotate_key_post_0_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> rotate_api_key_auth_rotate_key_post_0_with_http_info(key_rotation_request)

```ruby
begin
  # Rotate Api Key
  data, status_code, headers = api_instance.rotate_api_key_auth_rotate_key_post_0_with_http_info(key_rotation_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue MailSafePro::ApiError => e
  puts "Error when calling AuthenticationApi->rotate_api_key_auth_rotate_key_post_0_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **key_rotation_request** | [**KeyRotationRequest**](KeyRotationRequest.md) |  |  |

### Return type

**Object**

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

