---
api_key_in:
- header
- query
api_specs:
- filename: sentio-ai-api-openapi.yml
  format: yaml
  label: Sentio AI API
  slug: sentio-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-ai-api-openapi.yml
- filename: sentio-alerts-api-openapi.yml
  format: yaml
  label: Sentio Alerts API
  slug: sentio-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-alerts-api-openapi.yml
- filename: sentio-data-api-openapi.yml
  format: yaml
  label: Sentio Data API
  slug: sentio-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-data-api-openapi.yml
- filename: sentio-debug-and-simulation-api-openapi.yml
  format: yaml
  label: Sentio Debug and Simulation API
  slug: sentio-debug-and-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-debug-and-simulation-api-openapi.yml
- filename: sentio-forks-api-openapi.yml
  format: yaml
  label: Sentio Forks API
  slug: sentio-forks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-forks-api-openapi.yml
- filename: sentio-move-api-openapi.yml
  format: yaml
  label: Sentio Move API
  slug: sentio-move-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-move-api-openapi.yml
- filename: sentio-price-api-openapi.yml
  format: yaml
  label: Sentio Price API
  slug: sentio-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-price-api-openapi.yml
- filename: sentio-prices-api-openapi.yml
  format: yaml
  label: Sentio Prices API
  slug: sentio-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-prices-api-openapi.yml
- filename: sentio-processor-api-openapi.yml
  format: yaml
  label: Sentio Processor API
  slug: sentio-processor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-processor-api-openapi.yml
- filename: sentio-processorext-api-openapi.yml
  format: yaml
  label: Sentio ProcessorExt API
  slug: sentio-processorext-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-processorext-api-openapi.yml
- filename: sentio-web-api-openapi.yml
  format: yaml
  label: Sentio Web API
  slug: sentio-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-web-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sentio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sentio secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sentio
provider_slug: sentio
scheme_count: 2
schemes:
- in: header
  name: ApiKeyHeaderAuth
  parameter: api-key
  sources:
  - openapi/sentio-openapi.yml
  type: apiKey
- in: query
  name: ApiKeyQueryAuth
  parameter: api-key
  sources:
  - openapi/sentio-openapi.yml
  type: apiKey
slug: sentio-authentication
source_filename: sentio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sentio-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeaderAuth\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/sentio-openapi.yml\n- name: ApiKeyQueryAuth\n  type: apiKey\n  in: query\n  parameter: api-key\n  sources:\n  - openapi/sentio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/authentication/sentio-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Web3
- Blockchain
- Observability
- Analytics
- Data
- Indexing
- Monitoring
- Developer Tools
- Crypto
- API
---
