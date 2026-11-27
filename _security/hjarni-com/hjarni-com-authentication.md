---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hjarni-com-containers-api-openapi.yml
  format: yaml
  label: Hjarni Containers API
  slug: hjarni-com-containers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hjarni-com/openapi/hjarni-com-containers-api-openapi.yml
- filename: hjarni-com-dashboard-api-openapi.yml
  format: yaml
  label: Hjarni Dashboard API
  slug: hjarni-com-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hjarni-com/openapi/hjarni-com-dashboard-api-openapi.yml
- filename: hjarni-com-files-api-openapi.yml
  format: yaml
  label: Hjarni Files API
  slug: hjarni-com-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hjarni-com/openapi/hjarni-com-files-api-openapi.yml
- filename: hjarni-com-me-api-openapi.yml
  format: yaml
  label: Hjarni Me API
  slug: hjarni-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hjarni-com/openapi/hjarni-com-me-api-openapi.yml
- filename: hjarni-com-notes-api-openapi.yml
  format: yaml
  label: Hjarni Notes API
  slug: hjarni-com-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hjarni-com/openapi/hjarni-com-notes-api-openapi.yml
- filename: hjarni-com-search-api-openapi.yml
  format: yaml
  label: Hjarni Search API
  slug: hjarni-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hjarni-com/openapi/hjarni-com-search-api-openapi.yml
- filename: hjarni-com-tags-api-openapi.yml
  format: yaml
  label: Hjarni Tags API
  slug: hjarni-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hjarni-com/openapi/hjarni-com-tags-api-openapi.yml
auth_types: []
description: Authentication methods for Hjarni
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hjarni Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hjarni declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hjarni
provider_slug: hjarni-com
scheme_count: 1
schemes:
- evidence: Authorization Code flow with PKCE
  flows:
  - authorization_code
  name: OAuth
  type: oauth2
slug: hjarni-com-authentication
source_filename: hjarni-com-authentication.yml
source_heading: Authentication Profile
source_url: https://hjarni.com/docs/two-factor-authentication.md
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hjarni.com/docs/two-factor-authentication.md\nsources:\n- https://hjarni.com/docs/two-factor-authentication.md\n- https://hjarni.com/mcp-fix/claude-code-mcp-oauth-loop.md\n- https://hjarni.com/docs/two-factor-authentication\n- https://hjarni.com/docs/mcp\ndescription: Authentication methods for Hjarni\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Authorization Code flow with PKCE\n  flows:\n  - authorization_code\ndocs: https://hjarni.com/docs/two-factor-authentication.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/hjarni-com/authentication/hjarni-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Memory
- Knowledge Base
- Integration
---
