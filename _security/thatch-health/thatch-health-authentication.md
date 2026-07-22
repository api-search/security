---
api_key_in:
- header
api_specs:
- filename: thatch-health-platforms-openapi-original.yml
  format: yaml
  label: Thatch for Platforms API
  slug: thatch-for-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thatch-health/refs/heads/main/openapi/thatch-health-platforms-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Thatch Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thatch Health secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Thatch Health
provider_slug: thatch-health
scheme_count: 1
schemes:
- description: Provide your API key in a `Bearer` token header (as in, **Bearer sk_123**).
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/thatch-health-platforms-openapi-original.yml
  type: apiKey
slug: thatch-health-authentication
source_filename: thatch-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/thatch-health-platforms-openapi-original.yml\ndocs: https://docs.thatch.com/\nnotes: API keys are generated in the Thatch dashboard (app.thatch.com) and sent as\n  `Authorization Bearer <YOUR_API_KEY>` on every request; keys use an `sk_` prefix.\n  Partner accounts are provisioned by Thatch (platforms@thatch.com). Admin surfaces\n  on partners.thatchcloud.com and app.thatch.com expose OIDC discovery documents\n  (authorization-code flow, ES256), captured in well-known/.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Provide your API key in a `Bearer` token header (as in, **Bearer sk_123**).\n  sources:\n  - openapi/thatch-health-platforms-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thatch-health/refs/heads/main/authentication/thatch-health-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Healthcare
- Health Benefits
- ICHRA
- Insurance
- Payroll
- Embedded Benefits
- HR
---
