---
api_key_in: []
api_specs:
- filename: campaigns-api-openapi.yaml
  format: yaml
  label: MediaMath Campaigns V2.0 API
  slug: mediamath-campaigns-v20-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediamath/refs/heads/main/openapi/campaigns-api-openapi.yaml
- filename: reporting-api-openapi.yaml
  format: yaml
  label: MediaMath Reporting API V2
  slug: mediamath-reporting-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediamath/refs/heads/main/openapi/reporting-api-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Mediamath Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MediaMath secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MediaMath
provider_slug: mediamath
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://auth.mediamath.com/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://auth.mediamath.com/oauth/token
  name: Auth0
  sources:
  - openapi/campaigns-api-openapi.yaml
  - openapi/reporting-api-openapi.yaml
  type: oauth2
slug: mediamath-authentication
source_filename: mediamath-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/campaigns-api-openapi.yaml, openapi/reporting-api-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: Auth0\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.mediamath.com/authorize\n    tokenUrl: https://auth.mediamath.com/oauth/token\n    scopes: 2\n  sources:\n  - openapi/campaigns-api-openapi.yaml\n  - openapi/reporting-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mediamath/refs/heads/main/authentication/mediamath-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Programmatic Advertising
- DSP
- Demand-Side Platform
- Campaign Management
- Ad Tech
- Bidding
- Audience Segments
- Creative Management
- Reporting
- Analytics
---
