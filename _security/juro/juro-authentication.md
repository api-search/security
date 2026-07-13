---
api_key_in: []
api_specs:
- filename: juro-openapi.yml
  format: yaml
  label: Juro Contracts API
  slug: juro-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juro/refs/heads/main/openapi/juro-openapi.yml
- filename: juro-openapi.yml
  format: yaml
  label: Juro Templates API
  slug: juro-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juro/refs/heads/main/openapi/juro-openapi.yml
- filename: juro-openapi.yml
  format: yaml
  label: Juro Signatures API
  slug: juro-signatures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juro/refs/heads/main/openapi/juro-openapi.yml
- filename: juro-openapi.yml
  format: yaml
  label: Juro Webhooks API
  slug: juro-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juro/refs/heads/main/openapi/juro-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Juro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Juro secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Juro
provider_slug: juro
scheme_count: 1
schemes:
- description: API key generated in the Juro app under Settings > Integrations > API (also referred to as the Connectors hub). Sent on every request as the `x-api-key` header. API access is plan-gated - it is included with a Juro subscription and enabled through your Customer Success Manager. A sandbox key/environment is available at https://api-sandbox.juro.io/v3.
  in: header
  keyName: x-api-key
  name: apiKeyAuth
  scheme: api-key
  sources:
  - openapi/juro-openapi.yml
  - https://api-docs.juro.com/
  - https://intercom.help/juro/en/articles/8075637-working-with-juro-s-api
  type: apiKey
slug: juro-authentication
source_filename: juro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/juro-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  keyName: x-api-key\n  scheme: api-key\n  description: 'API key generated in the Juro app under Settings > Integrations > API\n    (also referred to as the Connectors hub). Sent on every request as the `x-api-key`\n    header. API access is plan-gated - it is included with a Juro subscription and\n    enabled through your Customer Success Manager. A sandbox key/environment is\n    available at https://api-sandbox.juro.io/v3.'\n  sources:\n  - openapi/juro-openapi.yml\n  - https://api-docs.juro.com/\n  - https://intercom.help/juro/en/articles/8075637-working-with-juro-s-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juro/refs/heads/main/authentication/juro-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Contract Management
- CLM
- Contract Lifecycle
- Contract Automation
- Legal
- LegalTech
- E-Signature
- Contracts
---
