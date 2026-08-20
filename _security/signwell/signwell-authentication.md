---
api_key_in:
- header
api_specs:
- filename: signwell-api-application-api-openapi.yml
  format: yaml
  label: SignWell API Application API
  slug: signwell-api-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signwell/refs/heads/main/openapi/signwell-api-application-api-openapi.yml
- filename: signwell-bulk-send-api-openapi.yml
  format: yaml
  label: SignWell Bulk Send API
  slug: signwell-bulk-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signwell/refs/heads/main/openapi/signwell-bulk-send-api-openapi.yml
- filename: signwell-document-api-openapi.yml
  format: yaml
  label: SignWell Document API
  slug: signwell-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signwell/refs/heads/main/openapi/signwell-document-api-openapi.yml
- filename: signwell-me-api-openapi.yml
  format: yaml
  label: SignWell Me API
  slug: signwell-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signwell/refs/heads/main/openapi/signwell-me-api-openapi.yml
- filename: signwell-regional-api-openapi.yml
  format: yaml
  label: SignWell Regional API
  slug: signwell-regional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signwell/refs/heads/main/openapi/signwell-regional-api-openapi.yml
- filename: signwell-template-api-openapi.yml
  format: yaml
  label: SignWell Template API
  slug: signwell-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signwell/refs/heads/main/openapi/signwell-template-api-openapi.yml
- filename: signwell-webhooks-api-openapi.yml
  format: yaml
  label: SignWell Webhooks API
  slug: signwell-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signwell/refs/heads/main/openapi/signwell-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Signwell Authentication
name_suffix: Authentication
oauth_flows: []
overview: SignWell secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SignWell
provider_slug: signwell
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: X-Api-Key
  sources:
  - openapi/signwell-signwell-api-openapi.yml
  type: apiKey
slug: signwell-authentication
source_filename: signwell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/signwell-signwell-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/signwell-signwell-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signwell/refs/heads/main/authentication/signwell-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- E-Signature
- Electronic Signature
- Documents
- PDF
- Signing
- Templates
- Workflows
- HIPAA
- SOC 2
---
