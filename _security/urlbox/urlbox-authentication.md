---
api_key_in: []
api_specs:
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Synchronous Render API
  slug: urlbox-render-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Asynchronous Render API
  slug: urlbox-render-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Render Status API
  slug: urlbox-render-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Render Links API
  slug: urlbox-render-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Webhooks API
  slug: urlbox-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Usage API
  slug: urlbox-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Urlbox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Urlbox secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Urlbox
provider_slug: urlbox
scheme_count: 1
schemes:
- description: Project secret key supplied as a Bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/urlbox-openapi.yml
  type: http
slug: urlbox-authentication
source_filename: urlbox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/urlbox-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Project secret key supplied as a Bearer token in the Authorization header.\n  sources:\n  - openapi/urlbox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/authentication/urlbox-authentication.yml
summary_line: http · 1 scheme
tags:
- Screenshots
- Rendering
- PDF
- Video
- Web Capture
---
