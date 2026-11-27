---
anonymous_access: false
api_key_in: []
api_specs:
- filename: iterant-ai-public-brands-api-openapi.yml
  format: yaml
  label: 'Iterant Public: Brands API'
  slug: iterant-ai-public-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iterant-ai/openapi/iterant-ai-public-brands-api-openapi.yml
- filename: iterant-ai-public-linking-api-openapi.yml
  format: yaml
  label: 'Iterant Public: Linking API'
  slug: iterant-ai-public-linking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iterant-ai/openapi/iterant-ai-public-linking-api-openapi.yml
- filename: iterant-ai-public-opportunities-api-openapi.yml
  format: yaml
  label: 'Iterant Public: Opportunities API'
  slug: iterant-ai-public-opportunities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iterant-ai/openapi/iterant-ai-public-opportunities-api-openapi.yml
- filename: iterant-ai-public-pages-api-openapi.yml
  format: yaml
  label: 'Iterant Public: Pages API'
  slug: iterant-ai-public-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iterant-ai/openapi/iterant-ai-public-pages-api-openapi.yml
- filename: iterant-ai-public-reports-api-openapi.yml
  format: yaml
  label: 'Iterant Public: Reports API'
  slug: iterant-ai-public-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iterant-ai/openapi/iterant-ai-public-reports-api-openapi.yml
- filename: iterant-ai-public-tasks-api-openapi.yml
  format: yaml
  label: 'Iterant Public: Tasks API'
  slug: iterant-ai-public-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iterant-ai/openapi/iterant-ai-public-tasks-api-openapi.yml
- filename: iterant-ai-public-visibility-api-openapi.yml
  format: yaml
  label: 'Iterant Public: Visibility API'
  slug: iterant-ai-public-visibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iterant-ai/openapi/iterant-ai-public-visibility-api-openapi.yml
auth_types: []
description: 'Iterant supports two authentication schemes: OAuth 2.1 with PKCE for interactive users and an itr_ API key for headless callers.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Iterant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Iterant declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Iterant
provider_slug: iterant-ai
scheme_count: 2
schemes:
- evidence: Interactive client acting for a person (Claude Code, Claude Desktop, Cursor, VS Code) | OAuth 2.1 with PKCE
  header: Authorization
  how_to_obtain: Register via Dynamic Client Registration at the authorization server's registration_endpoint; then run the standard authorization code flow with PKCE (S256) and request offline_access for a refresh token.
  location: header
  name: OAuth 2.1 with PKCE
  type: oauth2
- evidence: Headless job (CI, n8n, a script) | `itr_` API key
  header: Authorization
  how_to_obtain: An organization admin mints a key in Settings → Developers in the Iterant dashboard; the key is shown once and must be copied and stored securely.
  location: header
  name: itr_ API key
  type: apiKey
slug: iterant-ai-authentication
source_filename: iterant-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://iterant.ai/auth.md
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://iterant.ai/auth.md\nsources:\n- https://iterant.ai/auth.md\n- https://iterant.ai/docs/developers/api-keys\n- https://iterant.ai/docs/getting-started/overview\n- https://iterant.ai/docs/getting-started/core-concepts\ndescription: 'Iterant supports two authentication schemes: OAuth 2.1 with PKCE for interactive users and an itr_ API key for headless callers.'\nschemes:\n- type: oauth2\n  name: OAuth 2.1 with PKCE\n  evidence: Interactive client acting for a person (Claude Code, Claude Desktop, Cursor, VS Code) | OAuth 2.1 with PKCE\n  location: header\n  header: Authorization\n  how_to_obtain: Register via Dynamic Client Registration at the authorization server's registration_endpoint; then run the standard authorization\n    code flow with PKCE (S256) and request offline_access for a refresh token.\n- type: apiKey\n  name: itr_ API key\n  evidence: Headless job (CI, n8n,\
  \ a script) | `itr_` API key\n  location: header\n  header: Authorization\n  how_to_obtain: An organization admin mints a key in Settings → Developers in the Iterant dashboard; the key is shown once and must be copied\n    and stored securely.\ndocs: https://iterant.ai/auth.md\n"
source_yaml_url: https://artifacts.apis.io/iterant-ai/authentication/iterant-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- SEO
- Marketing
- Automation
- Amsterdam
- Company
---
