---
api_key_in:
- header
api_specs:
- filename: punchh-mobile-api-openapi.yml
  format: yaml
  label: Punchh Mobile API
  slug: punchh-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-mobile-api-openapi.yml
- filename: punchh-mobile-redemptions-legacy-openapi.yml
  format: yaml
  label: Punchh Redemptions 1.0 (Legacy) API - Mobile
  slug: punchh-mobile-redemptions-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-mobile-redemptions-legacy-openapi.yml
- filename: punchh-mobile-redemptions-v2-openapi.yml
  format: yaml
  label: Punchh Redemptions 2.0 (New) API - Mobile
  slug: punchh-mobile-redemptions-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-mobile-redemptions-v2-openapi.yml
- filename: punchh-mobile-subscription-openapi.yml
  format: yaml
  label: Punchh Subscription API - Mobile
  slug: punchh-mobile-subscription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-mobile-subscription-openapi.yml
- filename: punchh-online-ordering-redemptions-legacy-openapi.yml
  format: yaml
  label: Punchh Redemptions 1.0 (Legacy) API - Online Ordering
  slug: punchh-online-ordering-redemptions-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-online-ordering-redemptions-legacy-openapi.yml
- filename: punchh-online-ordering-redemptions-v2-openapi.yml
  format: yaml
  label: Punchh Redemptions 2.0 (New) API - Online Ordering
  slug: punchh-online-ordering-redemptions-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-online-ordering-redemptions-v2-openapi.yml
- filename: punchh-online-ordering-sso-api-openapi.yml
  format: yaml
  label: Punchh Online Ordering and SSO API
  slug: punchh-online-ordering-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-online-ordering-sso-api-openapi.yml
- filename: punchh-online-ordering-subscription-openapi.yml
  format: yaml
  label: Punchh Subscription API - Online Ordering
  slug: punchh-online-ordering-subscription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-online-ordering-subscription-openapi.yml
- filename: punchh-platform-functions-api-openapi.yml
  format: yaml
  label: Punchh Platform Functions API
  slug: punchh-platform-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-platform-functions-api-openapi.yml
- filename: punchh-platform-functions-headless-offers-openapi.yml
  format: yaml
  label: Punchh Headless Offers API - Platform Functions
  slug: punchh-platform-functions-headless-offers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-platform-functions-headless-offers-openapi.yml
- filename: punchh-platform-functions-offers-ingestion-openapi.yml
  format: yaml
  label: Punchh Offers Ingestion API - Platform Functions
  slug: punchh-platform-functions-offers-ingestion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-platform-functions-offers-ingestion-openapi.yml
- filename: punchh-platform-functions-subscription-openapi.yml
  format: yaml
  label: Punchh Subscription API - Platform Functions
  slug: punchh-platform-functions-subscription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-platform-functions-subscription-openapi.yml
- filename: punchh-pos-api-openapi.yml
  format: yaml
  label: Punchh POS API
  slug: punchh-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-pos-api-openapi.yml
- filename: punchh-pos-redemptions-legacy-openapi.yml
  format: yaml
  label: Punchh Redemptions 1.0 (Legacy) API - POS
  slug: punchh-pos-redemptions-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-pos-redemptions-legacy-openapi.yml
- filename: punchh-pos-redemptions-v2-openapi.yml
  format: yaml
  label: Punchh Redemptions 2.0 (New) API - POS
  slug: punchh-pos-redemptions-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-pos-redemptions-v2-openapi.yml
auth_types:
- http
- apiKey
- oauth2-flavoured
description: PAR Punchh authentication is a layered, hand-rolled scheme rather than a standards-discoverable one. A bearer access token establishes WHO is calling; an HMAC-SHA256 request digest establishes that the request was not tampered with; a device identifier establishes WHICH handset; and for proxied partners a true-client-IP header establishes which guest the call is really on behalf of. None of the 15 published OpenAPI documents declares a securityScheme — the auth contract lives entirely in the developer-portal prose and in explicit header parameters on individual operations.
kind: authentication
layout: security
method: searched
name: Punchh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Punchh secures its APIs with http, apiKey, and oauth2-flavoured across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Punchh
provider_slug: punchh
scheme_count: 7
schemes:
- applies_to:
  - mobile
  - online-ordering
  - platform-functions
  description: Access token issued by Sign In, SSO login, or the Advanced Authentication OTP exchange. Used on Mobile, Online Ordering/SSO and Platform Functions surfaces.
  name: PunchhBearer
  parameter: Authorization
  scheme: bearer
  type: http
  value: Bearer <access_token>
- applies_to:
  - mobile
  - online-ordering
  description: HMAC-SHA256 digest of the request URI and body. Punchh describes it as "security verification and protection against tampering during API calls between the mobile application and the Punchh server". Required alongside the bearer token; a wrong digest fails permanently, so never retry on it.
  in: header
  name: PunchhDigest
  parameter: x-pch-digest
  tooling: PAR publishes an interactive "Punchh x-pch-digest Generator" plus per-surface pages ("Generating x-pch-digest Header for Mobile APIs", "... for Online Ordering APIs").
  type: apiKey
- applies_to:
  - mobile
  description: 'Stable per-device GUID. An anti-fraud control: sign-up rewards are granted per device so a guest cannot re-register repeatedly on one handset. Must persist across a device reset (iOS keychain / Android permanent storage). Punchh publishes Java and Objective-C sample generators.'
  in: header
  name: PunchhDeviceId
  parameter: punchh-app-device-id
  required: true
  type: apiKey
- applies_to:
  - pos
  - kiosk
  description: POS and kiosk terminals authenticate with a location token / business token pair rather than a guest bearer token. POS is also the only Punchh surface still admitted at TLS 1.0+.
  in: header
  name: PunchhPosToken
  type: apiKey
- description: The business OAuth client id. Sent in the request body on unauthenticated mobile calls, and as an argument to the Advanced Authentication Send OTP, Verify Token and Refresh Token calls. Token endpoint is POST /oauth/token (operationId oauth_token).
  in: body
  name: PunchhOAuthClient
  parameter: client
  type: oauth2-flavoured
- description: Mandatory for indirect-access partners who proxy guest traffic. Punchh performs rate limiting and bot mitigation against this value instead of the connecting IP; requests without it "will be filtered and ignored". On the Platform Functions surface PAR's guidelines say this header must carry the customer brand name rather than an IP.
  in: header
  name: PunchhTrueClientIp
  parameter: x_true_client_ip
  required: conditional
  type: apiKey
- description: Recommended JA3 TLS fingerprint of the originating client, used for abuse filtering.
  in: header
  name: PunchhJa3
  parameter: x_ja3_fingerprint
  required: false
  type: apiKey
slug: punchh-authentication
source_filename: punchh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.partech.com/docs/dev-portal-mobile/headers-and-caching\ndocs:\n  - https://developers.partech.com/docs/dev-portal-mobile/headers-and-caching\n  - https://developers.partech.com/docs/dev-portal-mobile/user-authentication\n  - https://developers.partech.com/docs/dev-portal-developer-resources/advanced-authentication-developer-guide\n  - https://developers.partech.com/docs/dev-portal-developer-resources/punchh-api-security-guidelines\n  - https://developers.partech.com/docs/dev-portal-webhooks-manager/configuration\nprovider: PAR Punchh\nproviderId: punchh\ndescription: >-\n  PAR Punchh authentication is a layered, hand-rolled scheme rather than a\n  standards-discoverable one. A bearer access token establishes WHO is calling; an\n  HMAC-SHA256 request digest establishes that the request was not tampered with; a\n  device identifier establishes WHICH handset; and for proxied partners a\n  true-client-IP header\
  \ establishes which guest the call is really on behalf of.\n  None of the 15 published OpenAPI documents declares a securityScheme — the auth\n  contract lives entirely in the developer-portal prose and in explicit header\n  parameters on individual operations.\n\nsummary:\n  types: [http, apiKey, oauth2-flavoured]\n  api_key_in: [header]\n  declared_security_schemes_in_openapi: 0\n  well_known_metadata: none\n  scopes_published: false\n  note: >-\n    Auth headers appear as ordinary header PARAMETERS on operations (Authorization\n    on 23 operations, x-pch-digest on 1, User-Agent on 1) rather than as\n    components.securitySchemes. A generator reading these specs will produce a\n    client with no auth wired.\n\nschemes:\n  - name: PunchhBearer\n    type: http\n    scheme: bearer\n    parameter: Authorization\n    value: 'Bearer <access_token>'\n    description: >-\n      Access token issued by Sign In, SSO login, or the Advanced Authentication OTP\n      exchange. Used on Mobile, Online\
  \ Ordering/SSO and Platform Functions surfaces.\n    applies_to: [mobile, online-ordering, platform-functions]\n\n  - name: PunchhDigest\n    type: apiKey\n    in: header\n    parameter: x-pch-digest\n    description: >-\n      HMAC-SHA256 digest of the request URI and body. Punchh describes it as\n      \"security verification and protection against tampering during API calls\n      between the mobile application and the Punchh server\". Required alongside the\n      bearer token; a wrong digest fails permanently, so never retry on it.\n    applies_to: [mobile, online-ordering]\n    tooling: >-\n      PAR publishes an interactive \"Punchh x-pch-digest Generator\" plus per-surface\n      pages (\"Generating x-pch-digest Header for Mobile APIs\", \"... for Online\n      Ordering APIs\").\n\n  - name: PunchhDeviceId\n    type: apiKey\n    in: header\n    parameter: punchh-app-device-id\n    description: >-\n      Stable per-device GUID. An anti-fraud control: sign-up rewards are granted\
  \ per\n      device so a guest cannot re-register repeatedly on one handset. Must persist\n      across a device reset (iOS keychain / Android permanent storage). Punchh\n      publishes Java and Objective-C sample generators.\n    applies_to: [mobile]\n    required: true\n\n  - name: PunchhPosToken\n    type: apiKey\n    in: header\n    description: >-\n      POS and kiosk terminals authenticate with a location token / business token\n      pair rather than a guest bearer token. POS is also the only Punchh surface\n      still admitted at TLS 1.0+.\n    applies_to: [pos, kiosk]\n\n  - name: PunchhOAuthClient\n    type: oauth2-flavoured\n    parameter: client\n    in: body\n    description: >-\n      The business OAuth client id. Sent in the request body on unauthenticated\n      mobile calls, and as an argument to the Advanced Authentication Send OTP,\n      Verify Token and Refresh Token calls. Token endpoint is POST /oauth/token\n      (operationId oauth_token).\n\n  - name: PunchhTrueClientIp\n\
  \    type: apiKey\n    in: header\n    parameter: x_true_client_ip\n    description: >-\n      Mandatory for indirect-access partners who proxy guest traffic. Punchh\n      performs rate limiting and bot mitigation against this value instead of the\n      connecting IP; requests without it \"will be filtered and ignored\". On the\n      Platform Functions surface PAR's guidelines say this header must carry the\n      customer brand name rather than an IP.\n    required: conditional\n  - name: PunchhJa3\n    type: apiKey\n    in: header\n    parameter: x_ja3_fingerprint\n    required: false\n    description: Recommended JA3 TLS fingerprint of the originating client, used for abuse filtering.\n\nadvanced_authentication:\n  feature: PAR Punchh Advanced Authentication\n  enabled_by: PAR representative, per business\n  capabilities:\n    - Third-party identity providers\n    - Passwordless one-time password over email\n    - Passwordless one-time password over SMS\n    - SAML Single Sign-on\
  \ (online ordering)\n    - Sign in with Apple, Google sign-in (published mobile operations)\n  flow:\n    - step: Send OTP\n      inputs: [OAuth client id, validation method, email or phone + extension, terms_and_conditions=true, privacy_policy=true, PKCE code challenge]\n      operationId: mobile_generate_otp_token\n    - step: Verify Token\n      inputs: [OTP, identifier, OAuth client id, consent flags, PKCE code verifier]\n      returns: [access_token, refresh_token]\n      operationId: mobile_verify_token\n    - step: Refresh Token\n      inputs: [OAuth client id, refresh_token]\n      returns: [access_token, refresh_token]\n      note: Both tokens are replaced; Punchh rotates the refresh token.\n  note: >-\n    Sign-in and sign-up are the same call — if the user does not exist, one is\n    created. Consent flags are therefore load-bearing, not boilerplate.\n  id_token_shape: '{\"id\": \"<Issuer_Identifier>\", \"sub\": \"<Subject_Identifier>\", \"access_token\": \"<User_Access_Token>\"\
  }'\n  source: https://developers.partech.com/docs/dev-portal-developer-resources/advanced-authentication-developer-guide\n\nwebhook_consumer_authentication:\n  note: >-\n    Inbound-to-you auth for the Events Framework is separately specified — Basic,\n    Bearer, HMAC-SHA1 or HMAC-SHA256, with the client identifier in an x-pch-key\n    header. See asyncapi/punchh-webhooks.yml.\n\ngaps:\n  - No /.well-known/openid-configuration (404 on punchh.com, developers.partech.com, partech.com, api.punchh.com).\n  - No /.well-known/oauth-authorization-server (404 on all four hosts).\n  - No published OAuth scopes and no scopes/permissions reference page; derive-oauth-scopes found 0 oauth2 schemes across all 15 specs.\n  - No published token lifetimes for access_token or refresh_token.\n  - No securitySchemes block in any published OpenAPI document, so the auth contract is not machine-readable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/authentication/punchh-authentication.yml
summary_line: http/apiKey/oauth2-flavoured · 7 schemes
tags:
- Gift Cards
- Guest Engagement
- Loyalty
- Marketing
- Mobile
- Offers
- Online Ordering
- PAR Technology
- Point-of-Sale
- Restaurant
- Restaurant Technology
- Webhook
---
