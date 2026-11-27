---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lpsignal-app-account-api-openapi.yml
  format: yaml
  label: LPSignal Account API
  slug: lpsignal-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lpsignal-app/openapi/lpsignal-app-account-api-openapi.yml
- filename: lpsignal-app-agents-api-openapi.yml
  format: yaml
  label: LPSignal Agents API
  slug: lpsignal-app-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lpsignal-app/openapi/lpsignal-app-agents-api-openapi.yml
- filename: lpsignal-app-meta-api-openapi.yml
  format: yaml
  label: LPSignal Meta API
  slug: lpsignal-app-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lpsignal-app/openapi/lpsignal-app-meta-api-openapi.yml
- filename: lpsignal-app-pools-api-openapi.yml
  format: yaml
  label: LPSignal Pools API
  slug: lpsignal-app-pools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lpsignal-app/openapi/lpsignal-app-pools-api-openapi.yml
- filename: lpsignal-app-signals-api-openapi.yml
  format: yaml
  label: LPSignal Signals API
  slug: lpsignal-app-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lpsignal-app/openapi/lpsignal-app-signals-api-openapi.yml
- filename: lpsignal-app-smart-lps-api-openapi.yml
  format: yaml
  label: LPSignal smart LPs API
  slug: lpsignal-app-smart-lps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lpsignal-app/openapi/lpsignal-app-smart-lps-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: LPSignal Authentication
name_suffix: Authentication
oauth_flows: []
overview: LPSignal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LPSignal
provider_slug: lpsignal-app
scheme_count: 1
schemes:
- description: 'An LPSignal API key: `Authorization: Bearer lps_…`'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/lpsignal-app-openapi.json
  type: http
slug: lpsignal-app-authentication
source_filename: lpsignal-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/lpsignal-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'An LPSignal API key: `Authorization: Bearer lps_…`'\n  sources:\n  - openapi/lpsignal-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lpsignal-app/authentication/lpsignal-app-authentication.yml
summary_line: http · 1 scheme
tags:
- LP Signals
- Impermanent Loss
---
