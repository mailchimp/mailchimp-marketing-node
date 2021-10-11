# Changelog

## Transactional

### 1.0.46
* Added a little more granularity to the `set_timeout` method to the Client class in the Ruby SDK; now supports `read`, `write` and `connect` parameters, which will default to the `timeout` param if unspecified, or 300 seconds if `timeout` is unspecified.

### 1.0.45
* Added a `set_timeout` method to the Client class in the Ruby SDK

### 1.0.44
* Added a `set_timeout` method to the Client class in the Python SDK

### 1.0.43
* Added a `setTimeout` method to the Configuration class in the PHP SDK.

### 1.0.42
* Added a `setDefaultTimeoutMs` method to the node client. This allows users to override the default timeout for API requests, which is set to 5 minutes by default.

### 1.0.41
* Updated the "reject_reasons" response for /messages/send and /messages/send-template to correctly use "hard-bounce" and "soft-bounce" instead of the previously stated "hard_bounce" and "soft_bounce".

### 1.0.40
* Added the new /allowlists/ series of endpoints and the /exports/allowlist endpoint to the API reference

### 1.0.39
* Fixes the output directory for the Changelog for the php client library

### 1.0.38
* A change was made to `mailchimp-transactional-php` - the API client will now always return an `Exception`, instead of an `Exception` or a string, when the API returns an error. Having to parse the response as a string was found to be a bit clunky.

### 1.0.37
* Added a changelog, which will be used to describe changes to both transactional and marketing client libraries.

## Marketing

### 3.0.70
* Added more granularity for the `timeout` field in the Ruby Marketing SDK; now supports `read_timeout`, `write_timeout` and `connect_timeout` fields which will default to the `timeout` value.

### 3.0.69
* Added handling for a `timeout` field in the config block passed to the client constructor in the Ruby Marketing SDK.

### 3.0.68
* Added handling for a `'timeout'` field in `set_config()` in the Python Marketing SDK.

### 3.0.67
* Added a `setTimeout()` method to the configuration class in the PHP Marketing SDK, to allow manually setting the timeout for Guzzle requests.

### 3.0.65
* Added a new API endpoint, `/3.0/account-exports`, allowing users to programatically export their account information

### 3.0.64
* Fixes the output directory for the Changelog for the php client library

### 3.0.63
* Added a changelog, which will be used to describe changes to both transactional and marketing client libraries.
