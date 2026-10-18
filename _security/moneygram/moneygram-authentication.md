---
anonymous_access: false
api_key_in: []
api_specs:
- filename: moneygram-accounts-api-openapi.yml
  format: yaml
  label: MoneyGram Accounts API
  slug: moneygram-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-accounts-api-openapi.yml
- filename: moneygram-amend-api-openapi.yml
  format: yaml
  label: MoneyGram Amend API
  slug: moneygram-amend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-amend-api-openapi.yml
- filename: moneygram-fx-rate-api-openapi.yml
  format: yaml
  label: MoneyGram Fx Rate API
  slug: moneygram-fx-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-fx-rate-api-openapi.yml
- filename: moneygram-oauth-api-openapi.yml
  format: yaml
  label: MoneyGram OAuth API
  slug: moneygram-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-oauth-api-openapi.yml
- filename: moneygram-partnerconnect-api-openapi.yml
  format: yaml
  label: MoneyGram Partnerconnect API
  slug: moneygram-partnerconnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-partnerconnect-api-openapi.yml
- filename: moneygram-reference-data-api-openapi.yml
  format: yaml
  label: MoneyGram Reference Data API
  slug: moneygram-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-reference-data-api-openapi.yml
- filename: moneygram-transactions-api-openapi.yml
  format: yaml
  label: MoneyGram Transactions API
  slug: moneygram-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-transactions-api-openapi.yml
- filename: moneygram-transfer-api-openapi.yml
  format: yaml
  label: MoneyGram Transfer API
  slug: moneygram-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-transfer-api-openapi.yml
- filename: moneygram-transfers-api-openapi.yml
  format: yaml
  label: MoneyGram Transfers API
  slug: moneygram-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-transfers-api-openapi.yml
auth_types: []
description: Authentication for MoneyGram APIs uses OAuth 2.0 client credentials flow with HTTP Basic authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Moneygram Authentication
name_suffix: Authentication
oauth_flows: []
overview: MoneyGram declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MoneyGram
provider_slug: moneygram
scheme_count: 1
schemes:
- evidence: MoneyGram uses the OAuth 2.0 framework. The application must use their OAuth client credentials to generate an accesstoken and pass it as a header value in API HTTP calls.
  header: Authorization
  how_to_obtain: Client ID and secret are provided by MoneyGram after partnership.
  location: header
  name: Basic
  token_url: https://api.moneygram.com/oauth/accesstoken?grant_type=client_credentials
  type: http-basic
slug: moneygram-authentication
source_filename: moneygram-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.moneygram.com/moneygram-developer/recipes/oauth-api-retrieve-an-access-token
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.moneygram.com/moneygram-developer/recipes/oauth-api-retrieve-an-access-token\nsources:\n- https://developer.moneygram.com/moneygram-developer/recipes/oauth-api-retrieve-an-access-token\n- https://developer.moneygram.com/moneygram-developer/docs/o-auth-api\ndescription: Authentication for MoneyGram APIs uses OAuth 2.0 client credentials flow with HTTP Basic authentication.\nschemes:\n- type: http-basic\n  name: Basic\n  evidence: MoneyGram uses the OAuth 2.0 framework. The application must use their OAuth client credentials to generate an accesstoken and pass\n    it as a header value in API HTTP calls.\n  location: header\n  header: Authorization\n  token_url: https://api.moneygram.com/oauth/accesstoken?grant_type=client_credentials\n  how_to_obtain: Client ID and secret are provided by MoneyGram after partnership.\ndocs: https://developer.moneygram.com/moneygram-developer/recipes/oauth-api-retrieve-an-access-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/authentication/moneygram-authentication.yml
summary_line: 1 scheme
tags:
- Money
- Payments
- Transfer
- Fintech
- Global
---
