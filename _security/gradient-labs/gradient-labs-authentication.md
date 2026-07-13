---
api_key_in: []
api_specs:
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Conversations API
  slug: gradient-labs-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Messages API
  slug: gradient-labs-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Hand-off & Assignment API
  slug: gradient-labs-hand-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Actions & Tools API
  slug: gradient-labs-actions-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Knowledge API
  slug: gradient-labs-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Webhooks API
  slug: gradient-labs-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gradient Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gradient Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gradient Labs
provider_slug: gradient-labs
scheme_count: 1
schemes:
- description: Provide your Gradient Labs API key as a Bearer token in the Authorization header. Some administrative endpoints (tools) require a Management API key.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gradient-labs-openapi.yml
  type: http
slug: gradient-labs-authentication
source_filename: gradient-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gradient-labs-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Provide your Gradient Labs API key as a Bearer token in the Authorization header.\n    Some administrative endpoints (tools) require a Management API key.\n  sources:\n  - openapi/gradient-labs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/authentication/gradient-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Customer Support
- AI Agent
- Conversations
- Financial Services
- Regulated
---
