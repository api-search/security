---
api_key_in: []
api_specs:
- filename: alloy-com-bank-accounts-api-openapi.yml
  format: yaml
  label: Alloy Bank Accounts API
  slug: alloy-com-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-bank-accounts-api-openapi.yml
- filename: alloy-com-batches-api-openapi.yml
  format: yaml
  label: Alloy Batches API
  slug: alloy-com-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-batches-api-openapi.yml
- filename: alloy-com-cases-api-openapi.yml
  format: yaml
  label: Alloy Cases API
  slug: alloy-com-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-cases-api-openapi.yml
- filename: alloy-com-custom-lists-api-openapi.yml
  format: yaml
  label: Alloy Custom Lists API
  slug: alloy-com-custom-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-custom-lists-api-openapi.yml
- filename: alloy-com-documents-api-openapi.yml
  format: yaml
  label: Alloy Documents API
  slug: alloy-com-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-documents-api-openapi.yml
- filename: alloy-com-entities-api-openapi.yml
  format: yaml
  label: Alloy Entities API
  slug: alloy-com-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-entities-api-openapi.yml
- filename: alloy-com-evaluations-api-openapi.yml
  format: yaml
  label: Alloy Evaluations API
  slug: alloy-com-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-evaluations-api-openapi.yml
- filename: alloy-com-events-api-openapi.yml
  format: yaml
  label: Alloy Events API
  slug: alloy-com-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-events-api-openapi.yml
- filename: alloy-com-groups-api-openapi.yml
  format: yaml
  label: Alloy Groups API
  slug: alloy-com-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-groups-api-openapi.yml
- filename: alloy-com-investigations-api-openapi.yml
  format: yaml
  label: Alloy Investigations API
  slug: alloy-com-investigations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-investigations-api-openapi.yml
- filename: alloy-com-journeys-api-openapi.yml
  format: yaml
  label: Alloy Journeys API
  slug: alloy-com-journeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-journeys-api-openapi.yml
- filename: alloy-com-lists-api-openapi.yml
  format: yaml
  label: Alloy Lists API
  slug: alloy-com-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-lists-api-openapi.yml
- filename: alloy-com-oauth-api-openapi.yml
  format: yaml
  label: Alloy OAuth API
  slug: alloy-com-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-oauth-api-openapi.yml
- filename: alloy-com-parameters-api-openapi.yml
  format: yaml
  label: Alloy Parameters API
  slug: alloy-com-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-parameters-api-openapi.yml
- filename: alloy-com-portfolio-evaluations-api-openapi.yml
  format: yaml
  label: Alloy Portfolio Evaluations API
  slug: alloy-com-portfolio-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-portfolio-evaluations-api-openapi.yml
- filename: alloy-com-published-attributes-api-openapi.yml
  format: yaml
  label: Alloy Published Attributes API
  slug: alloy-com-published-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-published-attributes-api-openapi.yml
- filename: alloy-com-reviews-api-openapi.yml
  format: yaml
  label: Alloy Reviews API
  slug: alloy-com-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/openapi/alloy-com-reviews-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Alloy Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alloy secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Alloy
provider_slug: alloy-com
scheme_count: 2
schemes:
- description: HTTP Basic Authentication with workflow or account-level API key as username and secret as password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/alloy-openapi.yml
  type: http
- description: OAuth 2.0 bearer token obtained via the OAuth endpoints.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/alloy-openapi.yml
  type: http
slug: alloy-com-authentication
source_filename: alloy-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alloy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication with workflow or account-level API key as username\n    and secret as password.\n  sources:\n  - openapi/alloy-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token obtained via the OAuth endpoints.\n  sources:\n  - openapi/alloy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloy-com/refs/heads/main/authentication/alloy-com-authentication.yml
summary_line: http · 2 schemes
tags:
- Identity Decisioning
- Identity Verification
- KYC
- KYB
- AML
- Fraud Prevention
- Credit Underwriting
- Ongoing Monitoring
- Case Management
- Fintech
- Banking
---
