---
anonymous_access: false
api_key_in: []
api_specs:
- filename: zespan-openapi-generated.yml
  format: yaml
  label: Zespan API
  slug: zespan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zespan/openapi/_ae-authored/zespan-openapi-generated.yml
auth_types: []
description: Authentication methods for Zespan APIs and CLI
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Zespan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zespan declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Zespan
provider_slug: zespan
scheme_count: 2
schemes:
- evidence: The SDK sends this key as an `x-api-key` header on requests to the ingest API. If you're calling Zespan's API directly rather than through the SDK, set the same header yourself.
  header: x-api-key
  how_to_obtain: Create and manage project API keys from the project's Settings → API Keys page in the Zespan dashboard. The key is shown in full only once at creation.
  location: header
  name: Project API key
  type: apiKey
- evidence: 'It starts with `lqtp_` and is sent as a Bearer token:'
  header: Authorization
  how_to_obtain: Generate and revoke personal API keys from your account settings in the Zespan dashboard.
  location: header
  name: Personal API key
  type: http-bearer
slug: zespan-authentication
source_filename: zespan-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.zespan.com/account/api-keys.md
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.zespan.com/account/api-keys.md\nsources:\n- https://docs.zespan.com/account/api-keys.md\n- https://docs.zespan.com/api-reference/sdk-cli-support/resolve-project-identity-from-an-api-key.md\n- https://docs.zespan.com/cli/auth.md\n- https://docs.zespan.com/quickstart.md\ndescription: Authentication methods for Zespan APIs and CLI\nschemes:\n- type: apiKey\n  name: Project API key\n  evidence: The SDK sends this key as an `x-api-key` header on requests to the ingest API. If you're calling Zespan's API directly rather than\n    through the SDK, set the same header yourself.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create and manage project API keys from the project's Settings → API Keys page in the Zespan dashboard. The key is shown in full\n    only once at creation.\n- type: http-bearer\n  name: Personal API key\n  evidence: 'It starts with `lqtp_` and\
  \ is sent as a Bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate and revoke personal API keys from your account settings in the Zespan dashboard.\nnote: OAuth 2.0 device grant is used by the Zespan CLI for user login, but the documentation does not provide token or authorize URLs, so no OAuth\n  flow entry is included.\ndocs: https://docs.zespan.com/account/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/zespan/authentication/zespan-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Monitoring
- Reliability
- Agents
- Platform
---
