---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: browserbase-contexts-api-openapi.yml
  format: yaml
  label: Browserbase Contexts API
  slug: browserbase-contexts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-contexts-api-openapi.yml
- filename: browserbase-extensions-api-openapi.yml
  format: yaml
  label: Browserbase Extensions API
  slug: browserbase-extensions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-extensions-api-openapi.yml
- filename: browserbase-projects-api-openapi.yml
  format: yaml
  label: Browserbase Projects API
  slug: browserbase-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-projects-api-openapi.yml
- filename: browserbase-sessions-api-openapi.yml
  format: yaml
  label: Browserbase Sessions API
  slug: browserbase-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-sessions-api-openapi.yml
- filename: browserbase-agents-api-openapi.yml
  format: yaml
  label: Browserbase Agents API
  slug: browserbase-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-agents-api-openapi.yml
- filename: browserbase-certificates-api-openapi.yml
  format: yaml
  label: Browserbase Certificates API
  slug: browserbase-certificates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-certificates-api-openapi.yml
- filename: browserbase-downloads-api-openapi.yml
  format: yaml
  label: Browserbase Downloads API
  slug: browserbase-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-downloads-api-openapi.yml
- filename: browserbase-fetch-api-openapi.yml
  format: yaml
  label: Browserbase Fetch API
  slug: browserbase-fetch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-fetch-api-openapi.yml
- filename: browserbase-functions-api-openapi.yml
  format: yaml
  label: Browserbase Functions API
  slug: browserbase-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-functions-api-openapi.yml
- filename: browserbase-search-api-openapi.yml
  format: yaml
  label: Browserbase Search API
  slug: browserbase-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-search-api-openapi.yml
- filename: browserbase-secrets-api-openapi.yml
  format: yaml
  label: Browserbase Secrets API
  slug: browserbase-secrets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-secrets-api-openapi.yml
- filename: browserbase-webhooks-api-openapi.yml
  format: yaml
  label: Browserbase Webhooks API
  slug: browserbase-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserbase/openapi/browserbase-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/browserbase/authentication/browserbase-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Browser Automation
- Browser Infrastructure
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
