---
api_key_in:
- header
- query
api_specs:
- filename: gitcoin-bounties-api-openapi.yml
  format: yaml
  label: Gitcoin Bounties API
  slug: gitcoin-bounties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/openapi/gitcoin-bounties-api-openapi.yml
- filename: gitcoin-contributors-api-openapi.yml
  format: yaml
  label: Gitcoin Contributors API
  slug: gitcoin-contributors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/openapi/gitcoin-contributors-api-openapi.yml
- filename: gitcoin-grants-api-openapi.yml
  format: yaml
  label: Gitcoin Grants API
  slug: gitcoin-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/openapi/gitcoin-grants-api-openapi.yml
- filename: gitcoin-model-analysis-api-openapi.yml
  format: yaml
  label: Gitcoin Model Analysis API
  slug: gitcoin-model-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/openapi/gitcoin-model-analysis-api-openapi.yml
- filename: gitcoin-rounds-api-openapi.yml
  format: yaml
  label: Gitcoin Rounds API
  slug: gitcoin-rounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/openapi/gitcoin-rounds-api-openapi.yml
- filename: gitcoin-stamp-api-api-openapi.yml
  format: yaml
  label: Gitcoin Stamp API API
  slug: gitcoin-stamp-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/openapi/gitcoin-stamp-api-api-openapi.yml
auth_types:
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Gitcoin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gitcoin secures its APIs with apiKey and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gitcoin
provider_slug: gitcoin
scheme_count: 4
schemes:
- description: API key obtained from the response body's meta.api_key field after authenticating via the GitHub authentication flow
  in: query
  name: ApiKeyAuth
  parameter: _key
  sources:
  - openapi/gitcoin-grants-api-openapi.json
  type: apiKey
- description: API secret used alongside the API key for authentication
  in: query
  name: ApiSecretAuth
  parameter: _secret
  sources:
  - openapi/gitcoin-grants-api-openapi.json
  type: apiKey
- description: GitHub OAuth authentication for Gitcoin
  name: GitHubAuth
  openIdConnectUrl: https://github.com/.well-known/openid-configuration
  sources:
  - openapi/gitcoin-grants-api-openapi.json
  type: openIdConnect
- in: header
  name: function
  parameter: X-API-Key
  sources:
  - openapi/gitcoin-passport-stamps-api-openapi.json
  type: apiKey
slug: gitcoin-authentication
source_filename: gitcoin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gitcoin-grants-api-openapi.json, openapi/gitcoin-passport-stamps-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  - openIdConnect\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: _key\n  description: API key obtained from the response body's meta.api_key field after authenticating\n    via the GitHub authentication flow\n  sources:\n  - openapi/gitcoin-grants-api-openapi.json\n- name: ApiSecretAuth\n  type: apiKey\n  in: query\n  parameter: _secret\n  description: API secret used alongside the API key for authentication\n  sources:\n  - openapi/gitcoin-grants-api-openapi.json\n- name: GitHubAuth\n  type: openIdConnect\n  openIdConnectUrl: https://github.com/.well-known/openid-configuration\n  description: GitHub OAuth authentication for Gitcoin\n  sources:\n  - openapi/gitcoin-grants-api-openapi.json\n- name: function\n  type: apiKey\n  in: header\n  parameter:\
  \ X-API-Key\n  sources:\n  - openapi/gitcoin-passport-stamps-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/authentication/gitcoin-authentication.yml
summary_line: apiKey/openIdConnect · 4 schemes
tags:
- Public Goods
- Grants
- Bounties
- Quadratic Funding
- Web3
- Verifiable Credentials
- Identity
- Open Source
---
