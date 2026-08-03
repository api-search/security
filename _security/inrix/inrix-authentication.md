---
api_key_in:
- query
- header
api_specs:
- filename: inrix-user-accounts-openapi-original.json
  format: json
  label: INRIX User Accounts System (UAS) API
  slug: inrix-user-accounts-system-uas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-user-accounts-openapi-original.json
- filename: inrix-parkme-openapi-original.json
  format: json
  label: INRIX Parking API (INRIX Parking Services 3.0 / ParkMe)
  slug: inrix-parking-api-inrix-parking-services-30-parkme
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-parkme-openapi-original.json
- filename: inrix-signals-analytics-openapi-original.json
  format: json
  label: INRIX Signals Analytics API
  slug: inrix-signals-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/openapi/inrix-signals-analytics-openapi-original.json
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Inrix Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: INRIX secures its APIs with http, apiKey, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: INRIX
provider_slug: inrix
scheme_count: 3
schemes:
- name: Basic
  note: HTTP Basic is declared on the Parkme/INRIX Parking Services spec for operator-level endpoints (for example reservation creation).
  scheme: basic
  sources:
  - openapi/inrix-parkme-openapi-original.json
  type: http
- bearerFormat: JWT
  name: Bearer Token
  note: The INRIX Signals Analytics API declares a JWT bearer scheme; the token is the UAS access token.
  scheme: bearer
  sources:
  - openapi/inrix-signals-analytics-openapi-original.json
  type: http
- in: query
  name: accessToken
  note: Documented across the Traffic, Parking, Analytics and data-stream APIs as an alternative to the Authorization header.
  sources:
  - https://docs.inrix.com/sendingdata/gpsdatastream/
  - https://docs.inrix.com/traffic/segmentspeed/
  type: apiKey
slug: inrix-authentication
source_filename: inrix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://docs.inrix.com/authentication/getting_authorized/\ndocs: https://docs.inrix.com/authentication/getting_authorized/\nsummary:\n  types:\n  - http\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  - header\n  oauth2_flows:\n  - clientCredentials\n  note: 'Every INRIX product API is gated by a bearer access token minted by the INRIX User Accounts System (UAS).\n    The token may be presented either as an `accessToken` query-string parameter or as an `Authorization: Bearer`\n    header.'\nprimary_flow:\n  name: UAS appToken\n  description: Exchange an INRIX-issued appId (GUID) and a SHA-1 hashToken for a time-limited access token.\n  token_endpoint: https://uas-api.inrix.com/v1/appToken\n  operation: openapi/inrix-user-accounts-openapi-original.json#Application_GetAppToken\n  parameters:\n  - name: appId\n    in: query\n    description: Unique GUID provided by INRIX.\n  - name: hashToken\n    in: query\n    description:\
  \ SHA-1 hash of the lowercase UTF-8 string \"AppId|AppKey\".\n  response_fields:\n  - token\n  - expiry (token validity period)\n  presentation:\n  - style: query\n    parameter: accessToken\n  - style: header\n    header: Authorization\n    format: Bearer {UAS-TOKEN}\n  guidance: Cache the token and reuse it for subsequent requests until it is close to expiring; tokens are not interchangeable\n    between environments.\nadditional_flows:\n- name: OAuth2 application token\n  token_endpoint: https://uas-api.inrix.com/v1/oauth2/apptoken\n  operation: openapi/inrix-user-accounts-openapi-original.json#Application_OAuth2Token\n  note: OAuth2-shaped application token endpoint exposed by UAS. No scope vocabulary is published.\n- name: OAuth2 user token\n  token_endpoint: https://uas-api.inrix.com/v1/oauth2/token\n  operation: openapi/inrix-user-accounts-openapi-original.json#Auth_OAuth2Token\n- name: User sign-in\n  token_endpoint: https://uas-api.inrix.com/v1/signin\n  operation: openapi/inrix-user-accounts-openapi-original.json#Auth_Signin\n\
  - name: Token renewal\n  token_endpoint: https://uas-api.inrix.com/v1/renewtoken\n  operation: openapi/inrix-user-accounts-openapi-original.json#Auth_RenewToken\n  parameters:\n  - name: refreshToken\n    in: query\n    required: true\n  - name: oAuthToken\n    in: query\n- name: Token validation\n  token_endpoint: https://uas-api.inrix.com/v1/validatetoken\n  operation: openapi/inrix-user-accounts-openapi-original.json#Auth_CheckToken\n- name: GetSecurityToken (legacy Connected Services)\n  token_endpoint: https://{serverPath}.inrix.com/traffic/Inrix.ashx?Action=GetSecurityToken\n  parameters:\n  - name: vendorId\n    in: query\n  - name: consumerId\n    in: query\n  - name: format\n    in: query\n    description: XML or JSON; XML is the default.\n  response_fields:\n  - token\n  - tokenExpireDtUtc\n  - serverPath\n  presentation:\n  - style: query\n    parameter: token\n  status: legacy\n  note: The legacy gateway returns the regional server path the caller must use for all subsequent\
  \ requests (for\n    example na-api2.inrix.com or eu.api.inrix.com).\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/inrix-parkme-openapi-original.json\n  note: HTTP Basic is declared on the Parkme/INRIX Parking Services spec for operator-level endpoints (for example\n    reservation creation).\n- name: Bearer Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/inrix-signals-analytics-openapi-original.json\n  note: The INRIX Signals Analytics API declares a JWT bearer scheme; the token is the UAS access token.\n- name: accessToken\n  type: apiKey\n  in: query\n  sources:\n  - https://docs.inrix.com/sendingdata/gpsdatastream/\n  - https://docs.inrix.com/traffic/segmentspeed/\n  note: Documented across the Traffic, Parking, Analytics and data-stream APIs as an alternative to the Authorization\n    header.\nno_oauth_scopes: true\nscope_note: INRIX publishes OAuth2-shaped token endpoints but no scope vocabulary or permissions\
  \ reference; entitlement\n  is set per application/account by INRIX, not by requested scope.\ncredential_request: https://inrix.com/contact/\nx-evidence:\n- url: https://docs.inrix.com/authentication/getting_authorized/\n  fetched: '2026-08-01'\n  http_status: 200\n- url: https://uas-api.inrix.com/swagger/docs/v1\n  fetched: '2026-08-01'\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inrix/refs/heads/main/authentication/inrix-authentication.yml
summary_line: http/apiKey/oauth2 · 3 schemes
tags:
- Transportation
- Traffic
- Mobility
- Parking
- Geospatial
- Location Data
- Analytics
- Automotive
- Smart Cities
- Routing
- Connected Vehicles
- Road Network
- Data
- Fleet
- Intelligent Transportation Systems
---
