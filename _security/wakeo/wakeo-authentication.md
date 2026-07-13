---
api_key_in: []
api_specs:
- filename: wakeo-openapi.yml
  format: yaml
  label: Wakeo Shipments API
  slug: wakeo-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakeo/refs/heads/main/openapi/wakeo-openapi.yml
- filename: wakeo-openapi.yml
  format: yaml
  label: Wakeo Tracking API
  slug: wakeo-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakeo/refs/heads/main/openapi/wakeo-openapi.yml
- filename: wakeo-openapi.yml
  format: yaml
  label: Wakeo Webhooks API
  slug: wakeo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakeo/refs/heads/main/openapi/wakeo-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: documented
name: Wakeo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wakeo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wakeo
provider_slug: wakeo
scheme_count: 1
schemes:
- confirmed: true
  description: 'All Wakeo API endpoints are secured with an OAuth 2.0 access token. Every request must include the Authorization header with a valid bearer token: `Authorization: Bearer <ACCESS_TOKEN>`. This is confirmed from Wakeo''s published documentation and by live probe of https://api.wakeo.co, which is fronted by AWS API Gateway and returns HTTP 403 ForbiddenException for unauthenticated requests. The token endpoint, grant type, and scopes are not publicly documented (the reference is password-protected) and are modeled in the OpenAPI; obtain credentials from Wakeo Customer Success or support@wakeo.co.'
  name: oauth2
  scheme: bearer
  sources:
  - https://docs.wakeo.co/docs/getting-started
  - https://api.wakeo.co
  type: oauth2
slug: wakeo-authentication
source_filename: wakeo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://docs.wakeo.co/docs/getting-started\nsummary:\n  types:\n  - oauth2\nschemes:\n- name: oauth2\n  type: oauth2\n  scheme: bearer\n  description: >-\n    All Wakeo API endpoints are secured with an OAuth 2.0 access token. Every\n    request must include the Authorization header with a valid bearer token:\n    `Authorization: Bearer <ACCESS_TOKEN>`. This is confirmed from Wakeo's\n    published documentation and by live probe of https://api.wakeo.co, which is\n    fronted by AWS API Gateway and returns HTTP 403 ForbiddenException for\n    unauthenticated requests. The token endpoint, grant type, and scopes are not\n    publicly documented (the reference is password-protected) and are modeled in\n    the OpenAPI; obtain credentials from Wakeo Customer Success or\n    support@wakeo.co.\n  confirmed: true\n  sources:\n  - https://docs.wakeo.co/docs/getting-started\n  - https://api.wakeo.co\nnotes: >-\n  Wakeo is an enterprise,\
  \ customer-provisioned platform. Credentials are issued\n  to customers - there is no self-serve API key signup. The OAuth token URL and\n  grant type shown in openapi/wakeo-openapi.yml are modeled and must be\n  reconciled against the password-protected reference.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wakeo/refs/heads/main/authentication/wakeo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Supply Chain
- Transportation Visibility
- Real-Time Visibility
- Multimodal
- Logistics
- Shipment Tracking
- ETA
- Freight
- Supply Chain Visibility
- SaaS
---
