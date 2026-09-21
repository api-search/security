---
anonymous_access: false
api_key_in: []
api_specs:
- filename: airalo-partner-api-openapi.yml
  format: yaml
  label: Airalo Partner API
  slug: airalo-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airalo/refs/heads/main/openapi/airalo-partner-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Airalo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airalo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Airalo
provider_slug: airalo
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Access token from POST /v2/token (OAuth2 client_credentials grant with client_id + client_secret). Tokens are valid for 24 hours; the token endpoint is limited to 3 requests per minute.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/airalo-partner-api-openapi.yml
  type: http
slug: airalo-authentication
source_filename: airalo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/airalo-partner-api-openapi.yml\ndocs:\n- https://developers.partners.airalo.com/request-access-token-11883021e0\n- https://developers.partners.airalo.com/ip-allowlist-whitelisting-2327548m0\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Access token from POST /v2/token (OAuth2 client_credentials grant with client_id\n    + client_secret). Tokens are valid for 24 hours; the token endpoint is limited to 3 requests\n    per minute.\n  sources:\n  - openapi/airalo-partner-api-openapi.yml\ntoken_endpoint:\n  operation_id: requestAccessToken\n  path: POST /v2/token\n  grant_type: client_credentials\n  content_type: application/x-www-form-urlencoded\n  parameters: [client_id, client_secret, grant_type]\n  response: {token_type, expires_in, access_token}\n  lifetime_hours: 24\n  rate_limit: 3 requests per minute\n  scopes_published: false\n  docs:\
  \ https://developers.partners.airalo.com/request-access-token-11883021e0\n  note: >-\n    An RFC 6749 client-credentials exchange that mints a bearer token, but Airalo declares no oauth2\n    securityScheme in its published fragments and documents no scopes — authorization is all-or-nothing per\n    credential pair. No scopes/ artifact is emitted for that reason.\ncredential_issuance:\n  location: Partner Platform (https://app.partners.airalo.com)\n  self_serve: false\n  note: Credentials are issued after an account manager onboards the company; the same pair works in Sandbox and Production.\nnetwork_controls:\n  ip_allowlist:\n    supported: true\n    default_state: off\n    scope: per company, covers Sandbox and Production\n    formats: [IPv4, IPv6, IPv4 CIDR, IPv6 CIDR]\n    max_entries: 100\n    rejection: HTTP 403, body code 89\n    effective: immediately on save\n    docs: https://developers.partners.airalo.com/ip-allowlist-whitelisting-2327548m0\nconsole_sso:\n  protocol: SAML 2.0\n\
  \  applies_to: Partner Platform console, not the API\n  idps: [Okta, OneLogin, Google Workspace, Microsoft Azure]\n  roles: [Admin, Operations, Finance, Employee]\n  domain_verification: TXT record within 72 hours\n  docs: https://developers.partners.airalo.com/faq-752238m0\nwebhook_authentication:\n  direction: inbound-to-partner\n  header: airalo-signature\n  algorithm: HMAC-SHA512\n  key: partner API secret\n  docs: https://developers.partners.airalo.com/webhook-definition-1380483m0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airalo/refs/heads/main/authentication/airalo-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- eSIM
- Telecommunications
- Travel
- Connectivity
- Mobile Data
- Roaming
- Partner API
- Webhook
- Singapore
---
