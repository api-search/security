---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lumail-io-campaigns-api-openapi.yml
  format: yaml
  label: Lumail Campaigns API
  slug: lumail-io-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-campaigns-api-openapi.yml
- filename: lumail-io-domains-api-openapi.yml
  format: yaml
  label: Lumail Domains API
  slug: lumail-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-domains-api-openapi.yml
- filename: lumail-io-email-api-openapi.yml
  format: yaml
  label: Lumail Email API
  slug: lumail-io-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-email-api-openapi.yml
- filename: lumail-io-events-api-openapi.yml
  format: yaml
  label: Lumail Events API
  slug: lumail-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-events-api-openapi.yml
- filename: lumail-io-subscribers-api-openapi.yml
  format: yaml
  label: Lumail Subscribers API
  slug: lumail-io-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-subscribers-api-openapi.yml
- filename: lumail-io-tags-api-openapi.yml
  format: yaml
  label: Lumail Tags API
  slug: lumail-io-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-tags-api-openapi.yml
- filename: lumail-io-verify-api-openapi.yml
  format: yaml
  label: Lumail Verify API
  slug: lumail-io-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-verify-api-openapi.yml
auth_types: []
description: Lumail API authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lumail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lumail declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lumail
provider_slug: lumail-io
scheme_count: 2
schemes:
- evidence: 'All API requests must include the token in the Authorization header using the Bearer authentication scheme: Authorization: Bearer lum_your_token_here'
  header: Authorization
  how_to_obtain: Create an API token in the Lumail dashboard (Settings → API Tokens) or via the CLI; the token format is lum_ followed by a 64‑character random string.
  location: header
  name: API Token
  type: http-bearer
- evidence: bearer_methods_supported:["header"]
  header: Authorization
  location: header
  name: OAuth2
  scopes:
  - openid
  - profile
  - email
  - offline_access
  - lumail.read
  - lumail.write
  - lumail.full
  token_url: https://lumail.io/api/auth
  type: oauth2
slug: lumail-io-authentication
source_filename: lumail-io-authentication.yml
source_heading: Authentication Profile
source_url: https://lumail.io/.well-known/oauth-protected-resource/mcp
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lumail.io/.well-known/oauth-protected-resource/mcp\nsources:\n- https://lumail.io/.well-known/oauth-protected-resource/mcp\n- https://lumail.io/docs/api-reference/api-tokens\n- https://lumail.io/docs/tutorials/create-api-token.md\n- https://lumail.io/docs/sdk/v2/tokens.md\ndescription: Lumail API authentication\nschemes:\n- type: http-bearer\n  name: API Token\n  evidence: 'All API requests must include the token in the Authorization header using the Bearer authentication scheme: Authorization: Bearer\n    lum_your_token_here'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API token in the Lumail dashboard (Settings → API Tokens) or via the CLI; the token format is lum_ followed by a 64‑character\n    random string.\n- type: oauth2\n  name: OAuth2\n  evidence: bearer_methods_supported:[\"header\"]\n  location: header\n  header: Authorization\n \
  \ token_url: https://lumail.io/api/auth\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  - lumail.read\n  - lumail.write\n  - lumail.full\ndocs: https://lumail.io/.well-known/oauth-protected-resource/mcp\n"
source_yaml_url: https://artifacts.apis.io/lumail-io/authentication/lumail-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Email Marketing
- Automation
- Software-as-a-Service
---
