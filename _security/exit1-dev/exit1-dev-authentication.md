---
anonymous_access: false
api_key_in: []
api_specs:
- filename: exit1-dev-checks-api-openapi.yml
  format: yaml
  label: Exit1.dev Checks API
  slug: exit1-dev-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exit1-dev/openapi/exit1-dev-checks-api-openapi.yml
- filename: exit1-dev-history-api-openapi.yml
  format: yaml
  label: Exit1.dev History API
  slug: exit1-dev-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exit1-dev/openapi/exit1-dev-history-api-openapi.yml
- filename: exit1-dev-statistics-api-openapi.yml
  format: yaml
  label: Exit1.dev Statistics API
  slug: exit1-dev-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exit1-dev/openapi/exit1-dev-statistics-api-openapi.yml
auth_types: []
description: Authentication schemes for exit1.dev API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Exit1.dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exit1.dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Exit1.dev
provider_slug: exit1-dev
scheme_count: 2
schemes:
- evidence: API keys , sent in the X-Api-Key header.
  header: X-Api-Key
  how_to_obtain: Create a key via Settings > API, select scopes, optionally set expiry or restrictions, then copy the generated key.
  location: header
  name: API Key
  type: apiKey
- evidence: 'Bearer tokens , sent as Authorization: Bearer <token> . An AI agent gets one by signing its user up with POST https://app.exit1.dev/oauth/agent-signup .'
  header: Authorization
  how_to_obtain: Obtain a token by signing up an AI agent with POST https://app.exit1.dev/oauth/agent-signup.
  location: header
  name: Bearer token
  token_url: https://app.exit1.dev/oauth/agent-signup
  type: http-bearer
slug: exit1-dev-authentication
source_filename: exit1-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.exit1.dev/api-reference/authentication
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.exit1.dev/api-reference/authentication\nsources:\n- https://docs.exit1.dev/api-reference/authentication\n- https://docs.exit1.dev/getting-started\n- https://docs.exit1.dev/getting-started/creating-your-account\n- https://docs.exit1.dev/getting-started/your-first-check\ndescription: Authentication schemes for exit1.dev API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: API keys , sent in the X-Api-Key header.\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Create a key via Settings > API, select scopes, optionally set expiry or restrictions, then copy the generated key.\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Bearer tokens , sent as Authorization: Bearer <token> . An AI agent gets one by signing its user up with POST https://app.exit1.dev/oauth/agent-signup\n    .'\n  location: header\n  header: Authorization\n  token_url: https://app.exit1.dev/oauth/agent-signup\n\
  \  how_to_obtain: Obtain a token by signing up an AI agent with POST https://app.exit1.dev/oauth/agent-signup.\ndocs: https://docs.exit1.dev/api-reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/exit1-dev/authentication/exit1-dev-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Monitoring
- Uptime
- Free
---
