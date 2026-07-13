---
api_key_in:
- header
api_specs:
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Authorize / Connect API
  slug: flinks-authorize-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Accounts Detail API
  slug: flinks-accounts-detail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Accounts Summary API
  slug: flinks-accounts-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Statements API
  slug: flinks-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Identity API
  slug: flinks-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Attributes / Analytics API
  slug: flinks-attributes-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Score API
  slug: flinks-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Fraud / KYC API
  slug: flinks-fraud-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Flinks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flinks secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flinks
provider_slug: flinks
scheme_count: 1
schemes:
- description: Short-lived (30-minute) authorize token obtained from /GenerateAuthorizeToken.
  in: header
  name: flinks_auth_key
  parameter: flinks-auth-key
  sources:
  - openapi/flinks-openapi.yml
  type: apiKey
slug: flinks-authentication
source_filename: flinks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flinks-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: flinks_auth_key\n  type: apiKey\n  in: header\n  parameter: flinks-auth-key\n  description: Short-lived (30-minute) authorize token obtained from /GenerateAuthorizeToken.\n  sources:\n  - openapi/flinks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/authentication/flinks-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Financial Data
- Open Banking
- Bank Aggregation
- Fintech
- Canada
---
