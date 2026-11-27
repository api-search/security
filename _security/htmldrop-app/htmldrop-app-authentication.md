---
anonymous_access: false
api_key_in: []
api_specs:
- filename: htmldrop-app-openapi-generated.yml
  format: yaml
  label: htmldrop API
  slug: htmldrop-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/htmldrop-app/openapi/_ae-authored/htmldrop-app-openapi-generated.yml
auth_types: []
description: Authentication methods for htmldrop API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: htmldrop Authentication
name_suffix: Authentication
oauth_flows: []
overview: htmldrop declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: htmldrop
provider_slug: htmldrop-app
scheme_count: 2
schemes:
- evidence: "curl https://htmldrop.app/api/v1/sites \n  -H \"Authorization: Bearer $HTMLDROP_API_TOKEN\""
  header: Authorization
  how_to_obtain: Create one at Dashboard → Settings → API tokens; tokens look like `hsk_live_…` and are shown once.
  location: header
  name: API token
  type: http-bearer
- evidence: 'The server implements OAuth 2.1 with PKCE and dynamic client registration, so a compliant client discovers everything it needs:'
  how_to_obtain: Discover endpoints via https://htmldrop.app/.well-known/oauth-authorization-server and https://htmldrop.app/.well-known/oauth-protected-resource; approve in the browser and the client stores and refreshes tokens.
  name: OAuth
  scopes:
  - mcp
  - cli
  type: oauth2
slug: htmldrop-app-authentication
source_filename: htmldrop-app-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.htmldrop.app/api/authentication.md
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.htmldrop.app/api/authentication.md\nsources:\n- https://docs.htmldrop.app/api/authentication.md\n- https://docs.htmldrop.app/quickstart.md\ndescription: Authentication methods for htmldrop API\nschemes:\n- type: http-bearer\n  name: API token\n  evidence: \"curl https://htmldrop.app/api/v1/sites \\n  -H \\\"Authorization: Bearer $HTMLDROP_API_TOKEN\\\"\"\n  location: header\n  header: Authorization\n  how_to_obtain: Create one at Dashboard → Settings → API tokens; tokens look like `hsk_live_…` and are shown once.\n- type: oauth2\n  name: OAuth\n  evidence: 'The server implements OAuth 2.1 with PKCE and dynamic client registration, so a compliant client discovers everything it needs:'\n  scopes:\n  - mcp\n  - cli\n  how_to_obtain: Discover endpoints via https://htmldrop.app/.well-known/oauth-authorization-server and https://htmldrop.app/.well-known/oauth-protected-resource;\n\
  \    approve in the browser and the client stores and refreshes tokens.\ndocs: https://docs.htmldrop.app/api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/htmldrop-app/authentication/htmldrop-app-authentication.yml
summary_line: 2 schemes
tags:
- File Hosting
- HTML
- Markdown
- URL Shorteners
- Developer Tools
---
