---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: avnet-iotconnect-master-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT Master API
  slug: avnet-iotconnect-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-master-openapi.yml
- filename: avnet-iotconnect-auth-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT Authenticate API
  slug: avnet-iotconnect-authenticate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-auth-openapi.yml
- filename: avnet-iotconnect-user-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT User API
  slug: avnet-iotconnect-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-user-openapi.yml
- filename: avnet-iotconnect-device-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT Device API
  slug: avnet-iotconnect-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-device-openapi.yml
- filename: avnet-iotconnect-firmware-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT Firmware API
  slug: avnet-iotconnect-firmware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-firmware-openapi.yml
- filename: avnet-iotconnect-event-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT Event API
  slug: avnet-iotconnect-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-event-openapi.yml
- filename: avnet-iotconnect-telemetry-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT Telemetry API
  slug: avnet-iotconnect-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-telemetry-openapi.yml
- filename: avnet-iotconnect-file-openapi.yml
  format: yaml
  label: Avnet /IOTCONNECT File API
  slug: avnet-iotconnect-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/openapi/avnet-iotconnect-file-openapi.yml
auth_types:
- apiKey
- oauth2
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Avnet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avnet secures its APIs with apiKey, oauth2, and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Avnet
provider_slug: avnet
scheme_count: 4
schemes:
- in: header
  name: Ocp-Apim-Subscription-Key
  parameter: Ocp-Apim-Subscription-Key
  surface: Avnet API Portal
  type: apiKey
- flow: clientCredentials
  name: OAuth2 client credentials
  surface: Avnet API Portal
  tokenUrl: https://apigw.avnet.com/external/getToken/oauth2/v2.0/token
  type: oauth2
- in: header
  name: Bearer
  parameter: Authorization
  surface: /IOTCONNECT
  type: apiKey
- in: header
  name: solution-key
  parameter: solution-key
  surface: /IOTCONNECT (login only)
  type: apiKey
slug: avnet-authentication
source_filename: avnet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: >-\n  Avnet API Portal How-To (https://apiportal.avnet.com/help/HowTo) and FAQ (https://apiportal.avnet.com/help/FAQ),\n  the /IOTCONNECT Authenticate API Swagger (https://auth.iotconnect.io/api/v2/swagger-json, saved to\n  openapi/avnet-iotconnect-auth-openapi.yml) and the securityDefinitions shared by all eight /IOTCONNECT module specs,\n  plus the iotc-python-rest-api README (https://github.com/avnet-iotconnect/iotc-python-rest-api).\ndocs: https://apiportal.avnet.com/help/HowTo\nsummary:\n  types: [apiKey, oauth2, http]\n  api_key_in: [header, query]\n  note: >-\n    Two unrelated auth systems. The Avnet API Portal (procurement) layers an Azure API Management subscription key on top\n    of an Entra ID OAuth 2.0 client-credentials bearer token. /IOTCONNECT issues its own JWT from a username/password\n    login that also carries a per-tenant solution key in a header.\nsurfaces:\n  - surface: Avnet API Portal (procurement\
  \ APIs, gateway apigw.avnet.com)\n    schemes:\n      - name: Ocp-Apim-Subscription-Key\n        type: apiKey\n        in: header\n        parameter: Ocp-Apim-Subscription-Key\n        alternate: {in: query, parameter: subscription-key}\n        description: >-\n          Mandatory on every call. A subscription key is scoped to ONE API Product; a second product needs a second key.\n          Keys are issued only after an Avnet API owner approves the subscription request, and each subscription carries a\n          primary/secondary key pair so one can be regenerated while the other stays live. Avnet recommends renewing every\n          6 months.\n      - name: OAuth2 client credentials\n        type: oauth2\n        flow: clientCredentials\n        tokenUrl: https://apigw.avnet.com/external/getToken/oauth2/v2.0/token\n        description: >-\n          grant_type=client_credentials with the client_id, client_secret and scope shown on the portal Profile page after\n          approval (none\
  \ of the three is published). The token endpoint proxies Microsoft Entra ID — an anonymous POST\n          returns AADSTS7000216 invalid_client. The access token is sent as Authorization: Bearer <token>. Client secrets\n          expire and must be renewed every 6 months; at most 2 active secrets per client; a Developer Utility endpoint\n          POST https://apigw.avnet.com/external/clientsecret/{client_id} (bearer-authenticated) rotates a secret programmatically.\n    probes:\n      - url: https://apigw.avnet.com/external/getToken/oauth2/v2.0/token\n        method: POST\n        status: 401\n        body: AADSTS7000216 invalid_client (client_assertion, client_secret or request required)\n        checked: '2026-09-18'\n  - surface: /IOTCONNECT REST API (eight modules on *.iotconnect.io)\n    schemes:\n      - name: Bearer\n        type: apiKey\n        in: header\n        parameter: Authorization\n        description: >-\n          Declared as an apiKey scheme named Bearer in every module's\
  \ securityDefinitions (\"Please enter JWT with Bearer\n          into field\"); applied globally (security: [{Bearer: []}]). The JWT comes from POST /api/v2/Auth/login on\n          auth.iotconnect.io, which additionally requires a solution-key header (the tenant's Solution Key, obtained through\n          an /IOTCONNECT support ticket). GET /api/v2/Auth/basic-token, POST /api/v2/Auth/refresh-token, GET\n          /api/v2/Auth/verify-token and POST /api/v2/Auth/m-login complete the flow. The first-party REST client stores the\n          token locally, treats it as valid for 24 hours and refreshes it on use after one hour.\n        sources:\n          - openapi/avnet-iotconnect-auth-openapi.yml\n          - openapi/avnet-iotconnect-device-openapi.yml\n          - openapi/avnet-iotconnect-event-openapi.yml\n          - openapi/avnet-iotconnect-file-openapi.yml\n          - openapi/avnet-iotconnect-firmware-openapi.yml\n          - openapi/avnet-iotconnect-master-openapi.yml\n          -\
  \ openapi/avnet-iotconnect-telemetry-openapi.yml\n          - openapi/avnet-iotconnect-user-openapi.yml\n      - name: solution-key\n        type: apiKey\n        in: header\n        parameter: solution-key\n        description: Required on the login and mobile-login operations only (openapi/avnet-iotconnect-auth-openapi.yml).\nschemes:\n- name: Ocp-Apim-Subscription-Key\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  surface: Avnet API Portal\n- name: OAuth2 client credentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://apigw.avnet.com/external/getToken/oauth2/v2.0/token\n  surface: Avnet API Portal\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  surface: /IOTCONNECT\n- name: solution-key\n  type: apiKey\n  in: header\n  parameter: solution-key\n  surface: /IOTCONNECT (login only)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avnet/refs/heads/main/authentication/avnet-authentication.yml
summary_line: apiKey/oauth2/http · 4 schemes
tags:
- Fortune 500
- Electronics
- Components
- Supply Chain
- IoT
- Manufacturing
- Distribution
- Procurement
- Device Management
- Firmware
---
