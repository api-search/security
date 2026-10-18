---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cloudidr-external-api-openapi.yml
  format: yaml
  label: Cloudidr External API
  slug: cloudidr-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudidr/refs/heads/main/openapi/cloudidr-external-api-openapi.yml
auth_types: []
description: Authentication methods for Cloudidr APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cloudidr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudidr declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cloudidr
provider_slug: cloudidr
scheme_count: 2
schemes:
- evidence: Cloudidr API Key is required in the API calls with "X-Cloudidr-Key"
  header: X-Cloudidr-Key
  how_to_obtain: Create and manage API keys under the **My Keys** tab in Settings; keys start with prefix **trk_**
  location: header
  name: X-Cloudidr-Key
  type: apiKey
- evidence: Authenticate and obtain an access token (JWT) for API requests. The access token must be included in the Authorization header as 'Bearer <token>' for all subsequent API calls.
  header: Authorization
  how_to_obtain: POST to https://public-api.cloudidr.com/external/api/v1/sign‑in with JSON body containing "username" and "password" to receive a JWT access token
  location: header
  name: bearerAuth
  type: http-bearer
slug: cloudidr-authentication
source_filename: cloudidr-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cloudidr.com/guides/llm-ops/api-keys.md
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cloudidr.com/guides/llm-ops/api-keys.md\nsources:\n- https://docs.cloudidr.com/guides/llm-ops/api-keys.md\n- https://docs.cloudidr.com/api-reference/auth-api.json\n- https://docs.cloudidr.com/guides/llm-ops/getting-started.md\n- https://docs.cloudidr.com/guides/flex-compute/getting-started.md\ndescription: Authentication methods for Cloudidr APIs\nschemes:\n- type: apiKey\n  name: X-Cloudidr-Key\n  evidence: Cloudidr API Key is required in the API calls with \"X-Cloudidr-Key\"\n  location: header\n  header: X-Cloudidr-Key\n  how_to_obtain: Create and manage API keys under the **My Keys** tab in Settings; keys start with prefix **trk_**\n- type: http-bearer\n  name: bearerAuth\n  evidence: Authenticate and obtain an access token (JWT) for API requests. The access token must be included in the Authorization header as 'Bearer\n    <token>' for all subsequent API calls.\n\
  \  location: header\n  header: Authorization\n  how_to_obtain: POST to https://public-api.cloudidr.com/external/api/v1/sign‑in with JSON body containing \"username\" and \"password\" to receive\n    a JWT access token\ndocs: https://docs.cloudidr.com/guides/llm-ops/api-keys.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudidr/refs/heads/main/authentication/cloudidr-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Identity and Access Management
- Cloud
- Security
- Artificial Intelligence
- FinOps
---
