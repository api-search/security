---
api_key_in: []
api_specs:
- filename: facebook-marketing-openapi.yml
  format: yaml
  label: Facebook Marketing API
  slug: facebook-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-marketing-openapi.yml
- filename: facebook-pages-openapi.yml
  format: yaml
  label: Facebook Pages API
  slug: facebook-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-pages-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Facebook Business Manager Authentication
name_suffix: Authentication
oauth_flows: []
overview: Facebook Business Manager secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Facebook Business Manager
provider_slug: facebook-business-manager
scheme_count: 1
schemes:
- description: OAuth 2.0 access token with ads_management or ads_read permissions. Obtain tokens via the Facebook Login flow.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/facebook-marketing-openapi.yml
  - openapi/facebook-pages-openapi.yml
  type: http
slug: facebook-business-manager-authentication
source_filename: facebook-business-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/facebook-marketing-openapi.yml, openapi/facebook-pages-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token with ads_management or ads_read permissions. Obtain tokens\n    via the Facebook Login flow.\n  sources:\n  - openapi/facebook-marketing-openapi.yml\n  - openapi/facebook-pages-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/authentication/facebook-business-manager-authentication.yml
summary_line: http · 1 scheme
tags:
- Advertising
- Analytics
- Business Management
- Marketing
- Social Media
---
