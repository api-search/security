---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: phantombuster-agent-api-openapi.yml
  format: yaml
  label: Phantombuster Agent API
  slug: phantombuster-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-agent-api-openapi.yml
- filename: phantombuster-agents-api-openapi.yml
  format: yaml
  label: Phantombuster Agents API
  slug: phantombuster-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-agents-api-openapi.yml
- filename: phantombuster-ai-api-openapi.yml
  format: yaml
  label: Phantombuster AI API
  slug: phantombuster-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-ai-api-openapi.yml
- filename: phantombuster-branches-api-openapi.yml
  format: yaml
  label: Phantombuster Branches API
  slug: phantombuster-branches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-branches-api-openapi.yml
- filename: phantombuster-brightdata-api-openapi.yml
  format: yaml
  label: Phantombuster Brightdata API
  slug: phantombuster-brightdata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-brightdata-api-openapi.yml
- filename: phantombuster-buyerspersonas-api-openapi.yml
  format: yaml
  label: Phantombuster Buyers Personas API
  slug: phantombuster-buyerspersonas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-buyerspersonas-api-openapi.yml
- filename: phantombuster-captcha-api-openapi.yml
  format: yaml
  label: Phantombuster Captcha API
  slug: phantombuster-captcha-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-captcha-api-openapi.yml
- filename: phantombuster-containers-api-openapi.yml
  format: yaml
  label: Phantombuster Containers API
  slug: phantombuster-containers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-containers-api-openapi.yml
- filename: phantombuster-icps-api-openapi.yml
  format: yaml
  label: Phantombuster Icps API
  slug: phantombuster-icps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-icps-api-openapi.yml
- filename: phantombuster-identities-api-openapi.yml
  format: yaml
  label: Phantombuster Identities API
  slug: phantombuster-identities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-identities-api-openapi.yml
- filename: phantombuster-location-api-openapi.yml
  format: yaml
  label: Phantombuster Location API
  slug: phantombuster-location-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-location-api-openapi.yml
- filename: phantombuster-org-storage-api-openapi.yml
  format: yaml
  label: Phantombuster Org Storage API
  slug: phantombuster-org-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-org-storage-api-openapi.yml
- filename: phantombuster-orgs-api-openapi.yml
  format: yaml
  label: Phantombuster Orgs API
  slug: phantombuster-orgs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-orgs-api-openapi.yml
- filename: phantombuster-scoring-api-openapi.yml
  format: yaml
  label: Phantombuster Scoring API
  slug: phantombuster-scoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-scoring-api-openapi.yml
- filename: phantombuster-script-api-openapi.yml
  format: yaml
  label: Phantombuster Script API
  slug: phantombuster-script-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-script-api-openapi.yml
- filename: phantombuster-scripts-api-openapi.yml
  format: yaml
  label: Phantombuster Scripts API
  slug: phantombuster-scripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-scripts-api-openapi.yml
- filename: phantombuster-user-api-openapi.yml
  format: yaml
  label: Phantombuster User API
  slug: phantombuster-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-user-api-openapi.yml
- filename: phantombuster-users-api-openapi.yml
  format: yaml
  label: Phantombuster Users API
  slug: phantombuster-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/phantombuster/openapi/phantombuster-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Phantombuster Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phantombuster secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Phantombuster
provider_slug: phantombuster
scheme_count: 2
schemes:
- in: header
  name: internalApiKey
  parameter: X-Phantombuster-Key-1
  sources:
  - openapi/phantombuster-api-v1-api-openapi.yml
  type: apiKey
- in: header
  name: apiKeyAuth
  parameter: X-Phantombuster-Key
  sources:
  - openapi/phantombuster-api-v2-api-openapi.yml
  type: apiKey
slug: phantombuster-authentication
source_filename: phantombuster-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/phantombuster-api-v1-api-openapi.yml, openapi/phantombuster-api-v2-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: internalApiKey\n  type: apiKey\n  in: header\n  parameter: X-Phantombuster-Key-1\n  sources:\n  - openapi/phantombuster-api-v1-api-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Phantombuster-Key\n  sources:\n  - openapi/phantombuster-api-v2-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/phantombuster/authentication/phantombuster-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Automation
- Sales
- Lead Generation
- Web Scraping
- Data Enrichment
---
