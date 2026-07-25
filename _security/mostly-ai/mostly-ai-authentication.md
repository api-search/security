---
api_key_in:
- header
api_specs:
- filename: mostly-ai-about-api-openapi.yml
  format: yaml
  label: MOSTLY AI About API
  slug: mostly-ai-about-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mostly-ai/refs/heads/main/openapi/mostly-ai-about-api-openapi.yml
- filename: mostly-ai-computes-api-openapi.yml
  format: yaml
  label: MOSTLY AI Computes API
  slug: mostly-ai-computes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mostly-ai/refs/heads/main/openapi/mostly-ai-computes-api-openapi.yml
- filename: mostly-ai-connectors-api-openapi.yml
  format: yaml
  label: MOSTLY AI Connectors API
  slug: mostly-ai-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mostly-ai/refs/heads/main/openapi/mostly-ai-connectors-api-openapi.yml
- filename: mostly-ai-datasets-api-openapi.yml
  format: yaml
  label: MOSTLY AI Datasets API
  slug: mostly-ai-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mostly-ai/refs/heads/main/openapi/mostly-ai-datasets-api-openapi.yml
- filename: mostly-ai-generators-api-openapi.yml
  format: yaml
  label: MOSTLY AI Generators API
  slug: mostly-ai-generators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mostly-ai/refs/heads/main/openapi/mostly-ai-generators-api-openapi.yml
- filename: mostly-ai-models-api-openapi.yml
  format: yaml
  label: MOSTLY AI Models API
  slug: mostly-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mostly-ai/refs/heads/main/openapi/mostly-ai-models-api-openapi.yml
- filename: mostly-ai-organizations-api-openapi.yml
  format: yaml
  label: MOSTLY AI Organizations API
  slug: mostly-ai-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mostly-ai/refs/heads/main/openapi/mostly-ai-organizations-api-openapi.yml
- filename: mostly-ai-synthetic-datasets-api-openapi.yml
  format: yaml
  label: MOSTLY AI Synthetic Datasets API
  slug: mostly-ai-synthetic-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mostly-ai/refs/heads/main/openapi/mostly-ai-synthetic-datasets-api-openapi.yml
- filename: mostly-ai-synthetic-probes-api-openapi.yml
  format: yaml
  label: MOSTLY AI Synthetic Probes API
  slug: mostly-ai-synthetic-probes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mostly-ai/refs/heads/main/openapi/mostly-ai-synthetic-probes-api-openapi.yml
- filename: mostly-ai-users-api-openapi.yml
  format: yaml
  label: MOSTLY AI Users API
  slug: mostly-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mostly-ai/refs/heads/main/openapi/mostly-ai-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mostly Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: MOSTLY AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MOSTLY AI
provider_slug: mostly-ai
scheme_count: 1
schemes:
- description: API key issued from the user profile in the MOSTLY AI web app.
  in: header
  name: apiKey
  parameter: X-MOSTLY-API-KEY
  sources:
  - openapi/mostly-ai-openapi.yml
  type: apiKey
slug: mostly-ai-authentication
source_filename: mostly-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mostly-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-MOSTLY-API-KEY\n  description: API key issued from the user profile in the MOSTLY AI web app.\n  sources:\n  - openapi/mostly-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mostly-ai/refs/heads/main/authentication/mostly-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Synthetic Data
- Privacy
- Tabular
- Differential Privacy
- Python SDK
- REST
- Apache 2.0
---
