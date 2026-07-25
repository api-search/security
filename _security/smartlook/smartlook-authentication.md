---
api_key_in: []
api_specs:
- filename: smartlook-events-api-openapi.yml
  format: yaml
  label: Smartlook Events API
  slug: smartlook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlook/refs/heads/main/openapi/smartlook-events-api-openapi.yml
- filename: smartlook-funnels-api-openapi.yml
  format: yaml
  label: Smartlook Funnels API
  slug: smartlook-funnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlook/refs/heads/main/openapi/smartlook-funnels-api-openapi.yml
- filename: smartlook-mappingfiles-api-openapi.yml
  format: yaml
  label: Smartlook mappingFiles API
  slug: smartlook-mappingfiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlook/refs/heads/main/openapi/smartlook-mappingfiles-api-openapi.yml
- filename: smartlook-sessions-api-openapi.yml
  format: yaml
  label: Smartlook Sessions API
  slug: smartlook-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlook/refs/heads/main/openapi/smartlook-sessions-api-openapi.yml
- filename: smartlook-system-api-openapi.yml
  format: yaml
  label: Smartlook System API
  slug: smartlook-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlook/refs/heads/main/openapi/smartlook-system-api-openapi.yml
- filename: smartlook-visitors-api-openapi.yml
  format: yaml
  label: Smartlook Visitors API
  slug: smartlook-visitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlook/refs/heads/main/openapi/smartlook-visitors-api-openapi.yml
- filename: smartlook-webhooks-api-openapi.yml
  format: yaml
  label: Smartlook Webhooks API
  slug: smartlook-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartlook/refs/heads/main/openapi/smartlook-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Smartlook Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smartlook secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smartlook
provider_slug: smartlook
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/smartlook-rest-api-openapi.yml
  type: http
slug: smartlook-authentication
source_filename: smartlook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smartlook-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/smartlook-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartlook/refs/heads/main/authentication/smartlook-authentication.yml
summary_line: http · 1 scheme
tags:
- Product Analytics
- Session Recording
- Heatmaps
- Funnels
- User Behavior
- Event Tracking
- Visitor Analytics
- Digital Experience
---
