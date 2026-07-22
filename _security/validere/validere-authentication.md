---
api_key_in:
- header
api_specs:
- filename: validere-carbonhub-openapi-original.json
  format: json
  label: Validere CarbonHub App API
  slug: validere-carbonhub-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validere/refs/heads/main/openapi/validere-carbonhub-openapi-original.json
- filename: validere-dataplatform-source-openapi-original.json
  format: json
  label: Validere Data Platform Source API
  slug: validere-data-platform-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validere/refs/heads/main/openapi/validere-dataplatform-source-openapi-original.json
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Validere Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Validere secures its APIs with oauth2, http, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Validere
provider_slug: validere
scheme_count: 3
schemes:
- flows:
  - audience: https://validere360.com/api
    flow: clientCredentials
    tokenUrl: https://validere.auth0.com/oauth/token
  name: OAuth2ClientCredentials
  sources:
  - https://docs.validere.com/guides/api/authentication
  type: oauth2
- bearerFormat: JWT
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/validere-dataplatform-source-openapi-original.json
  - https://docs.validere.com/guides/api/authentication
  type: http
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/validere-dataplatform-source-openapi-original.json
  type: apiKey
slug: validere-authentication
source_filename: validere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.validere.com/guides/api/authentication\ndocs: https://docs.validere.com/guides/api/authentication\nsummary:\n  types:\n  - oauth2\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nnotes: >-\n  Validere's Public API uses OAuth 2.0 client_credentials against the company's\n  Auth0 tenant. Clients obtain an auth0 client_id/client_secret from Validere's\n  Data Services Consulting team (no self-serve signup), exchange them for a\n  machine JWT at https://validere.auth0.com/oauth/token with audience\n  https://validere360.com/api, and send the JWT as a Bearer token. The\n  documented example token lifetime is expires_in 86400 seconds; caching the\n  token until expiry is recommended. The Data Platform Source API spec\n  additionally declares an X-API-Key header scheme. The CarbonHub App API spec\n  references Staging/Integration/Local security schemes without defining them\n \
  \ in components.securitySchemes.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://validere.auth0.com/oauth/token\n    audience: https://validere360.com/api\n  sources:\n  - https://docs.validere.com/guides/api/authentication\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/validere-dataplatform-source-openapi-original.json\n  - https://docs.validere.com/guides/api/authentication\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/validere-dataplatform-source-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/validere/refs/heads/main/authentication/validere-authentication.yml
summary_line: oauth2/http/apiKey · 3 schemes
tags:
- Company
- Applications
- Energy
- Emissions
- Methane
- Oil And Gas
- Environmental Data
- Measurement
- Carbon Intensity
- EHS
---
