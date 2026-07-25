---
api_key_in:
- header
api_specs:
- filename: onomondo-connectors-api-openapi.yml
  format: yaml
  label: Onomondo Connectors API
  slug: onomondo-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/openapi/onomondo-connectors-api-openapi.yml
- filename: onomondo-network-lists-api-openapi.yml
  format: yaml
  label: Onomondo Network Lists API
  slug: onomondo-network-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/openapi/onomondo-network-lists-api-openapi.yml
- filename: onomondo-sims-api-openapi.yml
  format: yaml
  label: Onomondo SIMs API
  slug: onomondo-sims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/openapi/onomondo-sims-api-openapi.yml
- filename: onomondo-sms-api-openapi.yml
  format: yaml
  label: Onomondo SMS API
  slug: onomondo-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/openapi/onomondo-sms-api-openapi.yml
- filename: onomondo-tags-api-openapi.yml
  format: yaml
  label: Onomondo Tags API
  slug: onomondo-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/openapi/onomondo-tags-api-openapi.yml
- filename: onomondo-usage-api-openapi.yml
  format: yaml
  label: Onomondo Usage API
  slug: onomondo-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/openapi/onomondo-usage-api-openapi.yml
- filename: onomondo-webhooks-api-openapi.yml
  format: yaml
  label: Onomondo Webhooks API
  slug: onomondo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/openapi/onomondo-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Onomondo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Onomondo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Onomondo
provider_slug: onomondo
scheme_count: 1
schemes:
- description: Organization-scoped API key supplied in the Authorization header. Generated in the Onomondo platform and coupled to the organization under which it is created.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/onomondo-openapi.yml
  type: apiKey
slug: onomondo-authentication
source_filename: onomondo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/onomondo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Organization-scoped API key supplied in the Authorization header. Generated in\n    the Onomondo platform and coupled to the organization under which it is created.\n  sources:\n  - openapi/onomondo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onomondo/refs/heads/main/authentication/onomondo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- IoT
- Connectivity
- Cellular
- SIM
- Telecom
---
