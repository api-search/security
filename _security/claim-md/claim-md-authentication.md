---
api_key_in:
- query
api_specs:
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD Claim Submission API
  slug: claim-submission
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD Claim Status API
  slug: claim-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD ERA / Remits API
  slug: era-remits
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD Eligibility API
  slug: eligibility
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD Responses & Files API
  slug: responses-files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Claim Md Authentication
name_suffix: Authentication
oauth_flows: []
overview: Claim.MD secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Claim.MD
provider_slug: claim-md
scheme_count: 1
schemes:
- description: Account authentication key from Settings > Account Settings in the Claim.MD portal. Submitted with each request (as a form field or query parameter).
  in: query
  name: AccountKey
  parameter: AccountKey
  sources:
  - openapi/claim-md-openapi.yml
  type: apiKey
slug: claim-md-authentication
source_filename: claim-md-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/claim-md-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: AccountKey\n  type: apiKey\n  in: query\n  parameter: AccountKey\n  description: Account authentication key from Settings > Account Settings in the Claim.MD portal.\n    Submitted with each request (as a form field or query parameter).\n  sources:\n  - openapi/claim-md-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/authentication/claim-md-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Healthcare
- Medical Claims
- Clearinghouse
- EDI
- X12
- Revenue Cycle
---
