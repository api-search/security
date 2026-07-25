---
api_key_in:
- header
api_specs:
- filename: harbor-compliance-compliance-filings-api-openapi.yml
  format: yaml
  label: Harbor Compliance Compliance Filings API
  slug: harbor-compliance-compliance-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/openapi/harbor-compliance-compliance-filings-api-openapi.yml
- filename: harbor-compliance-entities-api-openapi.yml
  format: yaml
  label: Harbor Compliance Entities API
  slug: harbor-compliance-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/openapi/harbor-compliance-entities-api-openapi.yml
- filename: harbor-compliance-jurisdictions-api-openapi.yml
  format: yaml
  label: Harbor Compliance Jurisdictions API
  slug: harbor-compliance-jurisdictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/openapi/harbor-compliance-jurisdictions-api-openapi.yml
- filename: harbor-compliance-licenses-api-openapi.yml
  format: yaml
  label: Harbor Compliance Licenses API
  slug: harbor-compliance-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/openapi/harbor-compliance-licenses-api-openapi.yml
- filename: harbor-compliance-orders-api-openapi.yml
  format: yaml
  label: Harbor Compliance Orders API
  slug: harbor-compliance-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/openapi/harbor-compliance-orders-api-openapi.yml
- filename: harbor-compliance-registered-agents-api-openapi.yml
  format: yaml
  label: Harbor Compliance Registered Agents API
  slug: harbor-compliance-registered-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/openapi/harbor-compliance-registered-agents-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Harbor Compliance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harbor Compliance secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Harbor Compliance
provider_slug: harbor-compliance
scheme_count: 1
schemes:
- description: API key for authenticating partner requests. Obtain your API key from the Harbor Compliance developer portal.
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/harbor-compliance-openapi.yml
  type: apiKey
slug: harbor-compliance-authentication
source_filename: harbor-compliance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/harbor-compliance-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key for authenticating partner requests. Obtain your API key from the Harbor\n    Compliance developer portal.\n  sources:\n  - openapi/harbor-compliance-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/authentication/harbor-compliance-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Business Licensing
- Compliance
- Legal
- Regulatory
---
