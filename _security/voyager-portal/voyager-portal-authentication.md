---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Voyager Portal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voyager Portal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Voyager Portal
provider_slug: voyager-portal
scheme_count: 1
schemes:
- base_urls:
  - environment: production
    url: https://kong.voyagerportal.com/api
  - environment: staging
    url: https://kong.staging.voyagerportal.com/api
  bearerFormat: JWT
  name: VoyagerBearerToken
  scheme: bearer
  sources:
  - https://gitlab.com/voyager-portal/voyager-public-api/-/wikis/Authentication
  token_endpoints:
  - environment: production
    url: https://kong.voyagerportal.com/auth/api/token
  - environment: staging
    url: https://kong.staging.voyagerportal.com/auth/api/token
  token_request:
    method: POST
    params:
    - description: Client identifier issued by the Voyager team
      name: client_id
    - description: Voyager app login email
      name: email
    - description: Voyager app login password
      name: password
  type: http
  usage:
    additional_headers:
    - description: Email of the user making the request
      name: usr-email
    header: 'Authorization: Bearer [IdToken]'
slug: voyager-portal-authentication
source_filename: voyager-portal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://gitlab.com/voyager-portal/voyager-public-api/-/wikis/Authentication\ndocs: https://gitlab.com/voyager-portal/voyager-public-api/-/wikis/Authentication\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  notes: Token-based bearer authentication. A POST to the token endpoint with client_id,\n    email, and password returns an IdToken (JWT) that is passed as a Bearer token\n    in the Authorization header. The client_id is issued by the Voyager team. Requests\n    also carry a usr-email header identifying the calling user.\nschemes:\n- name: VoyagerBearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  token_endpoints:\n  - environment: production\n    url: https://kong.voyagerportal.com/auth/api/token\n  - environment: staging\n    url: https://kong.staging.voyagerportal.com/auth/api/token\n  token_request:\n    method: POST\n    params:\n    - name: client_id\n      description: Client\
  \ identifier issued by the Voyager team\n    - name: email\n      description: Voyager app login email\n    - name: password\n      description: Voyager app login password\n  usage:\n    header: 'Authorization: Bearer [IdToken]'\n    additional_headers:\n    - name: usr-email\n      description: Email of the user making the request\n  base_urls:\n  - environment: production\n    url: https://kong.voyagerportal.com/api\n  - environment: staging\n    url: https://kong.staging.voyagerportal.com/api\n  sources:\n  - https://gitlab.com/voyager-portal/voyager-public-api/-/wikis/Authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyager-portal/refs/heads/main/authentication/voyager-portal-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Maritime
- Shipping
- Logistics
- Demurrage
- Laytime
- Voyages
- Workflows
- Bulk Commodities
---
