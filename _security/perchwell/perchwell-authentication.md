---
api_key_in:
- header
api_specs:
- filename: perchwell-json-api-openapi.yml
  format: yaml
  label: Perchwell JSON API
  slug: perchwell-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-json-api-openapi.yml
- filename: perchwell-reso-web-api-openapi.yml
  format: yaml
  label: Perchwell RESO Web API
  slug: perchwell-reso-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/openapi/perchwell-reso-web-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Perchwell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Perchwell secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Perchwell
provider_slug: perchwell
scheme_count: 3
schemes:
- description: JSON API simple token authentication (raw token in the Authorization header).
  in: header
  name: tokenAuth
  parameter_name: Authorization
  sources:
  - openapi/perchwell-json-api-openapi.yml
  type: apiKey
- description: RESO Web API token authentication (Authorization Bearer header).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/perchwell-reso-web-api-openapi.yml
  type: http
- description: RETS 1.7 server token authentication (Authorization header on Login, Search, Logout, and GetMetadata transactions at http://rets.perchwell.com:6103).
  in: header
  name: retsToken
  parameter_name: Authorization
  sources:
  - https://docs.perchwell.com/#/rets_getting_started
  type: apiKey
slug: perchwell-authentication
source_filename: perchwell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.perchwell.com/#/reso_getting_started\ndocs: https://docs.perchwell.com\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    All three Perchwell APIs use simple token authentication via the\n    Authorization header. The JSON API sends the raw token\n    (Authorization: {token}); the RESO Web API uses a Bearer token\n    (Authorization: Bearer {token}); the RETS API sends the token in the\n    Authorization header on Login/Search/GetMetadata transactions. There is no\n    OAuth 2.0 authorization server, so there is no scope surface. Credentials\n    are issued by Perchwell support (support@perchwell.com).\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  description: JSON API simple token authentication (raw token in the Authorization header).\n  sources: [openapi/perchwell-json-api-openapi.yml]\n- name: bearerAuth\n  type:\
  \ http\n  scheme: bearer\n  description: RESO Web API token authentication (Authorization Bearer header).\n  sources: [openapi/perchwell-reso-web-api-openapi.yml]\n- name: retsToken\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  description: >-\n    RETS 1.7 server token authentication (Authorization header on Login, Search,\n    Logout, and GetMetadata transactions at http://rets.perchwell.com:6103).\n  sources: [https://docs.perchwell.com/#/rets_getting_started]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perchwell/refs/heads/main/authentication/perchwell-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Real Estate
- MLS
- Listings
- Property Data
- RESO
- RETS
- OData
- Real Estate Data
---
