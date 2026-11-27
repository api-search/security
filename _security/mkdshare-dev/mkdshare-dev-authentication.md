---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mkdshare-dev-openapi-generated.yml
  format: yaml
  label: mkdshare.DEV API
  slug: mkdshare-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mkdshare-dev/openapi/_ae-authored/mkdshare-dev-openapi-generated.yml
auth_types: []
description: Authentication for mkdshare.DEV MCP API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: mkdshare.DEV Authentication
name_suffix: Authentication
oauth_flows: []
overview: mkdshare.DEV declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mkdshare.DEV
provider_slug: mkdshare-dev
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer <your-token>'
  header: Authorization
  how_to_obtain: Get yours at mkdshare.dev/api-access after signing in.
  location: header
  name: Bearer
  type: http-bearer
slug: mkdshare-dev-authentication
source_filename: mkdshare-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://mkdshare.dev/docs/mcp
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mkdshare.dev/docs/mcp\nsources:\n- https://mkdshare.dev/docs/mcp\ndescription: Authentication for mkdshare.DEV MCP API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization: Bearer <your-token>'\n  location: header\n  header: Authorization\n  how_to_obtain: Get yours at mkdshare.dev/api-access after signing in.\ndocs: https://mkdshare.dev/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/mkdshare-dev/authentication/mkdshare-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
