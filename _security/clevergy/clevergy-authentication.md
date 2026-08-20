---
api_key_in:
- header
api_specs:
- filename: clevergy-connect-api-openapi.yml
  format: yaml
  label: Clevergy Connect API
  slug: clevergy-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevergy/refs/heads/main/openapi/clevergy-connect-api-openapi.yml
auth_types:
- apiKey
- bearer-jwt
description: Clevergy documents three distinct authentication paths. Server-to-server calls to the Connect API use a tenant API key in the clevergy-api-key header. Embedded microfrontends (web components) authenticate with a short-lived user JWT that the integrator's own backend mints by calling the Connect API with its API key. A third "login with token" path passes that same JWT in a URL query string to open the full Clevergy webview on a tenant subdomain.
kind: authentication
layout: security
method: searched
name: Clevergy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clevergy secures its APIs with apiKey and bearer-jwt across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clevergy
provider_slug: clevergy
scheme_count: 3
schemes:
- audience: server-to-server
  description: Tenant API key for the Connect API. Issued per environment by Clevergy — the docs instruct integrators to request it from their Customer Success Manager, and it is also revealed and regenerable from the Operations Portal under Settings > API key management. Regenerating immediately invalidates the previous key.
  in: header
  name: key
  parameter: clevergy-api-key
  provisioning:
    channel: Customer Success Manager request, or Operations Portal > Settings > API key management
    docs: https://docs.clever.gy/helpdesk/portal/settings/api-key-management
    rotation: Self-service regenerate in the portal; regeneration revokes the prior key immediately
    self_serve: false
  sources:
  - openapi/clevergy-connect-api-openapi.yml
  - https://docs.clever.gy/developer/getting-started/authentication
  type: apiKey
- audience: browser / embedded microfrontend
  bearerFormat: JWT
  description: 'Per-user JWT (RFC 7519) minted by the Connect API operation retrieveUserAccessToken (GET /auth/{userId}/token). Passed to a microfrontend via its data-token attribute. Expires after 1 hour. The docs are explicit that the API key must never reach the end user: the integrator''s own API acts as a secure proxy that holds the key and hands out only the JWT.'
  minted_by: retrieveUserAccessToken
  name: user-jwt
  scheme: bearer
  sources:
  - https://docs.clever.gy/developer/getting-started/authentication
  ttl: 3600
  type: http
- audience: hosted webview
  description: The same user JWT can be passed as a token query parameter to open the entire Clevergy webview at https://{tenant_name}.clever.gy/login-with-token?token=... The tenant subdomain is assigned by Clevergy on request. Same 1 hour expiry.
  name: login-with-token
  sources:
  - https://docs.clever.gy/developer/getting-started/authentication
  type: query-token
  url_template: https://{tenant_name}.clever.gy/login-with-token?token={jwt}
slug: clevergy-authentication
source_filename: clevergy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: openapi/clevergy-connect-api-openapi.yml\ndocs: https://docs.clever.gy/developer/getting-started/authentication\ndescription: >-\n  Clevergy documents three distinct authentication paths. Server-to-server calls to the Connect\n  API use a tenant API key in the clevergy-api-key header. Embedded microfrontends (web\n  components) authenticate with a short-lived user JWT that the integrator's own backend mints\n  by calling the Connect API with its API key. A third \"login with token\" path passes that same\n  JWT in a URL query string to open the full Clevergy webview on a tenant subdomain.\nsummary:\n  types:\n  - apiKey\n  - bearer-jwt\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: key\n  type: apiKey\n  in: header\n  parameter: clevergy-api-key\n  audience: server-to-server\n  description: >-\n    Tenant API key for the Connect API. Issued per environment by Clevergy — the docs instruct\n    integrators\
  \ to request it from their Customer Success Manager, and it is also revealed and\n    regenerable from the Operations Portal under Settings > API key management. Regenerating\n    immediately invalidates the previous key.\n  provisioning:\n    self_serve: false\n    channel: Customer Success Manager request, or Operations Portal > Settings > API key management\n    rotation: Self-service regenerate in the portal; regeneration revokes the prior key immediately\n    docs: https://docs.clever.gy/helpdesk/portal/settings/api-key-management\n  sources:\n  - openapi/clevergy-connect-api-openapi.yml\n  - https://docs.clever.gy/developer/getting-started/authentication\n- name: user-jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  audience: browser / embedded microfrontend\n  description: >-\n    Per-user JWT (RFC 7519) minted by the Connect API operation retrieveUserAccessToken\n    (GET /auth/{userId}/token). Passed to a microfrontend via its data-token attribute. Expires\n    after\
  \ 1 hour. The docs are explicit that the API key must never reach the end user: the\n    integrator's own API acts as a secure proxy that holds the key and hands out only the JWT.\n  minted_by: retrieveUserAccessToken\n  ttl: 3600\n  sources:\n  - https://docs.clever.gy/developer/getting-started/authentication\n- name: login-with-token\n  type: query-token\n  audience: hosted webview\n  description: >-\n    The same user JWT can be passed as a token query parameter to open the entire Clevergy\n    webview at https://{tenant_name}.clever.gy/login-with-token?token=... The tenant subdomain\n    is assigned by Clevergy on request. Same 1 hour expiry.\n  url_template: https://{tenant_name}.clever.gy/login-with-token?token={jwt}\n  sources:\n  - https://docs.clever.gy/developer/getting-started/authentication\nnotes:\n- >-\n  No OAuth 2.0 or OpenID Connect surface is published for the Connect API itself; the only OAuth\n  in the platform is outbound, to third-party inverter vendors (Huawei OAuth\
  \ is named as the\n  prerequisite for battery control actions). scopes/ is therefore not applicable.\n- >-\n  No /.well-known/openid-configuration or /.well-known/oauth-authorization-server document is\n  served on any Clevergy host — see well-known/clevergy-well-known.yml for the probe record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clevergy/refs/heads/main/authentication/clevergy-authentication.yml
summary_line: apiKey/bearer-jwt · 3 schemes
tags:
- Company
- Climate Tech
- Energy
- Energy Management
- Utilities
- Smart Meter
- Solar
- Home Energy
- Battery Storage
- Electric Vehicle Charging
- Smart Home
- Sustainability
- Spain
- White Label
- Embedded Components
- Webhook
---
