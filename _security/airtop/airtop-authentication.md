---
api_key_in: []
api_specs:
- filename: airtop-ai-query-api-openapi.yml
  format: yaml
  label: Airtop AI Query API
  slug: airtop-ai-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-ai-query-api-openapi.yml
- filename: airtop-page-interaction-api-openapi.yml
  format: yaml
  label: Airtop Page Interaction API
  slug: airtop-page-interaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-page-interaction-api-openapi.yml
- filename: airtop-profiles-api-openapi.yml
  format: yaml
  label: Airtop Profiles API
  slug: airtop-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-profiles-api-openapi.yml
- filename: airtop-screenshots-api-openapi.yml
  format: yaml
  label: Airtop Screenshots API
  slug: airtop-screenshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-screenshots-api-openapi.yml
- filename: airtop-sessions-api-openapi.yml
  format: yaml
  label: Airtop Sessions API
  slug: airtop-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-sessions-api-openapi.yml
- filename: airtop-windows-api-openapi.yml
  format: yaml
  label: Airtop Windows API
  slug: airtop-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/openapi/airtop-windows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Airtop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airtop secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Airtop
provider_slug: airtop
scheme_count: 1
schemes:
- description: 'Airtop API key supplied as a Bearer token in the Authorization header: `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/airtop-openapi.yml
  type: http
slug: airtop-authentication
source_filename: airtop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airtop-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Airtop API key supplied as a Bearer token in the Authorization header: `Authorization:\n    Bearer [example key]`.'\n  sources:\n  - openapi/airtop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airtop/refs/heads/main/authentication/airtop-authentication.yml
summary_line: http · 1 scheme
tags:
- Browser Automation
- AI Agents
- Cloud Browser
- Web Scraping
- Headless Chrome
---
