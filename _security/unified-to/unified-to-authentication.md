---
api_key_in:
- header
api_specs:
- filename: unified-to-accounting-openapi.yaml
  format: yaml
  label: Unified.to Accounting API
  slug: accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-accounting-openapi.yaml
- filename: unified-to-marketing-openapi.yaml
  format: yaml
  label: Unified.to Advertising API
  slug: ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-marketing-openapi.yaml
- filename: unified-to-hr-talent-openapi.yaml
  format: yaml
  label: Unified.to Assessment API
  slug: assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-hr-talent-openapi.yaml
- filename: unified-to-ats-openapi.yaml
  format: yaml
  label: Unified.to ATS API
  slug: ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-ats-openapi.yaml
- filename: unified-to-productivity-openapi.yaml
  format: yaml
  label: Unified.to Calendar & Meetings API
  slug: calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-productivity-openapi.yaml
- filename: unified-to-it-ops-openapi.yaml
  format: yaml
  label: Unified.to Call Center API
  slug: call-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-it-ops-openapi.yaml
- filename: unified-to-crm-openapi.yaml
  format: yaml
  label: Unified.to CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-crm-openapi.yaml
- filename: unified-to-commerce-openapi.yaml
  format: yaml
  label: Unified.to E-Commerce API
  slug: ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-commerce-openapi.yaml
- filename: unified-to-hris-openapi.yaml
  format: yaml
  label: Unified.to HR & Directory API
  slug: hris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-hris-openapi.yaml
- filename: unified-to-productivity-openapi.yaml
  format: yaml
  label: Unified.to Messaging API
  slug: messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-productivity-openapi.yaml
- filename: unified-to-it-ops-openapi.yaml
  format: yaml
  label: Unified.to Payments API
  slug: payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-it-ops-openapi.yaml
- filename: unified-to-it-ops-openapi.yaml
  format: yaml
  label: Unified.to Ticketing API
  slug: ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-it-ops-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Unified To Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unified.to secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unified.to
provider_slug: unified-to
scheme_count: 1
schemes:
- in: header
  name: jwt
  parameter: authorization
  sources:
  - openapi/unified-to-accounting-openapi.yaml
  - openapi/unified-to-ats-openapi.yaml
  - openapi/unified-to-commerce-openapi.yaml
  - openapi/unified-to-crm-openapi.yaml
  - openapi/unified-to-full-openapi.yaml
  - openapi/unified-to-hr-talent-openapi.yaml
  - openapi/unified-to-hris-openapi.yaml
  - openapi/unified-to-it-ops-openapi.yaml
  - openapi/unified-to-marketing-openapi.yaml
  - openapi/unified-to-productivity-openapi.yaml
  - openapi/unified-to-unified-core-openapi.yaml
  type: apiKey
slug: unified-to-authentication
source_filename: unified-to-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unified-to-accounting-openapi.yaml, openapi/unified-to-ats-openapi.yaml, openapi/unified-to-commerce-openapi.yaml,\n  openapi/unified-to-crm-openapi.yaml, openapi/unified-to-full-openapi.yaml, openapi/unified-to-hr-talent-openapi.yaml,\n  openapi/unified-to-hris-openapi.yaml, openapi/unified-to-it-ops-openapi.yaml, openapi/unified-to-marketing-openapi.yaml,\n  openapi/unified-to-productivity-openapi.yaml, openapi/unified-to-unified-core-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: jwt\n  type: apiKey\n  in: header\n  parameter: authorization\n  sources:\n  - openapi/unified-to-accounting-openapi.yaml\n  - openapi/unified-to-ats-openapi.yaml\n  - openapi/unified-to-commerce-openapi.yaml\n  - openapi/unified-to-crm-openapi.yaml\n  - openapi/unified-to-full-openapi.yaml\n  - openapi/unified-to-hr-talent-openapi.yaml\n  - openapi/unified-to-hris-openapi.yaml\n  - openapi/unified-to-it-ops-openapi.yaml\n\
  \  - openapi/unified-to-marketing-openapi.yaml\n  - openapi/unified-to-productivity-openapi.yaml\n  - openapi/unified-to-unified-core-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/authentication/unified-to-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Integrations
- Unified API
---
