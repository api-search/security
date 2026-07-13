---
api_key_in:
- header
api_specs:
- filename: snorkel-ai-openapi.yml
  format: yaml
  label: Snorkel Flow SDK / Platform
  slug: snorkel-flow-sdk-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snorkel-ai/refs/heads/main/openapi/snorkel-ai-openapi.yml
- filename: snorkel-ai-openapi.yml
  format: yaml
  label: Programmatic Labeling
  slug: programmatic-labeling
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snorkel-ai/refs/heads/main/openapi/snorkel-ai-openapi.yml
- filename: snorkel-ai-openapi.yml
  format: yaml
  label: Evaluation
  slug: evaluation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snorkel-ai/refs/heads/main/openapi/snorkel-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Snorkel Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snorkel AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Snorkel AI
provider_slug: snorkel-ai
scheme_count: 1
schemes:
- description: Snorkel Flow API key supplied to the SDK via SnorkelFlowContext. Keys are per-user and may be rotated by the platform on re-authentication.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/snorkel-ai-openapi.yml
  type: apiKey
slug: snorkel-ai-authentication
source_filename: snorkel-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snorkel-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Snorkel Flow API key supplied to the SDK via SnorkelFlowContext. Keys are per-user\n    and may be rotated by the platform on re-authentication.\n  sources:\n  - openapi/snorkel-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snorkel-ai/refs/heads/main/authentication/snorkel-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Data Development
- Programmatic Labeling
- Weak Supervision
- Evaluation
- SDK
---
