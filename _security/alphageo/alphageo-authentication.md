---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Alphageo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alphageo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alphageo
provider_slug: alphageo
scheme_count: 1
schemes:
- description: 'Access-token authentication. The account access token is passed verbatim as the value of the HTTP Authorization header (no "Bearer" prefix): `Authorization: <your_access_token>`. Tokens are obtained from the AlphaGeo dashboard (upper-right "API" menu) and require an Enterprise subscription and adequate in-app permissions. AlphaGeo recommends routinely refreshing the token as a security measure.'
  in: header
  name: AuthorizationToken
  parameter_name: Authorization
  sources:
  - https://docs.alphageo.ai/for-developers/alphageo-data-api
  type: apiKey
slug: alphageo-authentication
source_filename: alphageo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.alphageo.ai/for-developers/alphageo-data-api\ndocs: https://docs.alphageo.ai/for-developers/alphageo-data-api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: AuthorizationToken\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  description: >-\n    Access-token authentication. The account access token is passed verbatim as the value of\n    the HTTP Authorization header (no \"Bearer\" prefix): `Authorization: <your_access_token>`.\n    Tokens are obtained from the AlphaGeo dashboard (upper-right \"API\" menu) and require an\n    Enterprise subscription and adequate in-app permissions. AlphaGeo recommends routinely\n    refreshing the token as a security measure.\n  sources:\n  - https://docs.alphageo.ai/for-developers/alphageo-data-api\nnotes:\n  - Token issuance is gated behind an Enterprise subscription.\n  - No OAuth2/OIDC or scope surface is documented\
  \ for the public Data API; a single opaque account token authorizes all endpoints.\n  - Token can be refreshed/rotated from the dashboard.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphageo/refs/heads/main/authentication/alphageo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Climate
- Climate Risk
- Geospatial
- Analytics
- Risk
- Real Estate
- ESG
- Data
- Machine Learning
---
