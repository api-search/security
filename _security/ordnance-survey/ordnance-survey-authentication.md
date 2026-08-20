---
api_key_in:
- header
- query
api_specs:
- filename: ordnance-survey-ngd-features-openapi.json
  format: json
  label: OS NGD API - Features
  slug: os-ngd-api-features
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-ngd-features-openapi.json
- filename: ordnance-survey-ngd-tiles-openapi.json
  format: json
  label: OS NGD API - Tiles
  slug: os-ngd-api-tiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-ngd-tiles-openapi.json
- filename: ordnance-survey-downloads-openapi.yaml
  format: yaml
  label: OS Downloads API
  slug: os-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-downloads-openapi.yaml
- filename: ordnance-survey-osnet-openapi.yaml
  format: yaml
  label: OS Net API
  slug: os-net-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-osnet-openapi.yaml
- filename: ordnance-survey-places-openapi.json
  format: json
  label: OS Places API
  slug: os-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-places-openapi.json
- filename: ordnance-survey-names-openapi.json
  format: json
  label: OS Names API
  slug: os-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-names-openapi.json
- filename: ordnance-survey-linked-identifiers-openapi.json
  format: json
  label: OS Linked Identifiers API
  slug: os-linked-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-linked-identifiers-openapi.json
- filename: ordnance-survey-features-wfs-openapi.json
  format: json
  label: OS Features API
  slug: os-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-features-wfs-openapi.json
- filename: ordnance-survey-maps-openapi.json
  format: json
  label: OS Maps API
  slug: os-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-maps-openapi.json
- filename: ordnance-survey-vector-tile-openapi.json
  format: json
  label: OS Vector Tile API
  slug: os-vector-tile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-vector-tile-openapi.json
auth_types:
- apiKey
- oauth2
description: 'Three interchangeable credentials across the whole Ordnance Survey estate: the Project API Key as the `key` query parameter, the same key as the `key` request header, or an OAuth 2.0 client-credentials Bearer token. Credentials belong to an OS Data Hub API Project, not to a user, and carry no scopes - entitlement comes from which APIs are attached to the project and which plan the account holds. A 401 is a credential failure; a 403 is a LICENSING failure. The OS Net API spec ships an unresolved OAUTH_TOKEN_URL placeholder as its tokenUrl; the real endpoint is https://api.os.uk/oauth2/token/v1.'
kind: authentication
layout: security
method: searched
name: Ordnance Survey Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Ordnance Survey secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Ordnance Survey
provider_slug: ordnance-survey
scheme_count: 3
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.os.uk/oauth2/token/v1
  name: OAuth2
  sources:
  - openapi/ordnance-survey-downloads-openapi.yaml
  - openapi/ordnance-survey-linked-identifiers-openapi.json
  - openapi/ordnance-survey-ngd-features-openapi.json
  - openapi/ordnance-survey-ngd-tiles-openapi.json
  - openapi/ordnance-survey-osnet-openapi.yaml
  type: oauth2
- in: query
  name: APIKeyQuery
  parameter: key
  sources:
  - openapi/ordnance-survey-downloads-openapi.yaml
  - openapi/ordnance-survey-features-wfs-openapi.json
  - openapi/ordnance-survey-linked-identifiers-openapi.json
  - openapi/ordnance-survey-maps-openapi.json
  - openapi/ordnance-survey-names-openapi.json
  - openapi/ordnance-survey-ngd-features-openapi.json
  - openapi/ordnance-survey-ngd-tiles-openapi.json
  - openapi/ordnance-survey-osnet-openapi.yaml
  - openapi/ordnance-survey-places-openapi.json
  - openapi/ordnance-survey-vector-tile-openapi.json
  type: apiKey
- in: header
  name: APIKeyHeader
  parameter: key
  sources:
  - openapi/ordnance-survey-downloads-openapi.yaml
  - openapi/ordnance-survey-ngd-features-openapi.json
  - openapi/ordnance-survey-ngd-tiles-openapi.json
  - openapi/ordnance-survey-osnet-openapi.yaml
  type: apiKey
slug: ordnance-survey-authentication
source_filename: ordnance-survey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/ordnance-survey-downloads-openapi.yaml, openapi/ordnance-survey-features-wfs-openapi.json,\n  openapi/ordnance-survey-linked-identifiers-openapi.json, openapi/ordnance-survey-maps-openapi.json,\n  openapi/ordnance-survey-names-openapi.json, openapi/ordnance-survey-ngd-features-openapi.json,\n  openapi/ordnance-survey-ngd-tiles-openapi.json, openapi/ordnance-survey-osnet-openapi.yaml,\n  openapi/ordnance-survey-places-openapi.json, openapi/ordnance-survey-vector-tile-openapi.json\ndocs: https://docs.os.uk/os-apis/core-concepts/authentication\noauth2_docs: https://docs.os.uk/os-apis/accessing-os-apis/oauth-2-api/technical-specification\ndescription: >-\n  Three interchangeable credentials across the whole Ordnance Survey estate:\n  the Project API Key as the `key` query parameter, the same key as the `key`\n  request header, or an OAuth 2.0 client-credentials Bearer token. Credentials\n  belong to an OS Data Hub API Project,\
  \ not to a user, and carry no scopes -\n  entitlement comes from which APIs are attached to the project and which plan\n  the account holds. A 401 is a credential failure; a 403 is a LICENSING\n  failure. The OS Net API spec ships an unresolved OAUTH_TOKEN_URL placeholder\n  as its tokenUrl; the real endpoint is https://api.os.uk/oauth2/token/v1.\noauth2:\n  token_url: https://api.os.uk/oauth2/token/v1\n  grant_type: client_credentials\n  client_authentication: HTTP Basic - Project API Key as username, Project API Secret as password\n  request_content_type: application/x-www-form-urlencoded\n  response_fields: [access_token, expires_in, issued_at, token_type]\n  documented_expires_in: 299\n  token_type: Bearer\n  usage: 'Authorization: Bearer <accessToken>'\n  scopes_published: false\n  refresh_tokens: false\n  discovery: none - no /.well-known/openid-configuration and no RFC 8414 metadata\napi_key:\n  query_parameter: key\n  header: key\n  scope: OS Data Hub API Project\n  rotation: Keys\
  \ can be regenerated in place from the API project page in the OS Data Hub.\nprovider_guidance:\n  - Keep API keys and tokens secure at all times.\n  - Rotate keys periodically to minimise the risk of unauthorised access.\n  - Regularly check usage patterns of API keys.\n  - Set up alerts for unusual or unauthorised activity.\n  - Use separate API projects so usage can be monitored per project.\nfailure_semantics:\n  401: No credential or an incorrect/expired credential.\n  403: >-\n    Authenticated but not entitled - the API is not in your plan (Premium /\n    Public Sector / PSGA) or has not been added to this API project.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.os.uk/oauth2/token/v1\n    scopes: 0\n  sources:\n  - openapi/ordnance-survey-downloads-openapi.yaml\n  - openapi/ordnance-survey-linked-identifiers-openapi.json\n\
  \  - openapi/ordnance-survey-ngd-features-openapi.json\n  - openapi/ordnance-survey-ngd-tiles-openapi.json\n  - openapi/ordnance-survey-osnet-openapi.yaml\n- name: APIKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/ordnance-survey-downloads-openapi.yaml\n  - openapi/ordnance-survey-features-wfs-openapi.json\n  - openapi/ordnance-survey-linked-identifiers-openapi.json\n  - openapi/ordnance-survey-maps-openapi.json\n  - openapi/ordnance-survey-names-openapi.json\n  - openapi/ordnance-survey-ngd-features-openapi.json\n  - openapi/ordnance-survey-ngd-tiles-openapi.json\n  - openapi/ordnance-survey-osnet-openapi.yaml\n  - openapi/ordnance-survey-places-openapi.json\n  - openapi/ordnance-survey-vector-tile-openapi.json\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: key\n  sources:\n  - openapi/ordnance-survey-downloads-openapi.yaml\n  - openapi/ordnance-survey-ngd-features-openapi.json\n  - openapi/ordnance-survey-ngd-tiles-openapi.json\n \
  \ - openapi/ordnance-survey-osnet-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/authentication/ordnance-survey-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Real-Estate
- United Kingdom
- Land Registry
- Geospatial
- Addressing
- Open Data
- Property Data
- PropTech
- Government
- Mapping
- OGC
- UPRN
- National Mapping
- GNSS
- Vector Tiles
---
