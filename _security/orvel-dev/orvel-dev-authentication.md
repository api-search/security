---
anonymous_access: false
api_key_in: []
api_specs:
- filename: orvel-dev-e-invoicing-api-openapi.yml
  format: yaml
  label: orvel-dev E Invoicing API
  slug: orvel-dev-e-invoicing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orvel-dev/openapi/orvel-dev-e-invoicing-api-openapi.yml
- filename: orvel-dev-verification-api-openapi.yml
  format: yaml
  label: orvel-dev Verification API
  slug: orvel-dev-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orvel-dev/openapi/orvel-dev-verification-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Orvel Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: orvel-dev declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: orvel-dev
provider_slug: orvel-dev
scheme_count: 3
schemes:
- evidence: 'Authorization: Bearer fx.<your key>'
  header: Authorization
  how_to_obtain: Reveal the workspace's API‑key via the API‑key reveal button in the Factur‑X workspace and use it as a bearer token.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'The endpoint accepts either Authorization: Bearer YOUR_API_KEY or X-API-Key: YOUR_API_KEY . Both use the same key'
  header: X-API-Key
  how_to_obtain: Copy the API key from the workspace’s API‑key reveal button and supply it in the X‑API‑Key header (without the Bearer prefix).
  location: header
  name: X‑API‑Key header
  type: apiKey
- authorize_url: https://facturx.orvel.dev/mcp/account
  evidence: Add https://facturx.orvel.dev/mcp/account to an OAuth‑capable MCP client, select Authenticate, sign in and approve the connection.
  how_to_obtain: Use an OAuth‑capable client to initiate the flow at the /mcp/account endpoint, sign in with an Orvel account, and approve the connection to receive a token.
  name: MCP OAuth
  type: oauth2
slug: orvel-dev-authentication
source_filename: orvel-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://facturx.orvel.dev/docs/account/
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://facturx.orvel.dev/docs/account/\nsources:\n- https://facturx.orvel.dev/docs/account/\n- https://facturx.orvel.dev/docs/quickstart/\n- https://facturx.orvel.dev/docs/mcp/\n- https://facturx.orvel.dev/docs/fr/quickstart/\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Authorization: Bearer fx.<your key>'\n  location: header\n  header: Authorization\n  how_to_obtain: Reveal the workspace's API‑key via the API‑key reveal button in the Factur‑X workspace and use it as a bearer token.\n- type: apiKey\n  name: X‑API‑Key header\n  evidence: 'The endpoint accepts either Authorization: Bearer YOUR_API_KEY or X-API-Key: YOUR_API_KEY . Both use the same key'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Copy the API key from the workspace’s API‑key reveal button and supply it in the X‑API‑Key header (without the Bearer prefix).\n- type: oauth2\n  name:\
  \ MCP OAuth\n  evidence: Add https://facturx.orvel.dev/mcp/account to an OAuth‑capable MCP client, select Authenticate, sign in and approve the connection.\n  authorize_url: https://facturx.orvel.dev/mcp/account\n  how_to_obtain: Use an OAuth‑capable client to initiate the flow at the /mcp/account endpoint, sign in with an Orvel account, and approve the\n    connection to receive a token.\ndocs: https://facturx.orvel.dev/docs/account/\n"
source_yaml_url: https://artifacts.apis.io/orvel-dev/authentication/orvel-dev-authentication.yml
summary_line: 3 schemes
tags:
- e-invoicing
- accessibility
- API
- France
- EU
---
