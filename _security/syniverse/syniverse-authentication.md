---
api_key_in:
- header
api_specs:
- filename: syniverse-omni-channel-messaging-openapi.yml
  format: yaml
  label: Syniverse Omni-Channel Messaging API (SCG)
  slug: syniverse-omni-channel-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-omni-channel-messaging-openapi.yml
- filename: syniverse-multi-factor-authentication-openapi.yml
  format: yaml
  label: Syniverse Multi-Factor Authentication API
  slug: syniverse-multi-factor-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-multi-factor-authentication-openapi.yml
- filename: syniverse-phone-number-verification-openapi.yml
  format: yaml
  label: Syniverse Phone Number Verification API
  slug: syniverse-phone-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-phone-number-verification-openapi.yml
- filename: syniverse-right-party-verification-openapi.yml
  format: yaml
  label: Syniverse Right Party Verification API
  slug: syniverse-right-party-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-right-party-verification-openapi.yml
- filename: syniverse-account-takeover-detection-openapi.yml
  format: yaml
  label: Syniverse Account Takeover Detection API
  slug: syniverse-account-takeover-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-account-takeover-detection-openapi.yml
- filename: syniverse-messaging-trust-resolve-openapi.yml
  format: yaml
  label: Syniverse Messaging Trust Resolve API
  slug: syniverse-messaging-trust-resolve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-messaging-trust-resolve-openapi.yml
- filename: syniverse-messaging-trust-datafeed-openapi.yml
  format: yaml
  label: Syniverse Messaging Trust Spam Datafeed API
  slug: syniverse-messaging-trust-spam-datafeed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-messaging-trust-datafeed-openapi.yml
- filename: syniverse-10dlc-openapi.yml
  format: yaml
  label: Syniverse 10DLC API
  slug: syniverse-10dlc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-10dlc-openapi.yml
- filename: syniverse-10dlc-number-pool-openapi.yml
  format: yaml
  label: Syniverse 10DLC Number Pool API (v1, deprecated)
  slug: syniverse-10dlc-number-pool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-10dlc-number-pool-openapi.yml
- filename: syniverse-whitelisting-service-openapi.json
  format: json
  label: Syniverse Whitelisting Service API
  slug: syniverse-whitelisting-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-whitelisting-service-openapi.json
- filename: syniverse-token-management-openapi.yml
  format: yaml
  label: Syniverse SDC Application Access Token Management API
  slug: syniverse-access-token-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-token-management-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Syniverse Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- implicit
overview: Syniverse secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and implicit flow(s).
provider_name: Syniverse
provider_slug: syniverse
scheme_count: 5
schemes:
- description: Use Bearer {Syniverse SDC Application Token} for example "Bearer aaaaa-aabb-bbaa-bbbbbb"
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/syniverse-10dlc-number-pool-openapi.yml
  type: apiKey
- bearerFormat: SDC
  name: SyniverseToken
  scheme: bearer
  sources:
  - openapi/syniverse-10dlc-openapi.yml
  type: http
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/syniverse-phone-number-verification-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.mt1.messaging-trust.syniverse.com/oauth2/token
  name: OAuth2
  note: The only true OAuth 2.0 client-credentials surface. No scopes are declared. The token host does not resolve in public DNS — it is a customer-provisioned surface.
  sources:
  - openapi/syniverse-messaging-trust-datafeed-openapi.yml
  - openapi/syniverse-messaging-trust-resolve-openapi.yml
  type: oauth2
- flows:
  - authorizationUrl: https://beta.api.syniverse.com/token
    flow: implicit
    scopes: 0
  name: default
  note: Legacy WSO2 gateway declaration pointing at a beta host. The implicit flow is deprecated by OAuth 2.0 Security Best Current Practice; treat this declaration as stale rather than as guidance.
  sources:
  - openapi/syniverse-whitelisting-service-openapi.json
  type: oauth2
slug: syniverse-authentication
source_filename: syniverse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  Derived from the securitySchemes/securityDefinitions across openapi/syniverse-10dlc-number-pool-openapi.yml,\n  openapi/syniverse-10dlc-openapi.yml, openapi/syniverse-messaging-trust-datafeed-openapi.yml,\n  openapi/syniverse-messaging-trust-resolve-openapi.yml, openapi/syniverse-phone-number-verification-openapi.yml\n  and openapi/syniverse-whitelisting-service-openapi.json, then upgraded from the published\n  Syniverse Developer Community security and quickstart documentation.\ndocs:\n- https://sdcdocumentation.syniverse.com/index.php/reporting/security\n- https://sdcdocumentation.syniverse.com/index.php/omni-channel/getting-started/sms-mms-quickstart\n- https://sdcdocumentation.syniverse.com/index.php/developer-community-gateway-services/api-reference/explore-token-management-api-reference\nsummary:\n  model: >-\n    A single SDC application access token, presented as an HTTP bearer token, is the\n    dominant credential\
  \ across the entire Syniverse Developer Community estate. Syniverse\n    describes the model as OAuth 2.0 (RFC 6749) with bearer tokens (RFC 6750), but there\n    is no authorization endpoint, no scope surface and no discovery document — in practice\n    it is a long-lived application credential, not an OAuth authorization flow. True\n    client-credentials OAuth appears on exactly one product family (Messaging Trust), and\n    a legacy implicit flow is declared on the Whitelisting Service.\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials, implicit]\n  primary_header: 'Authorization: Bearer {SDC application access token}'\n  scopes_published: false\n  openid_connect: false\n  mtls: false\n  ciba: false\ncredentials:\n  issued_per: registered SDC application\n  components: [consumer key, consumer secret, access token]\n  initial_access_token_ttl: 1 hour\n  after_first_regeneration: does not expire\n  regeneration: unlimited — regenerate as often\
  \ as needed\n  rotation:\n    access_token: >-\n      Regenerate via GET /saop-rest-data/v1/apptoken-refresh. A compromised access token\n      does not require a new application.\n    consumer_key_secret: >-\n      No rotation path. A compromised consumer key or secret requires creating an entirely\n      new application with fresh credentials.\n  expiry_signal: 'SCG_ERROR_4046 — \"Access token expired\" (HTTP 404)'\ntransport:\n  https_only: true\n  tls_version: TLS 1.2 (stated as the currently supported standard)\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Use Bearer {Syniverse SDC Application Token} for example \"Bearer aaaaa-aabb-bbaa-bbbbbb\"\n  sources:\n  - openapi/syniverse-10dlc-number-pool-openapi.yml\n- name: SyniverseToken\n  type: http\n  scheme: bearer\n  bearerFormat: SDC\n  sources:\n  - openapi/syniverse-10dlc-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/syniverse-phone-number-verification-openapi.yml\n\
  - name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.mt1.messaging-trust.syniverse.com/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/syniverse-messaging-trust-datafeed-openapi.yml\n  - openapi/syniverse-messaging-trust-resolve-openapi.yml\n  note: >-\n    The only true OAuth 2.0 client-credentials surface. No scopes are declared. The token\n    host does not resolve in public DNS — it is a customer-provisioned surface.\n- name: default\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://beta.api.syniverse.com/token\n    scopes: 0\n  sources:\n  - openapi/syniverse-whitelisting-service-openapi.json\n  note: >-\n    Legacy WSO2 gateway declaration pointing at a beta host. The implicit flow is\n    deprecated by OAuth 2.0 Security Best Current Practice; treat this declaration as\n    stale rather than as guidance.\nundeclared_surfaces:\n- api: Syniverse Omni-Channel Messaging (SCG)\n  spec: openapi/syniverse-omni-channel-messaging-openapi.yml\n\
  \  note: >-\n    The Swagger declares no securityDefinitions at all, but the gateway enforces auth —\n    an anonymous GET to /scg-external-api/api/v1/messaging/message_requests returns 401.\n    The quickstart documents the same Authorization: Bearer header used everywhere else.\n- api: Syniverse Multi-Factor Authentication\n  spec: openapi/syniverse-multi-factor-authentication-openapi.yml\n  note: No securityDefinitions declared; same SDC bearer-token model per the documentation.\n- api: Right Party Verification / Account Takeover Detection\n  spec: openapi/syniverse-right-party-verification-openapi.yml, openapi/syniverse-account-takeover-detection-openapi.yml\n  note: No securitySchemes declared in either definition; both publish a sandbox host only.\ninbound_authentication:\n  context: Event Manager delivering events to a customer endpoint\n  options: [NONE, BASIC, 'OAUTH (client_credentials, password, refresh_token)']\n  payload_signing: false\n  note: >-\n    Syniverse does not sign\
  \ event payloads — there is no HMAC signature header. Endpoint\n    authentication is the only verification mechanism available to a webhook consumer.\ndiscovery:\n  openid_configuration: 404 on every host\n  oauth_authorization_server: 404 on every host\n  oauth_protected_resource: 404 on every host\n  see_also: well-known/syniverse-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/authentication/syniverse-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Telecommunications
- United States
- CPaaS
- Messaging
- SMS
- Roaming
- IPX
- Wholesale
- Identity Verification
- SIM Swap
- 10DLC
- Open Gateway
- Network APIs
- Aggregator
---
