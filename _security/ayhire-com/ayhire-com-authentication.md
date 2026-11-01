---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ayhire-com-account-api-openapi.yml
  format: yaml
  label: ayhire-com Account API
  slug: ayhire-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayhire-com/openapi/ayhire-com-account-api-openapi.yml
- filename: ayhire-com-company-maps-api-openapi.yml
  format: yaml
  label: ayhire-com Company maps API
  slug: ayhire-com-company-maps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayhire-com/openapi/ayhire-com-company-maps-api-openapi.yml
- filename: ayhire-com-integrations-api-openapi.yml
  format: yaml
  label: ayhire-com Integrations API
  slug: ayhire-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayhire-com/openapi/ayhire-com-integrations-api-openapi.yml
- filename: ayhire-com-people-api-openapi.yml
  format: yaml
  label: ayhire-com People API
  slug: ayhire-com-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayhire-com/openapi/ayhire-com-people-api-openapi.yml
- filename: ayhire-com-research-api-openapi.yml
  format: yaml
  label: ayhire-com Research API
  slug: ayhire-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayhire-com/openapi/ayhire-com-research-api-openapi.yml
- filename: ayhire-com-roles-api-openapi.yml
  format: yaml
  label: ayhire-com Roles API
  slug: ayhire-com-roles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayhire-com/openapi/ayhire-com-roles-api-openapi.yml
- filename: ayhire-com-watching-api-openapi.yml
  format: yaml
  label: ayhire-com Watching API
  slug: ayhire-com-watching-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayhire-com/openapi/ayhire-com-watching-api-openapi.yml
- filename: ayhire-com-workspaces-api-openapi.yml
  format: yaml
  label: ayhire-com Workspaces API
  slug: ayhire-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayhire-com/openapi/ayhire-com-workspaces-api-openapi.yml
auth_types: []
description: AyHire authenticates API requests using a bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ayhire Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ayhire-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ayhire-com
provider_slug: ayhire-com
scheme_count: 1
schemes:
- evidence: 'Add an MCP server named `ayhire`: URL `https://ayhire.com/api/mcp`, streamable HTTP, header `Authorization: Bearer <key>`.'
  header: Authorization
  how_to_obtain: User signs in once in a browser (https://ayhire.com/auth/sign‑in) which stores an API key locally; the key is then used as a Bearer token.
  location: header
  name: AyHire API key
  type: http-bearer
slug: ayhire-com-authentication
source_filename: ayhire-com-authentication.yml
source_heading: Authentication Profile
source_url: https://ayhire.com/setup.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ayhire.com/setup.md\nsources:\n- https://ayhire.com/setup.md\ndescription: AyHire authenticates API requests using a bearer token.\nschemes:\n- type: http-bearer\n  name: AyHire API key\n  evidence: 'Add an MCP server named `ayhire`: URL `https://ayhire.com/api/mcp`, streamable HTTP, header `Authorization: Bearer <key>`.'\n  location: header\n  header: Authorization\n  how_to_obtain: User signs in once in a browser (https://ayhire.com/auth/sign‑in) which stores an API key locally; the key is then used as a\n    Bearer token.\nnote: No OAuth2, apiKey, or other authentication methods are documented.\ndocs: https://ayhire.com/setup.md\n"
source_yaml_url: https://artifacts.apis.io/ayhire-com/authentication/ayhire-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Hiring
- DeveloperTools
- Recruitment
- OpenSource
---
