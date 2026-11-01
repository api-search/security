---
anonymous_access: false
api_key_in: []
api_specs:
- filename: airtop-profiles-api-openapi.yml
  format: yaml
  label: Airtop Profiles API
  slug: airtop-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-profiles-api-openapi.yml
- filename: airtop-sessions-api-openapi.yml
  format: yaml
  label: Airtop Sessions API
  slug: airtop-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-sessions-api-openapi.yml
- filename: airtop-windows-api-openapi.yml
  format: yaml
  label: Airtop Windows API
  slug: airtop-windows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-windows-api-openapi.yml
- filename: airtop-agent-director-api-openapi.yml
  format: yaml
  label: Airtop Agent Director API
  slug: airtop-agent-director-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-agent-director-api-openapi.yml
- filename: airtop-agent-folders-api-openapi.yml
  format: yaml
  label: Airtop Agent Folders API
  slug: airtop-agent-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-agent-folders-api-openapi.yml
- filename: airtop-agents-api-openapi.yml
  format: yaml
  label: Airtop Agents API
  slug: airtop-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-agents-api-openapi.yml
- filename: airtop-automations-api-openapi.yml
  format: yaml
  label: Airtop Automations API
  slug: airtop-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-automations-api-openapi.yml
- filename: airtop-beta-api-openapi.yml
  format: yaml
  label: Airtop Beta API
  slug: airtop-beta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-beta-api-openapi.yml
- filename: airtop-files-api-openapi.yml
  format: yaml
  label: Airtop Files API
  slug: airtop-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-files-api-openapi.yml
- filename: airtop-gtm-engineer-api-openapi.yml
  format: yaml
  label: Airtop GTM Engineer API
  slug: airtop-gtm-engineer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-gtm-engineer-api-openapi.yml
- filename: airtop-knowledge-base-api-openapi.yml
  format: yaml
  label: Airtop Knowledge Base API
  slug: airtop-knowledge-base-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-knowledge-base-api-openapi.yml
- filename: airtop-requests-api-openapi.yml
  format: yaml
  label: Airtop Requests API
  slug: airtop-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-requests-api-openapi.yml
- filename: airtop-sensitive-values-api-openapi.yml
  format: yaml
  label: Airtop Sensitive Values API
  slug: airtop-sensitive-values-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-sensitive-values-api-openapi.yml
- filename: airtop-services-api-openapi.yml
  format: yaml
  label: Airtop Services API
  slug: airtop-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-services-api-openapi.yml
- filename: airtop-team-vault-api-openapi.yml
  format: yaml
  label: Airtop Team Vault API
  slug: airtop-team-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-team-vault-api-openapi.yml
- filename: airtop-templates-api-openapi.yml
  format: yaml
  label: Airtop Templates API
  slug: airtop-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airtop/openapi/airtop-templates-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/airtop/authentication/airtop-authentication.yml
summary_line: http · 1 scheme
tags:
- Browser Automation
- AI Agents
- Cloud Browser
- Web Scraping
- Headless Chrome
---
