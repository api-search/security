---
api_key_in:
- header
api_specs:
- filename: typingdna-authentication-api-openapi-original.json
  format: json
  label: TypingDNA Authentication API
  slug: typingdna-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typingdna/refs/heads/main/openapi/typingdna-authentication-api-openapi-original.json
- filename: typingdna-verify-2fa-openapi.json
  format: json
  label: TypingDNA Verify 2FA API
  slug: typingdna-verify-2fa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typingdna/refs/heads/main/openapi/typingdna-verify-2fa-openapi.json
auth_types:
- apiKey
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Typingdna Authentication
name_suffix: Authentication
oauth_flows: []
overview: TypingDNA secures its APIs with apiKey, http, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TypingDNA
provider_slug: typingdna
scheme_count: 4
schemes:
- description: 'HTTP Basic over HTTPS (TLS 1.2+): apiKey as username, apiSecret as password. Keys are issued per account in the client dashboard (https://www.typingdna.com/clients/signup, free Starter tier available). Applies to every Authentication API operation on api.typingdna.com / eu-api.typingdna.com / us-api.typingdna.com.'
  name: basic_auth
  scheme: basic
  sources:
  - openapi/typingdna-authentication-api-openapi-original.json
  type: http
- description: Authorization token required for the /user/reset-profile endpoint. Obtain this from the TypingDNA Verify Dashboard under your application's Reset Profile endpoint section.
  in: header
  name: ResetProfileBasicAuth
  parameter: Authorization
  sources:
  - openapi/typingdna-verify-2fa-openapi.json
  type: apiKey
- description: Verify 2FA service calls (/otp/validate, /otp/send) authenticate with clientId + applicationId + an encrypted payload generated server-side by the official Verify client's getDataAttributes() using the application secret; credentials differ between Sandbox and Production environments.
  name: verify_2fa_payload
  sources:
  - https://verify.typingdna.com/docs
  type: custom
- description: 'Verify 2FA OIDC integration: verify.typingdna.com is a standard OIDC issuer (authorization_code + refresh_token + device_code + jwt-bearer, PKCE S256, RS256 id tokens; client_secret_post/client_secret_basic or public/private key auth). Used to plug typing verification into Okta, Ping Identity and Microsoft Entra ID.'
  name: verify_oidc
  openIdConnectUrl: https://verify.typingdna.com/.well-known/openid-configuration
  sources:
  - well-known/typingdna-verify-openid-configuration.json
  type: openIdConnect
slug: typingdna-authentication
source_filename: typingdna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/typingdna-authentication-api-openapi-original.json, openapi/typingdna-verify-2fa-openapi.json\ndocs: https://api.typingdna.com/docs/index.html\nsummary:\n  types:\n  - apiKey\n  - http\n  - openIdConnect\n  api_key_in:\n  - header\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic over HTTPS (TLS 1.2+): apiKey as username, apiSecret as\n    password. Keys are issued per account in the client dashboard\n    (https://www.typingdna.com/clients/signup, free Starter tier available).\n    Applies to every Authentication API operation on api.typingdna.com /\n    eu-api.typingdna.com / us-api.typingdna.com.\n  sources:\n  - openapi/typingdna-authentication-api-openapi-original.json\n- name: ResetProfileBasicAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Authorization token required for the /user/reset-profile endpoint. Obtain this\n    from the TypingDNA\
  \ Verify Dashboard under your application's Reset Profile endpoint section.\n  sources:\n  - openapi/typingdna-verify-2fa-openapi.json\n- name: verify_2fa_payload\n  type: custom\n  description: >-\n    Verify 2FA service calls (/otp/validate, /otp/send) authenticate with\n    clientId + applicationId + an encrypted payload generated server-side by\n    the official Verify client's getDataAttributes() using the application\n    secret; credentials differ between Sandbox and Production environments.\n  sources:\n  - https://verify.typingdna.com/docs\n- name: verify_oidc\n  type: openIdConnect\n  openIdConnectUrl: https://verify.typingdna.com/.well-known/openid-configuration\n  description: >-\n    Verify 2FA OIDC integration: verify.typingdna.com is a standard OIDC\n    issuer (authorization_code + refresh_token + device_code + jwt-bearer,\n    PKCE S256, RS256 id tokens; client_secret_post/client_secret_basic or\n    public/private key auth). Used to plug typing verification into Okta,\n\
  \    Ping Identity and Microsoft Entra ID.\n  sources:\n  - well-known/typingdna-verify-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typingdna/refs/heads/main/authentication/typingdna-authentication.yml
summary_line: apiKey/http/openIdConnect · 4 schemes
tags:
- Company
- Authentication
- Biometrics
- Typing Biometrics
- Two-Factor Authentication
- Identity
- Security
- Fraud Prevention
---
