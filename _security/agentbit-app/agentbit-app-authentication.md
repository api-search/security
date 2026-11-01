---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentbit-app-google-ads-account-api-openapi.yml
  format: yaml
  label: agentbit-app Google Ads - Account API
  slug: agentbit-app-google-ads-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbit-app/openapi/agentbit-app-google-ads-account-api-openapi.yml
- filename: agentbit-app-google-ads-audit-api-openapi.yml
  format: yaml
  label: agentbit-app Google Ads - Audit API
  slug: agentbit-app-google-ads-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbit-app/openapi/agentbit-app-google-ads-audit-api-openapi.yml
- filename: agentbit-app-google-ads-query-api-openapi.yml
  format: yaml
  label: agentbit-app Google Ads - Query API
  slug: agentbit-app-google-ads-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbit-app/openapi/agentbit-app-google-ads-query-api-openapi.yml
- filename: agentbit-app-google-ads-read-api-openapi.yml
  format: yaml
  label: agentbit-app Google Ads - Read API
  slug: agentbit-app-google-ads-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbit-app/openapi/agentbit-app-google-ads-read-api-openapi.yml
- filename: agentbit-app-google-ads-write-api-openapi.yml
  format: yaml
  label: agentbit-app Google Ads - Write API
  slug: agentbit-app-google-ads-write-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbit-app/openapi/agentbit-app-google-ads-write-api-openapi.yml
- filename: agentbit-app-meta-ads-audit-api-openapi.yml
  format: yaml
  label: agentbit-app Meta Ads - Audit API
  slug: agentbit-app-meta-ads-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbit-app/openapi/agentbit-app-meta-ads-audit-api-openapi.yml
- filename: agentbit-app-meta-ads-read-api-openapi.yml
  format: yaml
  label: agentbit-app Meta Ads - Read API
  slug: agentbit-app-meta-ads-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbit-app/openapi/agentbit-app-meta-ads-read-api-openapi.yml
- filename: agentbit-app-meta-ads-write-api-openapi.yml
  format: yaml
  label: agentbit-app Meta Ads - Write API
  slug: agentbit-app-meta-ads-write-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbit-app/openapi/agentbit-app-meta-ads-write-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agentbit App Authentication
name_suffix: Authentication
oauth_flows: []
overview: agentbit-app secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: agentbit-app
provider_slug: agentbit-app
scheme_count: 1
schemes:
- description: 'API key from your AdWhiz dashboard (https://www.adwhiz.ai/app/api-keys). Format: aw_live_<hex>'
  name: bearerApiKey
  scheme: bearer
  sources:
  - openapi/agentbit-app-openapi.json
  type: http
slug: agentbit-app-authentication
source_filename: agentbit-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/agentbit-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  description: 'API key from your AdWhiz dashboard (https://www.adwhiz.ai/app/api-keys). Format:\n    aw_live_<hex>'\n  sources:\n  - openapi/agentbit-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/agentbit-app/authentication/agentbit-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Tools
- Pay-per-call
- Data
---
