---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Venzee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Venzee secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Venzee
provider_slug: venzee
scheme_count: 1
schemes:
- description: 'All requests authenticate with a Bearer token supplied in the Authorization header ("Authorization: Bearer {token}"). API tokens are issued and rotated by the tenant''s Jasper PIM account representative; administrator-level access or higher is required to generate a token. Token rotation takes effect immediately and a rotated/invalid token returns 401 Unauthorized.'
  format: Bearer {token}
  header_name: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://apidocs.jasperpim.com/
  type: http
slug: venzee-authentication
source_filename: venzee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://apidocs.jasperpim.com/\ndocs: https://apidocs.jasperpim.com/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    All requests authenticate with a Bearer token supplied in the Authorization\n    header (\"Authorization: Bearer {token}\"). API tokens are issued and rotated\n    by the tenant's Jasper PIM account representative; administrator-level access\n    or higher is required to generate a token. Token rotation takes effect\n    immediately and a rotated/invalid token returns 401 Unauthorized.\n  in: header\n  header_name: Authorization\n  format: \"Bearer {token}\"\n  sources: [https://apidocs.jasperpim.com/]\nnotes:\n- Tokens are provisioned out-of-band by an account representative; there is no\n  self-service OAuth authorization or token endpoint documented.\n- The API base URL is tenant-scoped\
  \ (https://{hash}.{region}.jasperpim.com/api/v1),\n  so the token is bound to a specific PIM tenant and region (corsair or ans).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venzee/refs/heads/main/authentication/venzee-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Product Information Management
- PIM
- Ecommerce
- Product Data Syndication
- Retail
- Catalog Management
- API
---
