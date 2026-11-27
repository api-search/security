---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openstela-io-account-api-openapi.yml
  format: yaml
  label: OpenStela Account API
  slug: openstela-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-account-api-openapi.yml
- filename: openstela-io-characters-api-openapi.yml
  format: yaml
  label: OpenStela Characters API
  slug: openstela-io-characters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-characters-api-openapi.yml
- filename: openstela-io-deals-read-only-api-openapi.yml
  format: yaml
  label: OpenStela Deals (read-only) API
  slug: openstela-io-deals-read-only-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-deals-read-only-api-openapi.yml
- filename: openstela-io-messages-api-openapi.yml
  format: yaml
  label: OpenStela Messages API
  slug: openstela-io-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-messages-api-openapi.yml
- filename: openstela-io-public-api-openapi.yml
  format: yaml
  label: OpenStela Public API
  slug: openstela-io-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-public-api-openapi.yml
- filename: openstela-io-verify-api-openapi.yml
  format: yaml
  label: OpenStela Verify API
  slug: openstela-io-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-verify-api-openapi.yml
- filename: openstela-io-works-api-openapi.yml
  format: yaml
  label: OpenStela Works API
  slug: openstela-io-works-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openstela-io/openapi/openstela-io-works-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: OpenStela Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenStela declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OpenStela
provider_slug: openstela-io
scheme_count: 1
schemes:
- evidence: 'Auth: Authorization: Bearer alk_… — create keys in Account settings.'
  header: Authorization
  how_to_obtain: Create keys in Account settings.
  location: header
  name: Bearer
  type: http-bearer
slug: openstela-io-authentication
source_filename: openstela-io-authentication.yml
source_heading: Authentication Profile
source_url: https://app.openstela.io/api/docs#/Account/post_api_account_tokens
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://app.openstela.io/api/docs#/Account/post_api_account_tokens\nsources:\n- https://app.openstela.io/api/docs#/Account/post_api_account_tokens\n- https://app.openstela.io/api/docs#/Account/delete_api_account_tokens_prefix\n- https://app.openstela.io/api/docs\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Auth: Authorization: Bearer alk_… — create keys in Account settings.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys in Account settings.\ndocs: https://app.openstela.io/api/docs#/Account/post_api_account_tokens\n"
source_yaml_url: https://artifacts.apis.io/openstela-io/authentication/openstela-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Blockchain
- Marketplace
- Digital Assets
- Creators
---
