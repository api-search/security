---
api_key_in:
- header
api_specs:
- filename: protonai-call-notes-api-openapi.yml
  format: yaml
  label: Proton.ai Call Notes API
  slug: protonai-call-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/openapi/protonai-call-notes-api-openapi.yml
- filename: protonai-contacts-api-openapi.yml
  format: yaml
  label: Proton.ai Contacts API
  slug: protonai-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/openapi/protonai-contacts-api-openapi.yml
- filename: protonai-custom-fields-api-openapi.yml
  format: yaml
  label: Proton.ai Custom Fields API
  slug: protonai-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/openapi/protonai-custom-fields-api-openapi.yml
- filename: protonai-customers-api-openapi.yml
  format: yaml
  label: Proton.ai Customers API
  slug: protonai-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/openapi/protonai-customers-api-openapi.yml
- filename: protonai-leads-api-openapi.yml
  format: yaml
  label: Proton.ai Leads API
  slug: protonai-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/openapi/protonai-leads-api-openapi.yml
- filename: protonai-opportunities-api-openapi.yml
  format: yaml
  label: Proton.ai Opportunities API
  slug: protonai-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/openapi/protonai-opportunities-api-openapi.yml
- filename: protonai-product-initiatives-api-openapi.yml
  format: yaml
  label: Proton.ai Product Initiatives API
  slug: protonai-product-initiatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/openapi/protonai-product-initiatives-api-openapi.yml
- filename: protonai-quotes-api-openapi.yml
  format: yaml
  label: Proton.ai Quotes API
  slug: protonai-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/openapi/protonai-quotes-api-openapi.yml
- filename: protonai-recommendations-api-openapi.yml
  format: yaml
  label: Proton.ai Recommendations API
  slug: protonai-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/openapi/protonai-recommendations-api-openapi.yml
- filename: protonai-search-api-openapi.yml
  format: yaml
  label: Proton.ai Search API
  slug: protonai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/openapi/protonai-search-api-openapi.yml
- filename: protonai-tasks-api-openapi.yml
  format: yaml
  label: Proton.ai Tasks API
  slug: protonai-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/openapi/protonai-tasks-api-openapi.yml
- filename: protonai-tracking-api-openapi.yml
  format: yaml
  label: Proton.ai Tracking API
  slug: protonai-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/openapi/protonai-tracking-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Protonai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Proton.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Proton.ai
provider_slug: protonai
scheme_count: 1
schemes:
- description: Static API key supplied by Proton at integration onboarding.
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/protonai-openapi.yml
  type: apiKey
slug: protonai-authentication
source_filename: protonai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/protonai-openapi.yml\ndocs: https://api.proton.ai/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Auth is a single static API key sent in the X-Api-Key header, supplied by\n    Proton at the start of an integration (no dynamic generation or refresh).\n    Requests are additionally scoped by an X-Company tenant header and an\n    optional X-User-Id acting-user header. There is no OAuth surface.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Static API key supplied by Proton at integration onboarding.\n  sources:\n  - openapi/protonai-openapi.yml\nadditional_headers:\n- name: X-Company\n  required: true\n  description: Tenant company slug; also appears as the first path segment (/{company}/...).\n- name: X-User-Id\n  required: false\n  description: Identifies the acting user for attribution on writes and tracking events.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/protonai/refs/heads/main/authentication/protonai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- CRM
- Sales
- Distribution
- Artificial Intelligence
- Recommendations
- B2B
- Wholesale Distribution
---
