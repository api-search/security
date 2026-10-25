---
anonymous_access: false
api_key_in: []
api_specs:
- filename: afterpay-openapi-generated.yml
  format: yaml
  label: Afterpay API
  slug: afterpay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afterpay/refs/heads/main/openapi/_ae-authored/afterpay-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Afterpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Afterpay declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Afterpay
provider_slug: afterpay
scheme_count: 4
schemes:
- applies_to: Afterpay Online API
  description: Merchant ID as username and Secret Key as password, base64-encoded per RFC 7617. Afterpay provides merchant accounts per region, and each merchant account has unique API credentials. Required on every Online API endpoint except Ping.
  id: basicAuth
  scheme: basic
  type: http
- applies_to: Afterpay Online API
  description: Client Credentials (RFC 6749) bearer tokens; scope merchant_api_v2, or merchant_api_v1 for the first version of the merchant APIs.
  flow: clientCredentials
  id: clientCredentials
  sandboxTokenUrl: https://merchant-auth-sandbox.afterpay.com/v2/oauth2/token
  scopes:
  - merchant_api_v2
  - merchant_api_v1
  tokenUrl: https://merchant-auth.afterpay.com/v2/oauth2/token
  type: oauth2
- applies_to: Account linking
  description: 'Account Linking (OAuth): authorization code obtained through an Afterpay checkout, exchanged for access and refresh tokens.'
  docs: https://developers.afterpay.com/afterpay-online-developer/main/guides/api-development/additional-features/account-linking-oauth
  flow: authorizationCode
  id: accountLinking
  scopes:
  - read_user_info
  - create_checkout
  type: oauth2
- applies_to: Afterpay Partner API
  description: 'Partner API: HMAC-SHA256 signature in X-Afterpay-Request-Signature over URL, X-Afterpay-Request-Date epoch timestamp (no more than 60 seconds old) and body, keyed with the shared secret.'
  docs: https://developers.afterpay.com/afterpay-partner-api/guides/technical-guides/welcome/request-signing
  id: requestSigning
  in: header
  name: X-Afterpay-Request-Apikey
  type: apiKey
slug: afterpay-authentication
source_filename: afterpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Afterpay authentication\nprovider: afterpay\ngenerated: '2026-10-21'\nmethod: searched\nsource: https://developers.afterpay.com/afterpay-online-developer/main/api-reference/reference/introduction/authentication.md\ndocs: https://developers.afterpay.com/afterpay-online-developer/main/api-reference/reference/introduction/authentication\nschemes:\n- id: basicAuth\n  type: http\n  scheme: basic\n  description: Merchant ID as username and Secret Key as password, base64-encoded per RFC 7617. Afterpay provides merchant accounts per region, and each merchant account has unique API credentials. Required\n    on every Online API endpoint except Ping.\n  applies_to: Afterpay Online API\n- id: clientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://merchant-auth.afterpay.com/v2/oauth2/token\n  sandboxTokenUrl: https://merchant-auth-sandbox.afterpay.com/v2/oauth2/token\n  scopes:\n  - merchant_api_v2\n  - merchant_api_v1\n  description: Client Credentials\
  \ (RFC 6749) bearer tokens; scope merchant_api_v2, or merchant_api_v1 for the first version of the merchant APIs.\n  applies_to: Afterpay Online API\n- id: accountLinking\n  type: oauth2\n  flow: authorizationCode\n  scopes:\n  - read_user_info\n  - create_checkout\n  description: 'Account Linking (OAuth): authorization code obtained through an Afterpay checkout, exchanged for access and refresh tokens.'\n  docs: https://developers.afterpay.com/afterpay-online-developer/main/guides/api-development/additional-features/account-linking-oauth\n  applies_to: Account linking\n- id: requestSigning\n  type: apiKey\n  in: header\n  name: X-Afterpay-Request-Apikey\n  description: 'Partner API: HMAC-SHA256 signature in X-Afterpay-Request-Signature over URL, X-Afterpay-Request-Date epoch timestamp (no more than 60 seconds old) and body, keyed with the shared secret.'\n  docs: https://developers.afterpay.com/afterpay-partner-api/guides/technical-guides/welcome/request-signing\n  applies_to: Afterpay\
  \ Partner API\ntransport: All communication must use TLS 1.2 or higher.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afterpay/refs/heads/main/authentication/afterpay-authentication.yml
summary_line: 4 schemes
tags:
- Fintech
- Buy Now Pay Later
- Payments
- Consumer
- Block
- Australia
- Consumer Finance
---
