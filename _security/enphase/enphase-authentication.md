---
api_key_in:
- query
- header
api_specs:
- filename: enphase-monitoring-api-openapi.json
  format: json
  label: Enphase Monitoring API
  slug: enphase-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase/refs/heads/main/openapi/enphase-monitoring-api-openapi.json
- filename: enphase-commissioning-api-openapi.json
  format: json
  label: Enphase Commissioning API
  slug: enphase-commissioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase/refs/heads/main/openapi/enphase-commissioning-api-openapi.json
- filename: enphase-vpp-api-openapi.json
  format: json
  label: Enphase VPP API
  slug: enphase-vpp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase/refs/heads/main/openapi/enphase-vpp-api-openapi.json
auth_types:
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Enphase Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
- clientCredentials
overview: Enphase Energy secures its APIs with oauth2, apiKey, and http across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, password, and clientCredentials flow(s).
provider_name: Enphase Energy
provider_slug: enphase
scheme_count: 6
schemes:
- authorizationUrl: https://api.enphaseenergy.com/oauth/authorize
  client_authentication: HTTP Basic - base64(client_id:client_secret) in the Authorization header
  consent: The system owner (homeowner) signs in with Enlighten credentials, sees the application name, developer name and requested access controls, then approves or rejects. Rejection returns access_denied as a query parameter on the redirect_uri.
  default_redirect_uri: https://api.enphaseenergy.com/oauth/redirect_uri
  docs: https://developer-v4.enphase.com/docs/quickstart.html
  flow: authorizationCode
  name: oauth2_authorization_code
  refresh: POST /oauth/token with grant_type=refresh_token; a new refresh_token is issued each time
  state_parameter: supported and recommended, echoed back to the redirect_uri
  tokenUrl: https://api.enphaseenergy.com/oauth/token
  token_response_fields:
  - access_token
  - token_type
  - refresh_token
  - expires_in
  - scope
  - enl_uid
  - enl_cid
  - enl_password_last_changed
  - is_internal_app
  - app_type
  - jti
  token_ttl: access_token 1 day (expires_in 86393), refresh_token 1 month
  type: oauth2
  used_by: Enphase Monitoring API (developer applications on the Watt, Kilowatt and Megawatt plans)
- client_authentication: HTTP Basic - base64(client_id:client_secret) in the Authorization header
  credentials: Enphase cloud (Enlighten) email and password of the installer - not the developer portal account
  docs: https://developer-v4.enphase.com/docs/quickstart.html
  eligibility: Partner applications can only be created by a self-installer or a member of an installer company with at least ten installed systems; the application starts in a pending state and is enabled after Enphase verification.
  flow: password
  name: oauth2_password
  tokenUrl: https://api.enphaseenergy.com/oauth/token
  token_ttl: access_token 1 day, refresh_token 1 month
  type: oauth2
  used_by: Enphase Commissioning API and full Monitoring API access on the Partner plan
- client_authentication: base64(clientId:clientSecret) in the Authorization header, Content-Type application/x-www-form-urlencoded, Accept application/json
  flow: clientCredentials
  name: oauth2_client_credentials
  source_operation: openapi/enphase-vpp-api-openapi.json#getToken
  tokenUrl: https://vpp.enphaseenergy.com/auth/oauth2/token
  token_ttl: 3600 seconds, no refresh token - regenerate through the same call
  type: oauth2
  used_by: Enphase VPP API (grid-services partners)
- description: The per-application API key issued by the developer portal, sent on every request as ?key=. It must belong to the same application as the client_id the access token was minted for - a mismatch returns 401 "API Key -Client mismatch".
  in: query
  name: api_key_query
  parameter: key
  type: apiKey
  used_by: Enphase Monitoring API and Enphase Commissioning API
- description: Unique API key of the grid-services partner account, required on every VPP operation.
  in: header
  name: api_key_header
  parameter: x-api-key
  type: apiKey
  used_by: Enphase VPP API
- description: Authorization- Bearer <access_token> on every request alongside the API key.
  name: bearer
  scheme: bearer
  type: http
  used_by: all three APIs
slug: enphase-authentication
source_filename: enphase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/enphase-monitoring-api-openapi.json, openapi/enphase-commissioning-api-openapi.json,\n  openapi/enphase-vpp-api-openapi.json\ndocs: https://developer-v4.enphase.com/docs/quickstart.html\nnotes: >-\n  None of the three published Enphase specs declare a securityScheme - the Monitoring and\n  Commissioning Swagger 2.0 documents carry no securityDefinitions at all, and the VPP OpenAPI\n  3.0.1 document models its credentials as ordinary Authorization and x-api-key header\n  parameters on every operation. The profile below is therefore searched from the Enphase\n  Developer Portal quick start guide and the VPP Auth controller, not derived from the specs.\n  Every Enphase API call carries two credentials at once: an OAuth 2.0 bearer access token AND\n  the application API key.\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  - http\n  api_key_in:\n  - query\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - password\n\
  \  - clientCredentials\n  two_factor_credential: true\nschemes:\n- name: oauth2_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  used_by: Enphase Monitoring API (developer applications on the Watt, Kilowatt and Megawatt plans)\n  authorizationUrl: https://api.enphaseenergy.com/oauth/authorize\n  tokenUrl: https://api.enphaseenergy.com/oauth/token\n  default_redirect_uri: https://api.enphaseenergy.com/oauth/redirect_uri\n  client_authentication: HTTP Basic - base64(client_id:client_secret) in the Authorization header\n  state_parameter: supported and recommended, echoed back to the redirect_uri\n  consent: >-\n    The system owner (homeowner) signs in with Enlighten credentials, sees the application name,\n    developer name and requested access controls, then approves or rejects. Rejection returns\n    access_denied as a query parameter on the redirect_uri.\n  token_ttl: access_token 1 day (expires_in 86393), refresh_token 1 month\n  refresh: POST /oauth/token with grant_type=refresh_token;\
  \ a new refresh_token is issued each time\n  token_response_fields:\n  - access_token\n  - token_type\n  - refresh_token\n  - expires_in\n  - scope\n  - enl_uid\n  - enl_cid\n  - enl_password_last_changed\n  - is_internal_app\n  - app_type\n  - jti\n  docs: https://developer-v4.enphase.com/docs/quickstart.html\n- name: oauth2_password\n  type: oauth2\n  flow: password\n  used_by: Enphase Commissioning API and full Monitoring API access on the Partner plan\n  tokenUrl: https://api.enphaseenergy.com/oauth/token\n  credentials: Enphase cloud (Enlighten) email and password of the installer - not the developer\n    portal account\n  client_authentication: HTTP Basic - base64(client_id:client_secret) in the Authorization header\n  eligibility: >-\n    Partner applications can only be created by a self-installer or a member of an installer\n    company with at least ten installed systems; the application starts in a pending state and is\n    enabled after Enphase verification.\n  token_ttl: access_token\
  \ 1 day, refresh_token 1 month\n  docs: https://developer-v4.enphase.com/docs/quickstart.html\n- name: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  used_by: Enphase VPP API (grid-services partners)\n  tokenUrl: https://vpp.enphaseenergy.com/auth/oauth2/token\n  client_authentication: base64(clientId:clientSecret) in the Authorization header,\n    Content-Type application/x-www-form-urlencoded, Accept application/json\n  token_ttl: 3600 seconds, no refresh token - regenerate through the same call\n  source_operation: openapi/enphase-vpp-api-openapi.json#getToken\n- name: api_key_query\n  type: apiKey\n  in: query\n  parameter: key\n  used_by: Enphase Monitoring API and Enphase Commissioning API\n  description: >-\n    The per-application API key issued by the developer portal, sent on every request as ?key=.\n    It must belong to the same application as the client_id the access token was minted for -\n    a mismatch returns 401 \"API Key -Client mismatch\".\n\
  - name: api_key_header\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  used_by: Enphase VPP API\n  description: Unique API key of the grid-services partner account, required on every VPP operation.\n- name: bearer\n  type: http\n  scheme: bearer\n  used_by: all three APIs\n  description: Authorization- Bearer <access_token> on every request alongside the API key.\ntransport_security:\n  tls_minimum: TLS 1.2\n  announced: Effective April 1, 2023 the Enphase API only supports TLS 1.2 and will not accept\n    applications on older TLS versions.\n  source: https://developer-v4.enphase.com/docs/quickstart.html\ngaps:\n- No OpenID Connect discovery document; /.well-known/openid-configuration returns 404 on\n  api.enphaseenergy.com and developer-v4.enphase.com.\n- No RFC 8414 authorization-server metadata; /.well-known/oauth-authorization-server returns 404.\n- No PKCE, device code, or mTLS option documented.\n- The Commissioning and Partner-plan flows use the OAuth 2.0 resource-owner\
  \ password grant, which\n  is deprecated by OAuth 2.1 and requires the installer to hand raw Enlighten credentials to the\n  client application.\nrelated:\n- scopes/enphase-scopes.yml\n- conventions/enphase-conventions.yml\n- plans/enphase-plans.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enphase/refs/heads/main/authentication/enphase-authentication.yml
summary_line: oauth2/apiKey/http · 6 schemes
tags:
- Energy
- United States
- Solar
- DER
- Renewables
- Battery Storage
- EV Charging
- Demand Response
- Virtual Power Plant
- Grid Services
- Microinverters
- Home Energy Management
- Smart Metering
- Telemetry
---
