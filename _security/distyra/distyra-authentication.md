---
anonymous_access: false
api_key_in: []
api_specs:
- filename: distyra-authentication-api-openapi.yml
  format: yaml
  label: Brightfield Software Authentication API
  slug: distyra-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-authentication-api-openapi.yml
- filename: distyra-billing-api-openapi.yml
  format: yaml
  label: Brightfield Software Billing API
  slug: distyra-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-billing-api-openapi.yml
- filename: distyra-catalog-api-openapi.yml
  format: yaml
  label: Brightfield Software Catalog API
  slug: distyra-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-catalog-api-openapi.yml
- filename: distyra-connect-api-openapi.yml
  format: yaml
  label: Brightfield Software Connect API
  slug: distyra-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-connect-api-openapi.yml
- filename: distyra-enrichment-api-openapi.yml
  format: yaml
  label: Brightfield Software Enrichment API
  slug: distyra-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-enrichment-api-openapi.yml
- filename: distyra-feedback-api-openapi.yml
  format: yaml
  label: Brightfield Software Feedback API
  slug: distyra-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-feedback-api-openapi.yml
- filename: distyra-system-api-openapi.yml
  format: yaml
  label: Brightfield Software System API
  slug: distyra-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-system-api-openapi.yml
- filename: distyra-underwriting-api-openapi.yml
  format: yaml
  label: Brightfield Software Underwriting API
  slug: distyra-underwriting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-underwriting-api-openapi.yml
- filename: distyra-webhooks-api-openapi.yml
  format: yaml
  label: Brightfield Software Webhooks API
  slug: distyra-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Distyra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brightfield Software secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brightfield Software
provider_slug: distyra
scheme_count: 1
schemes:
- bearerFormat: sk_<32 base58 chars>
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/distyra-openapi.json
  type: http
slug: distyra-authentication
source_filename: distyra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: derived\nsource: openapi/distyra-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: sk_<32 base58 chars>\n  sources:\n  - openapi/distyra-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/authentication/distyra-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Banking
- API
- Fintech
- European
---
