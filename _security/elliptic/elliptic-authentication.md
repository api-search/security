---
api_key_in:
- header
api_specs:
- filename: elliptic-assets-api-openapi.yml
  format: yaml
  label: Elliptic Assets API
  slug: elliptic-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-assets-api-openapi.yml
- filename: elliptic-count-analyses-api-openapi.yml
  format: yaml
  label: Elliptic Count Analyses API
  slug: elliptic-count-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-count-analyses-api-openapi.yml
- filename: elliptic-criteria-api-openapi.yml
  format: yaml
  label: Elliptic Criteria API
  slug: elliptic-criteria-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-criteria-api-openapi.yml
- filename: elliptic-customers-api-openapi.yml
  format: yaml
  label: Elliptic Customers API
  slug: elliptic-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-customers-api-openapi.yml
- filename: elliptic-health-api-openapi.yml
  format: yaml
  label: Elliptic Health API
  slug: elliptic-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-health-api-openapi.yml
- filename: elliptic-risk-rules-api-openapi.yml
  format: yaml
  label: Elliptic Risk Rules API
  slug: elliptic-risk-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-risk-rules-api-openapi.yml
- filename: elliptic-sanctions-api-openapi.yml
  format: yaml
  label: Elliptic Sanctions API
  slug: elliptic-sanctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-sanctions-api-openapi.yml
- filename: elliptic-screenings-api-openapi.yml
  format: yaml
  label: Elliptic Screenings API
  slug: elliptic-screenings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-screenings-api-openapi.yml
- filename: elliptic-transaction-analyses-api-openapi.yml
  format: yaml
  label: Elliptic Transaction Analyses API
  slug: elliptic-transaction-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-transaction-analyses-api-openapi.yml
- filename: elliptic-transaction-workflow-api-openapi.yml
  format: yaml
  label: Elliptic Transaction Workflow API
  slug: elliptic-transaction-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-transaction-workflow-api-openapi.yml
- filename: elliptic-tron-nodeintelligence-api-openapi.yml
  format: yaml
  label: Elliptic Tron NodeIntelligence API
  slug: elliptic-tron-nodeintelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-tron-nodeintelligence-api-openapi.yml
- filename: elliptic-users-api-openapi.yml
  format: yaml
  label: Elliptic Users API
  slug: elliptic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-users-api-openapi.yml
- filename: elliptic-wallet-analyses-api-openapi.yml
  format: yaml
  label: Elliptic Wallet Analyses API
  slug: elliptic-wallet-analyses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-analyses-api-openapi.yml
- filename: elliptic-wallet-analyses-count-api-openapi.yml
  format: yaml
  label: Elliptic Wallet Analyses Count API
  slug: elliptic-wallet-analyses-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-analyses-count-api-openapi.yml
- filename: elliptic-wallet-api-openapi.yml
  format: yaml
  label: Elliptic Wallet API
  slug: elliptic-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-api-openapi.yml
- filename: elliptic-wallet-workflow-api-openapi.yml
  format: yaml
  label: Elliptic Wallet Workflow API
  slug: elliptic-wallet-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/elliptic-wallet-workflow-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Elliptic Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Elliptic secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Elliptic
provider_slug: elliptic
scheme_count: 5
schemes:
- flows:
  - authorizationUrl: https://login.elliptic.co/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.elliptic.co/oauth/token
  name: oauth2
  sources:
  - openapi/aml-api-oauth.json
  type: oauth2
- description: API Key
  in: header
  name: apiKey
  parameter: x-access-key
  sources:
  - openapi/aml-api-oauth.json
  - openapi/aml-api-v2.json
  - openapi/aml-api-v3.json
  - openapi/ia-api.json
  type: apiKey
- description: (Request Time, HTTP Method, Lowercase Path, Request Payload) signed with API Secret
  in: header
  name: signature
  parameter: x-access-sign
  sources:
  - openapi/aml-api-oauth.json
  - openapi/aml-api-v2.json
  - openapi/aml-api-v3.json
  - openapi/ia-api.json
  type: apiKey
- in: header
  name: timestamp
  parameter: x-access-timestamp
  sources:
  - openapi/aml-api-oauth.json
  - openapi/aml-api-v2.json
  - openapi/aml-api-v3.json
  - openapi/ia-api.json
  type: apiKey
- bearerFormat: JWT
  description: Bearer Authentication
  name: bearer
  scheme: bearer
  sources:
  - openapi/aml-api-v2.json
  - openapi/aml-api-v3.json
  - openapi/data-fabric.yaml
  - openapi/ia-api.json
  type: http
slug: elliptic-authentication
source_filename: elliptic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aml-api-oauth.json, openapi/aml-api-v2.json, openapi/aml-api-v3.json, openapi/data-fabric.yaml,\n  openapi/ia-api.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.elliptic.co/authorize\n    tokenUrl: https://login.elliptic.co/oauth/token\n    scopes: 2\n  sources:\n  - openapi/aml-api-oauth.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-access-key\n  description: API Key\n  sources:\n  - openapi/aml-api-oauth.json\n  - openapi/aml-api-v2.json\n  - openapi/aml-api-v3.json\n  - openapi/ia-api.json\n- name: signature\n  type: apiKey\n  in: header\n  parameter: x-access-sign\n  description: (Request Time, HTTP Method, Lowercase Path, Request Payload) signed with API\n    Secret\n  sources:\n  - openapi/aml-api-oauth.json\n\
  \  - openapi/aml-api-v2.json\n  - openapi/aml-api-v3.json\n  - openapi/ia-api.json\n- name: timestamp\n  type: apiKey\n  in: header\n  parameter: x-access-timestamp\n  sources:\n  - openapi/aml-api-oauth.json\n  - openapi/aml-api-v2.json\n  - openapi/aml-api-v3.json\n  - openapi/ia-api.json\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer Authentication\n  sources:\n  - openapi/aml-api-v2.json\n  - openapi/aml-api-v3.json\n  - openapi/data-fabric.yaml\n  - openapi/ia-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/authentication/elliptic-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Blockchain
- Crypto
- Compliance
- AML
- Transaction Screening
- Wallet Screening
- Risk Scoring
- Analytics
---
