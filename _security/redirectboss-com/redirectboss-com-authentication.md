---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: redirectboss-com-analytics-api-openapi.yml
  format: yaml
  label: RedirectBoss Analytics API
  slug: redirectboss-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redirectboss-com/openapi/redirectboss-com-analytics-api-openapi.yml
- filename: redirectboss-com-hosts-api-openapi.yml
  format: yaml
  label: RedirectBoss Hosts API
  slug: redirectboss-com-hosts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redirectboss-com/openapi/redirectboss-com-hosts-api-openapi.yml
- filename: redirectboss-com-redirects-api-openapi.yml
  format: yaml
  label: RedirectBoss Redirects API
  slug: redirectboss-com-redirects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redirectboss-com/openapi/redirectboss-com-redirects-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: RedirectBoss Authentication
name_suffix: Authentication
oauth_flows: []
overview: RedirectBoss secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RedirectBoss
provider_slug: redirectboss-com
scheme_count: 1
schemes:
- description: 'API key from the RedirectBoss dashboard. Example: "X-Api-Key: rb_live_<key>"'
  in: header
  name: apiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/redirectboss-com-openapi.json
  type: apiKey
slug: redirectboss-com-authentication
source_filename: redirectboss-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-23'\nmethod: derived\nsource: openapi/redirectboss-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: 'API key from the RedirectBoss dashboard. Example: \"X-Api-Key: rb_live_<key>\"'\n  sources:\n  - openapi/redirectboss-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/redirectboss-com/authentication/redirectboss-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Redirects
- Domain Management
- API
- MCP
- SaaS
---
