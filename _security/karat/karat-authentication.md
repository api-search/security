---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Karat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Karat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Karat
provider_slug: karat
scheme_count: 1
schemes:
- description: 'All Karat GraphQL API requests authenticate with a per-tenant API token supplied in the HTTP Authorization header as `Authorization: Bearer <token>`. Requests are scoped to the customer''s own subdomain/environment. Tokens are issued per customer account.'
  format: Bearer <token>
  header: Authorization
  location: header
  name: bearerAuth
  scheme: bearer
  sources:
  - graphql/karat-operations.graphql
  - https://github.com/karat/api-sdk/blob/main/src/karatclient/karatclient.py
  type: http
slug: karat-authentication
source_filename: karat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/karat/api-docs (Postman collection) + https://github.com/karat/api-sdk (KaratClient transport)\ndocs: https://karat.slab.com/posts/karat-api-documentation-dezzam7y\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    All Karat GraphQL API requests authenticate with a per-tenant API token supplied in\n    the HTTP Authorization header as `Authorization: Bearer <token>`. Requests are scoped\n    to the customer's own subdomain/environment. Tokens are issued per customer account.\n  location: header\n  header: Authorization\n  format: 'Bearer <token>'\n  sources:\n  - graphql/karat-operations.graphql\n  - https://github.com/karat/api-sdk/blob/main/src/karatclient/karatclient.py\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karat/refs/heads/main/authentication/karat-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Technical Interviewing
- Hiring
- Recruiting
- Talent Assessment
- Engineering
- GraphQL
- API
---
