---
anonymous_access: false
api_key_in: []
api_specs:
- filename: duneanalytics-com-openapi-generated.yml
  format: yaml
  label: Dune Analytics API
  slug: duneanalytics-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duneanalytics-com/openapi/_ae-authored/duneanalytics-com-openapi-generated.yml
auth_types: []
description: The Dune API uses API keys for authentication.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Duneanalytics Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dune Analytics declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Dune Analytics
provider_slug: duneanalytics-com
scheme_count: 2
schemes:
- evidence: To authenticate via the API header, include an `x-dune-api-key` property in your request header.
  header: X-DUNE-API-KEY
  how_to_obtain: Generate an API key in Dune settings → API → create new API key.
  location: header
  name: x-dune-api-key
  type: apiKey
- evidence: Alternatively, use an `api_key` query parameter for authentication.
  how_to_obtain: Generate an API key in Dune settings → API → create new API key.
  location: query
  name: api_key
  type: apiKey
slug: duneanalytics-com-authentication
source_filename: duneanalytics-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.dune.com/api-reference/overview/authentication.md
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.dune.com/api-reference/overview/authentication.md\nsources:\n- https://docs.dune.com/api-reference/overview/authentication.md\n- https://docs.dune.com/web-app/okta-sso.md\n- https://docs.dune.com/api-reference/connectors/dbt/getting-started.md\n- https://docs.dune.com/datashare/datashare-trial.md\ndescription: The Dune API uses API keys for authentication.\nschemes:\n- type: apiKey\n  name: x-dune-api-key\n  evidence: To authenticate via the API header, include an `x-dune-api-key` property in your request header.\n  location: header\n  header: X-DUNE-API-KEY\n  how_to_obtain: Generate an API key in Dune settings → API → create new API key.\n- type: apiKey\n  name: api_key\n  evidence: Alternatively, use an `api_key` query parameter for authentication.\n  location: query\n  how_to_obtain: Generate an API key in Dune settings → API → create new API key.\nnote: No OAuth2,\
  \ HTTP basic, bearer, JWT, HMAC, or mTLS schemes are documented.\ndocs: https://docs.dune.com/api-reference/overview/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/duneanalytics-com/authentication/duneanalytics-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Blockchain
- Data
- Analytics
- Crypto
---
