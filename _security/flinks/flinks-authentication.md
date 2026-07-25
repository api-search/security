---
api_key_in:
- header
api_specs:
- filename: flinks-authorize-api-openapi.yml
  format: yaml
  label: Flinks Authorize API
  slug: flinks-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-authorize-api-openapi.yml
- filename: flinks-connect-api-openapi.yml
  format: yaml
  label: Flinks Connect API
  slug: flinks-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-connect-api-openapi.yml
- filename: flinks-enrich-api-openapi.yml
  format: yaml
  label: Flinks Enrich API
  slug: flinks-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-enrich-api-openapi.yml
- filename: flinks-fraud-api-openapi.yml
  format: yaml
  label: Flinks Fraud API
  slug: flinks-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-fraud-api-openapi.yml
- filename: flinks-identity-api-openapi.yml
  format: yaml
  label: Flinks Identity API
  slug: flinks-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-identity-api-openapi.yml
- filename: flinks-score-api-openapi.yml
  format: yaml
  label: Flinks Score API
  slug: flinks-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-score-api-openapi.yml
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
