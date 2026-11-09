---
anonymous_access: false
api_key_in: []
api_specs:
- filename: steamgpt-net-bans-api-openapi.yml
  format: yaml
  label: steamgpt-net Bans API
  slug: steamgpt-net-bans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-bans-api-openapi.yml
- filename: steamgpt-net-batch-api-openapi.yml
  format: yaml
  label: steamgpt-net Batch API
  slug: steamgpt-net-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-batch-api-openapi.yml
- filename: steamgpt-net-compare-api-openapi.yml
  format: yaml
  label: steamgpt-net Compare API
  slug: steamgpt-net-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-compare-api-openapi.yml
- filename: steamgpt-net-converter-api-openapi.yml
  format: yaml
  label: steamgpt-net Converter API
  slug: steamgpt-net-converter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-converter-api-openapi.yml
- filename: steamgpt-net-faceit-api-openapi.yml
  format: yaml
  label: steamgpt-net Faceit API
  slug: steamgpt-net-faceit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-faceit-api-openapi.yml
- filename: steamgpt-net-friends-api-openapi.yml
  format: yaml
  label: steamgpt-net Friends API
  slug: steamgpt-net-friends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-friends-api-openapi.yml
- filename: steamgpt-net-identity-api-openapi.yml
  format: yaml
  label: steamgpt-net Identity API
  slug: steamgpt-net-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-identity-api-openapi.yml
- filename: steamgpt-net-profile-api-openapi.yml
  format: yaml
  label: steamgpt-net Profile API
  slug: steamgpt-net-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-profile-api-openapi.yml
- filename: steamgpt-net-ready-api-openapi.yml
  format: yaml
  label: steamgpt-net Ready API
  slug: steamgpt-net-ready-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-ready-api-openapi.yml
- filename: steamgpt-net-summary-api-openapi.yml
  format: yaml
  label: steamgpt-net Summary API
  slug: steamgpt-net-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-summary-api-openapi.yml
auth_types: []
description: Optional self‑service boost token obtained via client_credentials grant
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Steamgpt Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: steamgpt-net declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: steamgpt-net
provider_slug: steamgpt-net
scheme_count: 1
schemes:
- evidence: An optional self‑service token - one POST, no humans in the loop - raises the rate limit.
  flows:
  - client_credentials
  how_to_obtain: POST https://steamgpt.net/oauth/token with body grant_type=client_credentials (no client authentication). The response contains an access_token (Bearer JWT).
  name: Boost Token
  scopes:
  - rate-boost
  token_url: https://steamgpt.net/oauth/token
  type: oauth2
slug: steamgpt-net-authentication
source_filename: steamgpt-net-authentication.yml
source_heading: Authentication Profile
source_url: https://steamgpt.net/auth.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://steamgpt.net/auth.md\nsources:\n- https://steamgpt.net/auth.md\ndescription: Optional self‑service boost token obtained via client_credentials grant\nschemes:\n- type: oauth2\n  name: Boost Token\n  evidence: An optional self‑service token - one POST, no humans in the loop - raises the rate limit.\n  flows:\n  - client_credentials\n  token_url: https://steamgpt.net/oauth/token\n  scopes:\n  - rate-boost\n  how_to_obtain: POST https://steamgpt.net/oauth/token with body grant_type=client_credentials (no client authentication). The response contains\n    an access_token (Bearer JWT).\ndocs: https://steamgpt.net/auth.md\n"
source_yaml_url: https://artifacts.apis.io/steamgpt-net/authentication/steamgpt-net-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Gaming
- Steam
---
