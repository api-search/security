---
api_key_in:
- header
api_specs:
- filename: browserbase-contexts-api-openapi.yml
  format: yaml
  label: Browserbase Contexts API
  slug: browserbase-contexts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserbase/refs/heads/main/openapi/browserbase-contexts-api-openapi.yml
- filename: browserbase-extensions-api-openapi.yml
  format: yaml
  label: Browserbase Extensions API
  slug: browserbase-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserbase/refs/heads/main/openapi/browserbase-extensions-api-openapi.yml
- filename: browserbase-projects-api-openapi.yml
  format: yaml
  label: Browserbase Projects API
  slug: browserbase-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserbase/refs/heads/main/openapi/browserbase-projects-api-openapi.yml
- filename: browserbase-sessions-api-openapi.yml
  format: yaml
  label: Browserbase Sessions API
  slug: browserbase-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserbase/refs/heads/main/openapi/browserbase-sessions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Browserbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Browserbase secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Browserbase
provider_slug: browserbase
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-BB-API-Key
  sources:
  - openapi/browserbase-openapi.yml
  type: apiKey
slug: browserbase-authentication
source_filename: browserbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/browserbase-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-BB-API-Key\n  sources:\n  - openapi/browserbase-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/browserbase/refs/heads/main/authentication/browserbase-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Headless Browser
- Browser Infrastructure
- Web Automation
- AI Agents
- Web Scraping
- Stagehand
- Playwright
- Puppeteer
- Web Search
- Web Fetch
- Model Gateway
- MCP
- Session Recording
- Agent Identity
---
