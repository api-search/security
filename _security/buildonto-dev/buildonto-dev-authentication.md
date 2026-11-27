---
anonymous_access: false
api_key_in: []
api_specs:
- filename: buildonto-dev-batch-api-openapi.yml
  format: yaml
  label: Onto Batch API
  slug: buildonto-dev-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-batch-api-openapi.yml
- filename: buildonto-dev-extract-api-openapi.yml
  format: yaml
  label: Onto Extract API
  slug: buildonto-dev-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-extract-api-openapi.yml
- filename: buildonto-dev-map-api-openapi.yml
  format: yaml
  label: Onto Map API
  slug: buildonto-dev-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-map-api-openapi.yml
- filename: buildonto-dev-read-api-openapi.yml
  format: yaml
  label: Onto Read API
  slug: buildonto-dev-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-read-api-openapi.yml
- filename: buildonto-dev-read-score-api-openapi.yml
  format: yaml
  label: Onto Read + Score API
  slug: buildonto-dev-read-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-read-score-api-openapi.yml
- filename: buildonto-dev-score-api-openapi.yml
  format: yaml
  label: Onto Score API
  slug: buildonto-dev-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-score-api-openapi.yml
- filename: buildonto-dev-usage-api-openapi.yml
  format: yaml
  label: Onto Usage API
  slug: buildonto-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-usage-api-openapi.yml
auth_types: []
description: Onto uses Bearer tokens for its Read API and an OAuth2 authorization code flow (PKCE) for the Remote connector.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Onto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Onto declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Onto
provider_slug: buildonto-dev
scheme_count: 2
schemes:
- evidence: Every Read API request needs a Bearer token in the Authorization header.
  header: Authorization
  how_to_obtain: Sign in at https://app.buildonto.dev, go to /read/keys and copy the displayed key (onto_sk_live_...).
  location: header
  name: Read API key
  type: http-bearer
- authorize_url: https://api.buildonto.dev/authorize
  evidence: One URL — https://api.buildonto.dev/mcp — and a sign‑in with your Onto account. No key to paste, nothing to install.
  flows:
  - authorization_code
  how_to_obtain: Run the client’s add command (e.g., $ claude mcp add --scope user --transport http onto https://api.buildonto.dev/mcp); the client will be redirected to Onto’s sign‑in page, approve the request, and receive an access token via the PKCE authorization‑code flow.
  name: Remote connector (OAuth)
  scopes:
  - onto:read
  type: oauth2
slug: buildonto-dev-authentication
source_filename: buildonto-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.buildonto.dev/api/auth.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.buildonto.dev/api/auth.md\nsources:\n- https://docs.buildonto.dev/api/auth.md\n- https://docs.buildonto.dev/mcp/remote.md\n- https://docs.buildonto.dev/quickstart.md\n- https://docs.buildonto.dev/mcp/setup.md\ndescription: Onto uses Bearer tokens for its Read API and an OAuth2 authorization code flow (PKCE) for the Remote connector.\nschemes:\n- type: http-bearer\n  name: Read API key\n  evidence: Every Read API request needs a Bearer token in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in at https://app.buildonto.dev, go to /read/keys and copy the displayed key (onto_sk_live_...).\n- type: oauth2\n  name: Remote connector (OAuth)\n  evidence: One URL — https://api.buildonto.dev/mcp — and a sign‑in with your Onto account. No key to paste, nothing to install.\n  flows:\n  - authorization_code\n  authorize_url: https://api.buildonto.dev/authorize\n\
  \  scopes:\n  - onto:read\n  how_to_obtain: Run the client’s add command (e.g., $ claude mcp add --scope user --transport http onto https://api.buildonto.dev/mcp); the client\n    will be redirected to Onto’s sign‑in page, approve the request, and receive an access token via the PKCE authorization‑code flow.\ndocs: https://docs.buildonto.dev/api/auth.md\n"
source_yaml_url: https://artifacts.apis.io/buildonto-dev/authentication/buildonto-dev-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Content
- Markdown
- Read API
- Platform
---
