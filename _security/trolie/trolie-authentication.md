---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trolie-forecasting-api-openapi.yml
  format: yaml
  label: TROLIE Forecasting API
  slug: trolie-forecasting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-forecasting-api-openapi.yml
- filename: trolie-monitoring-sets-api-openapi.yml
  format: yaml
  label: TROLIE Monitoring Sets API
  slug: trolie-monitoring-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-monitoring-sets-api-openapi.yml
- filename: trolie-seasonal-api-openapi.yml
  format: yaml
  label: TROLIE Seasonal API
  slug: trolie-seasonal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-seasonal-api-openapi.yml
- filename: trolie-seasonal-overrides-api-openapi.yml
  format: yaml
  label: TROLIE Seasonal Overrides API
  slug: trolie-seasonal-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-seasonal-overrides-api-openapi.yml
- filename: trolie-temporary-aar-exceptions-api-openapi.yml
  format: yaml
  label: TROLIE Temporary AAR Exceptions API
  slug: trolie-temporary-aar-exceptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-temporary-aar-exceptions-api-openapi.yml
- filename: trolie-realtime-api-openapi.yml
  format: yaml
  label: TROLIE Realtime API
  slug: trolie-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-realtime-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Trolie Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: TROLIE secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: TROLIE
provider_slug: trolie
scheme_count: 1
schemes:
- description: Support RFC8725 JWT tokens.
  flows:
  - flow: clientCredentials
    scopes: 15
    tokenUrl: https://no-server/oauth2
  name: oauth2-primary-flow
  sources:
  - openapi/trolie-openapi.yml
  type: oauth2
slug: trolie-authentication
source_filename: trolie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://github.com/trolie/java-client-sdk\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2-primary-flow\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://no-server/oauth2\n    scopes: 15\n  description: Support RFC8725 JWT tokens.\n  sources:\n  - openapi/trolie-openapi.yml\ndocs: https://trolie.energy/spec-1.0\ndocs_additional:\n- https://github.com/trolie/java-client-sdk#connecting-to-spp-trolie-spp-two-factor-authentication\nnotes:\n- The spec tokenUrl is the placeholder https://no-server/oauth2; each implementing\n  RC/TP operates its own authorization server.\n- 'Implementation-specific: the Java Client SDK README documents built-in support\n  for SPP (Southwest Power Pool) Two-Factor Authentication, which requires signing\n  every outbound request with a custom X-SPP-API-Token header using HTTP request metadata\n  (path, timestamp, nonce, and\
  \ screen name) signed with an HMAC-SHA512 key, per SPP\n  TFA Technical Specifications v1.4.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/authentication/trolie-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Energy
- Electric Grid
- Transmission
- Open Standards
- OpenAPI
- LF Energy
- Open Source
---
