---
api_key_in:
- header
api_specs:
- filename: america-movil-check-sim-swap-api-openapi.yml
  format: yaml
  label: América Móvil Check SIM swap API
  slug: america-movil-check-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-check-sim-swap-api-openapi.yml
- filename: america-movil-device-locations-api-openapi.yml
  format: yaml
  label: América Móvil Device Locations API
  slug: america-movil-device-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-device-locations-api-openapi.yml
- filename: america-movil-location-verification-api-openapi.yml
  format: yaml
  label: América Móvil Location verification API
  slug: america-movil-location-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-location-verification-api-openapi.yml
- filename: america-movil-retrieve-sim-swap-date-api-openapi.yml
  format: yaml
  label: América Móvil Retrieve SIM swap date API
  slug: america-movil-retrieve-sim-swap-date-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/openapi/america-movil-retrieve-sim-swap-date-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: 'Every callable América Móvil API is Claro Brasil''s, and every one of them authenticates the same way: OAuth 2.0 client credentials against https://api.claro.com.br/oauth2/v1/token, exchanged for a bearer token. The wrinkle is the header. The 2019-generation "customers" services send both the Basic credential and the bearer token in a non-standard `x-client-auth` header and add an `X-CustomerID` partner header; the 2023-2025 Open Gateway services use the standard `Authorization` header. Geofencing additionally requires an `X-API-Key`. There is no three-legged flow, no CIBA and no user consent mechanism anywhere in the estate.'
kind: authentication
layout: security
method: searched
name: America Movil Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: América Móvil secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: América Móvil
provider_slug: america-movil
scheme_count: 4
schemes:
- detail: scopes/america-movil-scopes.yml
  flows:
  - absoluteTokenUrl: https://api.claro.com.br/oauth2/v1/token
    flow: clientCredentials
    scopes: 2 declared at operation level, none in the flow map
    tokenUrl: /oauth2/v1/token
  name: OAuth2
  sources:
  - openapi/america-movil-claro-device-location-openapi.json
  - openapi/america-movil-claro-sim-swap-openapi.json
  type: oauth2
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/america-movil-claro-device-location-openapi.json
  type: http
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/america-movil-claro-device-location-openapi.json
  type: http
- in: header
  name: ApiKeyAuth
  note: Also required alongside the bearer token on the Geofencing subscription endpoint.
  parameter: X-API-Key
  sources:
  - openapi/america-movil-claro-device-location-openapi.json
  - https://www.claroinsight.com.br/pt-br/geofencing
  type: apiKey
slug: america-movil-authentication
source_filename: america-movil-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  openapi/america-movil-claro-device-location-openapi.json,\n  openapi/america-movil-claro-sim-swap-openapi.json, and the authentication\n  sections plus code samples published on the Claro Insight product pages.\ndocs: https://www.claroinsight.com.br/pt-br/catalogo-api\ndescription: >-\n  Every callable América Móvil API is Claro Brasil's, and every one of them\n  authenticates the same way: OAuth 2.0 client credentials against\n  https://api.claro.com.br/oauth2/v1/token, exchanged for a bearer token. The\n  wrinkle is the header. The 2019-generation \"customers\" services send both the\n  Basic credential and the bearer token in a non-standard `x-client-auth` header\n  and add an `X-CustomerID` partner header; the 2023-2025 Open Gateway services\n  use the standard `Authorization` header. Geofencing additionally requires an\n  `X-API-Key`. There is no three-legged flow, no CIBA and no user consent\n  mechanism anywhere\
  \ in the estate.\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  three_legged: false\n  ciba: false\n  mtls: false\n  openid_connect: false\ntoken_endpoint:\n  url: https://api.claro.com.br/oauth2/v1/token\n  probe_status: 401\n  grant_type: client_credentials\n  request_content_type: application/x-www-form-urlencoded\n  credential_transport:\n  - 'Authorization: Basic base64(client_id:client_secret)'\n  - 'x-client-auth: Basic base64(client_id:client_secret)'\n  response_field: access_token\n  metadata_document: none (no RFC 8414 / OIDC discovery — see well-known/america-movil-well-known.yml)\ncredential_issuance:\n  self_serve: false\n  process: >-\n    Register at https://www.claroinsight.com.br/user/register, log in, request the\n    API from the catalog, and receive client_id/client_secret once the request is\n    approved. Credentials, endpoints and Swagger downloads are all behind the login.\n  ip_filtering: >-\n    The\
  \ gateway documents 403 for source IPs without permission, so allow-listing\n    is part of the access model.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/v1/token\n    absoluteTokenUrl: https://api.claro.com.br/oauth2/v1/token\n    scopes: 2 declared at operation level, none in the flow map\n  sources:\n  - openapi/america-movil-claro-device-location-openapi.json\n  - openapi/america-movil-claro-sim-swap-openapi.json\n  detail: scopes/america-movil-scopes.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/america-movil-claro-device-location-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/america-movil-claro-device-location-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/america-movil-claro-device-location-openapi.json\n  - https://www.claroinsight.com.br/pt-br/geofencing\n  note: Also required alongside\
  \ the bearer token on the Geofencing subscription endpoint.\nnon_standard_headers:\n- header: x-client-auth\n  carries: 'Basic <base64> on the token call, Bearer <token> on the API call'\n  used_by: [Claro Alerta, Claro Score, Claro Valida Telefone, Claro Valida Endereço 2.0, Tenure]\n- header: X-CustomerID\n  carries: partner/tenant identifier, e.g. claro_exemplo\n  used_by: [Claro Alerta, Claro Score, Claro Valida Telefone, Claro Valida Endereço 2.0]\ngaps:\n- No metadata document — clients cannot discover the token endpoint programmatically.\n- No refresh-token, token-introspection or revocation endpoint is documented.\n- >-\n  No subject authorization. CAMARA specifies three-legged/CIBA authorization for\n  SIM Swap, Number Verification, KYC and Device Location; Claro implements\n  two-legged client credentials, and the LGPD consent its own docs require for\n  Device Location Verify is contractual rather than protocol-enforced.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/america-movil/refs/heads/main/authentication/america-movil-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Telecommunications
- Mexico
- Latin America
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- Identity Verification
- Device Location
- Broadband
- 5G
- Carrier
---
