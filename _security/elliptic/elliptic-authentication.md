---
api_key_in:
- header
api_specs:
- filename: aml-api-oauth.json
  format: json
  label: Elliptic AML API
  slug: elliptic-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/aml-api-oauth.json
- filename: ia-api.json
  format: json
  label: Elliptic AI API
  slug: elliptic-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/ia-api.json
- filename: sanctions-api.json
  format: json
  label: Elliptic Sanctions API
  slug: elliptic-sanctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/sanctions-api.json
- filename: data-fabric.yaml
  format: yaml
  label: Elliptic Data Fabric API
  slug: elliptic-data-fabric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/data-fabric.yaml
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
