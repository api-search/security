---
api_key_in:
- header
api_specs:
- filename: steel-dev-openapi.yml
  format: yaml
  label: Steel Sessions API
  slug: steel-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steel-dev/refs/heads/main/openapi/steel-dev-openapi.yml
- filename: steel-dev-openapi.yml
  format: yaml
  label: Steel Scrape API
  slug: steel-scrape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steel-dev/refs/heads/main/openapi/steel-dev-openapi.yml
- filename: steel-dev-openapi.yml
  format: yaml
  label: Steel Screenshot & PDF API
  slug: steel-screenshot-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steel-dev/refs/heads/main/openapi/steel-dev-openapi.yml
- filename: steel-dev-openapi.yml
  format: yaml
  label: Steel CDP / Browser Connect API
  slug: steel-browser-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steel-dev/refs/heads/main/openapi/steel-dev-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Steel Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Steel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Steel
provider_slug: steel-dev
scheme_count: 1
schemes:
- description: API key issued from app.steel.dev. Pass it in the `Steel-Api-Key` request header. Self-hosted instances may run without auth.
  in: header
  name: SteelApiKey
  parameter: Steel-Api-Key
  sources:
  - openapi/steel-dev-openapi.yml
  type: apiKey
slug: steel-dev-authentication
source_filename: steel-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/steel-dev-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SteelApiKey\n  type: apiKey\n  in: header\n  parameter: Steel-Api-Key\n  description: API key issued from app.steel.dev. Pass it in the `Steel-Api-Key` request header.\n    Self-hosted instances may run without auth.\n  sources:\n  - openapi/steel-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steel-dev/refs/heads/main/authentication/steel-dev-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Browser
- Web Automation
- Scraping
- AI Agents
- Open Source
---
