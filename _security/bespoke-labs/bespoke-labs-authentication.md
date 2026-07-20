---
api_key_in:
- header
api_specs:
- filename: bespoke-labs-minicheck-openapi-original.json
  format: json
  label: Bespoke MiniCheck (Argus)
  slug: bespoke-minicheck-argus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bespoke-labs/refs/heads/main/openapi/bespoke-labs-minicheck-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bespoke Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bespoke Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bespoke Labs
provider_slug: bespoke-labs
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: api_key
  sources:
  - openapi/bespoke-labs-minicheck-openapi-original.json
  type: apiKey
slug: bespoke-labs-authentication
source_filename: bespoke-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/bespoke-labs-minicheck-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: api_key\n  sources:\n  - openapi/bespoke-labs-minicheck-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bespoke-labs/refs/heads/main/authentication/bespoke-labs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- LLM
- Synthetic Data
- Data Curation
- Fact Checking
- Hallucination Detection
- AI Agents
- Evaluation
---
