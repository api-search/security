---
api_key_in: []
auth_types:
- licenseKey
- jwt
- http-basic
description: ''
kind: authentication
layout: security
method: searched
name: Ai Coustics Authentication
name_suffix: Authentication
oauth_flows: []
overview: ai-coustics secures its APIs with licenseKey, jwt, and http-basic across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ai-coustics
provider_slug: ai-coustics
scheme_count: 3
schemes:
- description: Self-service SDK license key generated in the developer platform (developers.ai-coustics.com). Credential format is `<payload>.<signature>` where the payload is base64-encoded JSON with fields user, version and api_key. Embed directly in trusted server environments.
  in: sdk-config
  name: sdkLicenseKey
  source: https://developers.ai-coustics.com/
  type: apiKey
- bearerFormat: JWT
  description: Short-lived JWT dropped in exactly where a license key would be used, for untrusted client-side apps. Carries an `exp` claim (Unix seconds), ~1 hour TTL. Refresh proactively via the processor's update_bearer_token() without recreating the processor or reloading the model.
  name: jwtBearer
  scheme: bearer
  type: http
- description: HTTP Basic auth used to call the token-minting endpoint. The SDK api_key is the username; the password is empty.
  name: tokenMintBasicAuth
  response_fields:
  - token
  - expires_at
  scheme: basic
  token_endpoint: https://api.ai-coustics.io/v1/sdk/tokens
  type: http
slug: ai-coustics-authentication
source_filename: ai-coustics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.ai-coustics.com/models/get-started/authenticate-apps\ndocs: https://docs.ai-coustics.com/models/get-started/authenticate-apps\nsummary:\n  types: [licenseKey, jwt, http-basic]\n  description: >-\n    The ai-coustics SDK authenticates with a license (SDK) key on trusted\n    servers, or with short-lived JWTs minted from your backend for untrusted\n    clients. JWTs are issued by a token-minting endpoint protected with HTTP\n    Basic auth using the SDK api_key as the username and an empty password.\nschemes:\n  - name: sdkLicenseKey\n    type: apiKey\n    in: sdk-config\n    description: >-\n      Self-service SDK license key generated in the developer platform\n      (developers.ai-coustics.com). Credential format is `<payload>.<signature>`\n      where the payload is base64-encoded JSON with fields user, version and\n      api_key. Embed directly in trusted server environments.\n    source: https://developers.ai-coustics.com/\n\
  \  - name: jwtBearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Short-lived JWT dropped in exactly where a license key would be used, for\n      untrusted client-side apps. Carries an `exp` claim (Unix seconds), ~1 hour\n      TTL. Refresh proactively via the processor's update_bearer_token() without\n      recreating the processor or reloading the model.\n  - name: tokenMintBasicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic auth used to call the token-minting endpoint. The SDK api_key is\n      the username; the password is empty.\n    token_endpoint: https://api.ai-coustics.io/v1/sdk/tokens\n    response_fields: [token, expires_at]\nnotes:\n  - The legacy REST API (api-key based, single call voice enhancement) was sunset in 2026; migrate to the SDK.\n  - Offline entitlements in JWT licenses were added in SDK 0.21.1 (2026-06-26).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-coustics/refs/heads/main/authentication/ai-coustics-authentication.yml
summary_line: licenseKey/jwt/http-basic · 3 schemes
tags:
- Company
- Ai/Ml
- Audio
- Speech Enhancement
- Voice AI
- Speech Recognition
- SDK
- Real-Time
- Machine Learning
---
