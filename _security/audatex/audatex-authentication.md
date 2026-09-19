---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: audatex-audaconnect-api-openapi.yml
  format: yaml
  label: Audatex AudaConnect API
  slug: audatex-audaconnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audatex/refs/heads/main/openapi/audatex-audaconnect-api-openapi.yml
- filename: audatex-audaconnect-bms-api-openapi.yml
  format: yaml
  label: Audatex AudaConnect BMS API
  slug: audatex-audaconnect-bms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audatex/refs/heads/main/openapi/audatex-audaconnect-bms-api-openapi.yml
- filename: audatex-api-gateway-openapi.yml
  format: yaml
  label: Audatex API Gateway (Intelligent Vehicle Inspection)
  slug: audatex-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audatex/refs/heads/main/openapi/audatex-api-gateway-openapi.yml
- filename: audatex-gic-integration-api-openapi.yml
  format: yaml
  label: Audatex GIC API
  slug: audatex-gic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audatex/refs/heads/main/openapi/audatex-gic-integration-api-openapi.yml
- filename: audatex-dashboard-assignment-api-openapi.yml
  format: yaml
  label: Solera Dashboard Assignment API
  slug: audatex-dashboard-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audatex/refs/heads/main/openapi/audatex-dashboard-assignment-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Audatex Authentication
name_suffix: Authentication
oauth_flows:
- implicit
- password
overview: Audatex secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit and password flow(s).
provider_name: Audatex
provider_slug: audatex
scheme_count: 3
schemes:
- description: "JWT Authorization header using the Bearer scheme. \r\n\r\n Enter 'Bearer' [space] and then your token in the text input below.\r\n\r\nExample: \"Bearer 12345abcdef\""
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/audatex-api-gateway-openapi.yml
  type: apiKey
- description: OAuth2 Implicit Grant
  flows:
  - authorizationUrl: https://audaconnect.ax-aee.co.uk/AudaAPI.Portal/Oauth20
    flow: implicit
    scopes: 18
  name: oauth2
  sources:
  - openapi/audatex-audaconnect-api-openapi.yml
  - openapi/audatex-audaconnect-bms-api-openapi.yml
  type: oauth2
- description: Authorization using the JWT Bearer scheme
  flows:
  - flow: password
    scopes: 1
    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token
  name: oauth2
  sources:
  - openapi/audatex-dashboard-assignment-api-openapi.yml
  - openapi/audatex-gic-integration-api-openapi.yml
  type: oauth2
slug: audatex-authentication
source_filename: audatex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: Derived from the five specs in openapi/ (openapi/audatex-api-gateway-openapi.yml, openapi/audatex-audaconnect-api-openapi.yml,\n  openapi/audatex-audaconnect-bms-api-openapi.yml, openapi/audatex-dashboard-assignment-api-openapi.yml, openapi/audatex-gic-integration-api-openapi.yml,\n  openapi/audatex-audaconnect-api-openapi.yml), then upgraded from the AudaConnect developers' guide https://audaconnect.ax-aee.co.uk/AudaAPI.BMSAPI/home/help\n  and the OpenID Connect discovery document at https://dispatch-login-demo.audatex.com/.well-known/openid-configuration\n  (2026-09-17).\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - implicit\n  - password\n  identity_servers:\n  - name: AudaConnect OAuth 2.0 (Audatex UK)\n    authorization_url: https://audaconnect.ax-aee.co.uk/AudaAPI.Portal/OAuth20\n    token_url: https://audaconnect.ax-aee.co.uk/AudaAPI.Portal/OAuth20/token\n    demo_authorization_url:\
  \ https://audaconnect-demo.ax-aee.co.uk/AudaAPI.Portal/OAuth20\n    serves:\n    - Audatex AudaConnect API\n    - Audatex AudaConnect BMS API\n  - name: Solera / Audatex dispatch-login (North America, OpenID Connect)\n    issuer: https://dispatch-login-demo.audatex.com\n    token_url: https://dispatch-login-demo.audatex.com/connect/token\n    authorization_url: https://dispatch-login-demo.audatex.com/connect/authorize\n    discovery: well-known/audatex-openid-configuration.json\n    serves:\n    - Audatex GIC API\n    - Solera Dashboard Assignment API\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: \"JWT Authorization header using the Bearer scheme. \\r\\n\\r\\n Enter 'Bearer' [space] and then your\\\n    \\ token in the text input below.\\r\\n\\r\\nExample: \\\"Bearer 12345abcdef\\\"\"\n  sources:\n  - openapi/audatex-api-gateway-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://audaconnect.ax-aee.co.uk/AudaAPI.Portal/Oauth20\n\
  \    scopes: 18\n  description: OAuth2 Implicit Grant\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n  - openapi/audatex-audaconnect-bms-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token\n    scopes: 1\n  description: Authorization using the JWT Bearer scheme\n  sources:\n  - openapi/audatex-dashboard-assignment-api-openapi.yml\n  - openapi/audatex-gic-integration-api-openapi.yml\ndocs: https://audaconnect.ax-aee.co.uk/AudaAPI.BMSAPI/home/help\ndocumented_flows:\n  source: https://audaconnect.ax-aee.co.uk/AudaAPI.BMSAPI/home/help\n  note: The developers' guide documents THREE OAuth 2.0 flows for AudaConnect while the Swagger securityDefinitions\n    declare only implicit — the spec under-describes the auth surface.\n  flows:\n  - flow: authorization_code\n    rfc: RFC 6749 §1.3.1\n    recommended_for: applications hosted on a secure server needing long-term access\n    authorize:\
  \ GET https://audaconnect.ax-aee.co.uk/AudaAPI.Portal/OAuth20?client_id=&redirect_uri=&scope=&response_type=code\n    token: 'POST https://audaconnect.ax-aee.co.uk/AudaAPI.Portal/OAuth20/token (application/x-www-form-urlencoded:\n      code, client_id, client_secret, redirect_uri, grant_type=authorization_code)'\n    access_token_lifetime_seconds: 1800\n    refresh_token: true\n  - flow: refresh_token\n    token: POST https://audaconnect.ax-aee.co.uk/AudaAPI.Portal/oauth20/token (client_id, client_secret, refresh_token,\n      grant_type=refresh_token) — or client_id/client_secret as HTTP Basic credentials\n    note: Returns a new access token and a new refresh token; losing the refresh token forces the user back through\n      consent.\n  - flow: implicit\n    rfc: RFC 6749 §1.3.2\n    recommended_for: applications running locally on a user device (secret cannot be protected)\n    authorize: GET https://audaconnect.ax-aee.co.uk/AudaAPI.Portal/OAuth20?client_id=&redirect_uri=&scope=&response_type=token\n\
  \    access_token_lifetime_seconds: 1800\n    refresh_token: false\n    caveat: 'Guide: ''Some Audatex APIs will not work with the implicit flow. You should make us aware if you plan\n      to use this flow.'''\n  - flow: password\n    rfc: RFC 6749 §4.3\n    serves:\n    - Audatex GIC API\n    - Solera Dashboard Assignment API\n    token: POST https://dispatch-login-demo.audatex.com/connect/token\n    scope: b2b.fnol.api\n    note: Declared in the GIC and Dashboard Assignment OpenAPIs; the OIDC discovery document also advertises device_authorization_endpoint,\n      introspection and revocation.\n  token_usage: 'Authorization: Bearer <access_token> on every request (e.g. GET /AudaAPI.WebAPI/api/users/me).'\n  scope_delimiter: space (URL-encoded), e.g. scope=BMS.Basic BMS.Extended\n  registration: Applications must be registered and approved in the AudaConnect Portal (My Client Applications);\n    client id, secret and server endpoints are emailed after approval — https://audaconnect.ax-aee.co.uk/AudaAPI.BMSAPI/home/register\n\
  \  unauthenticated_response:\n    audaconnect: 401 text/plain \"Unauthorised. Please provide valid user credentials.\" with a Correlation-Id header\n    api_gateway_and_gic: 401 (JWT Bearer; GIC additionally 400 ApiVersionUnspecified when api-version is missing)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audatex/refs/heads/main/authentication/audatex-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Automotive
- Claims Processing
- Insurance
- Repair Management
- Vehicle Data
- Collision Repair
- Vehicle Inspection
---
