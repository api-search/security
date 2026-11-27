---
anonymous_access: false
api_key_in: []
api_specs:
- filename: algotradertools-accounts-api-openapi.yml
  format: yaml
  label: Algo Trader Tools Accounts API
  slug: algotradertools-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algotradertools/openapi/algotradertools-accounts-api-openapi.yml
- filename: algotradertools-copiers-api-openapi.yml
  format: yaml
  label: Algo Trader Tools Copiers API
  slug: algotradertools-copiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algotradertools/openapi/algotradertools-copiers-api-openapi.yml
- filename: algotradertools-copy-events-api-openapi.yml
  format: yaml
  label: Algo Trader Tools Copy events API
  slug: algotradertools-copy-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algotradertools/openapi/algotradertools-copy-events-api-openapi.yml
- filename: algotradertools-followers-api-openapi.yml
  format: yaml
  label: Algo Trader Tools Followers API
  slug: algotradertools-followers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algotradertools/openapi/algotradertools-followers-api-openapi.yml
auth_types: []
description: Authentication with API keys
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Algo Trader Tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: Algo Trader Tools declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Algo Trader Tools
provider_slug: algotradertools
scheme_count: 2
schemes:
- evidence: 'Pass the key as a bearer token in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Create and revoke keys under **API keys** in the app at https://app.algotradertools.com/api-keys.
  location: header
  name: API Key Bearer
  type: http-bearer
- evidence: 'If a tool can''t set the `Authorization` header but can set a custom one, send the key in `X-API-Key` instead:'
  header: X-API-Key
  how_to_obtain: Create and revoke keys under **API keys** in the app at https://app.algotradertools.com/api-keys.
  location: header
  name: API Key Header
  type: apiKey
slug: algotradertools-authentication
source_filename: algotradertools-authentication.yml
source_heading: Authentication Profile
source_url: https://algotradertools.com/docs/authentication.md
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://algotradertools.com/docs/authentication.md\nsources:\n- https://algotradertools.com/docs/authentication.md\n- https://algotradertools.com/docs/authentication\n- https://algotradertools.com/docs/quickstart\n- https://algotradertools.com/docs/authentication/index.md\ndescription: Authentication with API keys\nschemes:\n- type: http-bearer\n  name: API Key Bearer\n  evidence: 'Pass the key as a bearer token in the `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create and revoke keys under **API keys** in the app at https://app.algotradertools.com/api-keys.\n- type: apiKey\n  name: API Key Header\n  evidence: 'If a tool can''t set the `Authorization` header but can set a custom one, send the key in `X-API-Key` instead:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create and revoke keys under **API keys** in the app at https://app.algotradertools.com/api-keys.\n\
  note: No OAuth2, http-basic, jwt, hmac, mtls, or other schemes are documented.\ndocs: https://algotradertools.com/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/algotradertools/authentication/algotradertools-authentication.yml
summary_line: 2 schemes
tags:
- Trading
- Cloud
- MetaTrader
- Copy Trading
- Finance
---
