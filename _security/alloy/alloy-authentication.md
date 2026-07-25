---
api_key_in: []
api_specs:
- filename: alloy-bank-accounts-api-openapi.yml
  format: yaml
  label: Alloy Bank Accounts API
  slug: alloy-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-bank-accounts-api-openapi.yml
- filename: alloy-documents-api-openapi.yml
  format: yaml
  label: Alloy Documents API
  slug: alloy-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-documents-api-openapi.yml
- filename: alloy-entities-api-openapi.yml
  format: yaml
  label: Alloy Entities API
  slug: alloy-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-entities-api-openapi.yml
- filename: alloy-entity-groups-api-openapi.yml
  format: yaml
  label: Alloy Entity Groups API
  slug: alloy-entity-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-entity-groups-api-openapi.yml
- filename: alloy-evaluations-api-openapi.yml
  format: yaml
  label: Alloy Evaluations API
  slug: alloy-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-evaluations-api-openapi.yml
- filename: alloy-events-api-openapi.yml
  format: yaml
  label: Alloy Events API
  slug: alloy-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-events-api-openapi.yml
- filename: alloy-investigations-api-openapi.yml
  format: yaml
  label: Alloy Investigations API
  slug: alloy-investigations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-investigations-api-openapi.yml
- filename: alloy-journeys-api-openapi.yml
  format: yaml
  label: Alloy Journeys API
  slug: alloy-journeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-journeys-api-openapi.yml
- filename: alloy-oauth-api-openapi.yml
  format: yaml
  label: Alloy OAuth API
  slug: alloy-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-oauth-api-openapi.yml
- filename: alloy-transactions-api-openapi.yml
  format: yaml
  label: Alloy Transactions API
  slug: alloy-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/openapi/alloy-transactions-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Alloy Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Alloy secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Alloy
provider_slug: alloy
scheme_count: 2
schemes:
- description: HTTP basic authorization using a workflow token and secret
  name: basic
  scheme: basic
  sources:
  - openapi/alloy-identity-api-openapi.yml
  type: http
- description: OAuth2 using a workflow token and secret to generate a bearer token
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /oauth/bearer
  name: oauth2
  sources:
  - openapi/alloy-identity-api-openapi.yml
  type: oauth2
slug: alloy-authentication
source_filename: alloy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alloy-identity-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  description: HTTP basic authorization using a workflow token and secret\n  sources:\n  - openapi/alloy-identity-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/bearer\n    scopes: 0\n  description: OAuth2 using a workflow token and secret to generate a bearer token\n  sources:\n  - openapi/alloy-identity-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloy/refs/heads/main/authentication/alloy-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Identity Verification
- KYC
- KYB
- Fraud Prevention
- Compliance
- Onboarding
- Transaction Monitoring
- Risk Decisioning
- AML
- Fintech
---
