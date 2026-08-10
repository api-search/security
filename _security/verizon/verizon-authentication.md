---
api_key_in:
- header
api_specs:
- filename: verizon-accounts-api-openapi.yml
  format: yaml
  label: Verizon Accounts API
  slug: verizon-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/openapi/verizon-accounts-api-openapi.yml
- filename: verizon-callbacks-api-openapi.yml
  format: yaml
  label: Verizon Callbacks API
  slug: verizon-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/openapi/verizon-callbacks-api-openapi.yml
- filename: verizon-devices-api-openapi.yml
  format: yaml
  label: Verizon Devices API
  slug: verizon-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/openapi/verizon-devices-api-openapi.yml
- filename: verizon-session-api-openapi.yml
  format: yaml
  label: Verizon Session API
  slug: verizon-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/openapi/verizon-session-api-openapi.yml
- filename: verizon-sms-api-openapi.yml
  format: yaml
  label: Verizon SMS API
  slug: verizon-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/openapi/verizon-sms-api-openapi.yml
auth_types:
- oauth2
- apiKey
description: Verizon ThingSpace uses a two-token model. An OAuth 2.0 client-credentials grant issues a ThingSpace access token from the application key/secret; that token is then exchanged, together with UWS (Unified Web Services) username/password, for a VZ-M2M session token that authorizes every Connectivity Management call. Both tokens must be present on Connectivity Management requests.
kind: authentication
layout: security
method: searched
name: Verizon Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Verizon secures its APIs with oauth2 and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Verizon
provider_slug: verizon
scheme_count: 3
schemes:
- credential: Application key and secret, colon-joined and Base64-encoded
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://thingspace.verizon.com/api/ts/v1/oauth2/token
  name: ThingSpaceOAuth2
  request_header: 'Authorization: Basic <base64(key:secret)>'
  response_header: 'Authorization: Bearer <access_token>'
  sources:
  - https://thingspace.verizon.com/documentation/apis/connectivity-management/getting-started/getting-credentials.html
  token_ttl: 3600
  token_ttl_note: Valid for one hour from first issue; further token requests inside that window return the same token rather than minting a new one.
  type: oauth2
- credential: ThingSpace OAuth token + UWS username/password
  in: header
  name: VZM2MSessionToken
  obtained_via: openapi/verizon-session-api-openapi.yml#loginSession
  parameter_name: VZ-M2M-Token
  sources:
  - openapi/verizon-session-api-openapi.yml
  - https://thingspace.verizon.com/documentation/apis/connectivity-management/getting-started/getting-credentials.html
  token_ttl_note: Remains valid while the application keeps using it; expires after 20 minutes of inactivity. Explicitly terminated with the End Connectivity Management Session operation.
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://thingspace.verizon.com/api/m2m/v2/session/token
  name: OAuth2ClientCredentials
  note: The scheme as declared in the harvested OpenAPI. The docs-confirmed token issuer is https://thingspace.verizon.com/api/ts/v1/oauth2/token; the /api/m2m/v2 path in the spec is the Connectivity Management base, not the token endpoint.
  sources:
  - openapi/verizon-accounts-api-openapi.yml
  - openapi/verizon-callbacks-api-openapi.yml
  - openapi/verizon-devices-api-openapi.yml
  - openapi/verizon-session-api-openapi.yml
  - openapi/verizon-sms-api-openapi.yml
  type: oauth2
slug: verizon-authentication
source_filename: verizon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/verizon-session-api-openapi.yml\ndocs: https://thingspace.verizon.com/documentation/apis/connectivity-management/getting-started/getting-credentials.html\ndescription: >-\n  Verizon ThingSpace uses a two-token model. An OAuth 2.0 client-credentials grant\n  issues a ThingSpace access token from the application key/secret; that token is then\n  exchanged, together with UWS (Unified Web Services) username/password, for a\n  VZ-M2M session token that authorizes every Connectivity Management call. Both\n  tokens must be present on Connectivity Management requests.\nsummary:\n  types:\n    - oauth2\n    - apiKey\n  oauth2_flows:\n    - clientCredentials\n  api_key_in: [header]\nschemes:\n  - name: ThingSpaceOAuth2\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://thingspace.verizon.com/api/ts/v1/oauth2/token\n        scopes: 3\n    credential: Application key and secret, colon-joined\
  \ and Base64-encoded\n    request_header: 'Authorization: Basic <base64(key:secret)>'\n    response_header: 'Authorization: Bearer <access_token>'\n    token_ttl: 3600\n    token_ttl_note: >-\n      Valid for one hour from first issue; further token requests inside that window\n      return the same token rather than minting a new one.\n    sources:\n      - https://thingspace.verizon.com/documentation/apis/connectivity-management/getting-started/getting-credentials.html\n  - name: VZM2MSessionToken\n    type: apiKey\n    in: header\n    parameter_name: VZ-M2M-Token\n    obtained_via: openapi/verizon-session-api-openapi.yml#loginSession\n    credential: ThingSpace OAuth token + UWS username/password\n    token_ttl_note: >-\n      Remains valid while the application keeps using it; expires after 20 minutes of\n      inactivity. Explicitly terminated with the End Connectivity Management Session\n      operation.\n    sources:\n      - openapi/verizon-session-api-openapi.yml\n      - https://thingspace.verizon.com/documentation/apis/connectivity-management/getting-started/getting-credentials.html\n\
  \  - name: OAuth2ClientCredentials\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://thingspace.verizon.com/api/m2m/v2/session/token\n        scopes: 3\n    sources:\n      - openapi/verizon-accounts-api-openapi.yml\n      - openapi/verizon-callbacks-api-openapi.yml\n      - openapi/verizon-devices-api-openapi.yml\n      - openapi/verizon-session-api-openapi.yml\n      - openapi/verizon-sms-api-openapi.yml\n    note: >-\n      The scheme as declared in the harvested OpenAPI. The docs-confirmed token\n      issuer is https://thingspace.verizon.com/api/ts/v1/oauth2/token; the\n      /api/m2m/v2 path in the spec is the Connectivity Management base, not the\n      token endpoint.\ncredential_management:\n  console: https://thingspace.verizon.com\n  path: Account Settings > Key Management > My Keys\ncombined_request_headers:\n  - name: Authorization\n    value: Bearer <ThingSpace access token>\n    required_on: all requests\n  - name: VZ-M2M-Token\n \
  \   value: <session token>\n    required_on: Connectivity Management requests\nrelated:\n  scopes: scopes/verizon-scopes.yml\n  conventions: conventions/verizon-conventions.yml\n  sandbox: sandbox/verizon-sandbox.yml\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n    - https://thingspace.verizon.com/documentation/apis/connectivity-management/getting-started/getting-credentials.html\n    - https://thingspace.verizon.com/documentation/apis/connectivity-management/getting-started.html\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/authentication/verizon-authentication.yml
summary_line: oauth2/apiKey · 3 schemes
tags:
- Wireless
- Telecommunications
- IoT
- 5G
- Enterprise
- Network APIs
- Fortune 100
---
