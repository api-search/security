---
api_key_in: []
api_specs:
- filename: braintrust-openapi.json
  format: json
  label: Braintrust API
  slug: braintrust-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust/refs/heads/main/openapi/braintrust-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Braintrust Authentication
name_suffix: Authentication
oauth_flows: []
overview: Braintrust secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Braintrust
provider_slug: braintrust
scheme_count: 1
schemes:
- bearerFormat: API key or JWT
  description: 'Most Braintrust endpoints are authenticated by providing your API key as a header `Authorization: Bearer [api_key]` to your HTTP request. You can create an API key in the Braintrust [organization settings page](https://www.braintrustdata.com/app/settings?subroute=api-keys).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/braintrust-openapi.json
  type: http
slug: braintrust-authentication
source_filename: braintrust-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/braintrust-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key or JWT\n  description: 'Most Braintrust endpoints are authenticated by providing your API key as a header\n    `Authorization: Bearer [api_key]` to your HTTP request. You can create an API key in the\n    Braintrust [organization settings page](https://www.braintrustdata.com/app/settings?subroute=api-keys).'\n  sources:\n  - openapi/braintrust-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braintrust/refs/heads/main/authentication/braintrust-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- LLM
- Observability
- Evaluation
- Experiments
- Datasets
- Prompts
- Tracing
- Monitoring
- Scoring
- AI Engineering
- Generative AI
---
