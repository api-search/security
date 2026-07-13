---
api_key_in:
- cookie
api_specs:
- filename: sitefinity-cms-content-api-openapi.yml
  format: yaml
  label: Sitefinity CMS Content API
  slug: content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sitefinity-cms/refs/heads/main/openapi/sitefinity-cms-content-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sitefinity Cms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sitefinity CMS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sitefinity CMS
provider_slug: sitefinity-cms
scheme_count: 1
schemes:
- description: Sitefinity CMS uses ASP.NET forms authentication. Authenticate via the /Sitefinity/Authenticate/SWT endpoint to obtain a token, or use the /api/default/Authenticate endpoint for REST token-based auth.
  in: cookie
  name: cookieAuth
  parameter: .ASPXAUTH
  sources:
  - openapi/sitefinity-cms-content-api-openapi.yml
  type: apiKey
slug: sitefinity-cms-authentication
source_filename: sitefinity-cms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sitefinity-cms-content-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: .ASPXAUTH\n  description: Sitefinity CMS uses ASP.NET forms authentication. Authenticate via the /Sitefinity/Authenticate/SWT\n    endpoint to obtain a token, or use the /api/default/Authenticate endpoint for REST token-based\n    auth.\n  sources:\n  - openapi/sitefinity-cms-content-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sitefinity-cms/refs/heads/main/authentication/sitefinity-cms-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Content Management
- Headless CMS
- .NET
- REST
---
