---
anonymous_access: false
api_key_in: []
api_specs:
- filename: offlinecreatorstudio-com-agent-api-openapi.yml
  format: yaml
  label: OfflineCreator Studio Agent API
  slug: offlinecreatorstudio-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/offlinecreatorstudio-com/openapi/offlinecreatorstudio-com-agent-api-openapi.yml
- filename: offlinecreatorstudio-com-generations-api-openapi.yml
  format: yaml
  label: OfflineCreator Studio Generations API
  slug: offlinecreatorstudio-com-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/offlinecreatorstudio-com/openapi/offlinecreatorstudio-com-generations-api-openapi.yml
auth_types: []
description: Authentication methods for OfflineCreator Studio MCP clients
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: OfflineCreator Studio Authentication
name_suffix: Authentication
oauth_flows: []
overview: OfflineCreator Studio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: OfflineCreator Studio
provider_slug: offlinecreatorstudio-com
scheme_count: 2
schemes:
- evidence: 'Send a legacy remote key in the Authorization header A remote fallback needs a client that can attach `Authorization: Bearer <API key>` to requests for `https://offlinecreatorstudio.com/mcp`.'
  header: Authorization
  how_to_obtain: 'Create a personal API key in Studio Settings and provide it to the client via an environment variable or configuration that injects `Authorization: Bearer <API key>` on each request.'
  name: Legacy API‑key Bearer Header
  scopes:
  - models
  - read
  - generate
  type: http-bearer
- evidence: For the plain CLI and local stdio package, OfflineCreator requires a personal key in the `OFFLINECREATOR_API_KEY` process environment.
  header: Authorization
  how_to_obtain: Export `OFFLINECREATOR_API_KEY` with the personal API key value in the shell that runs the CLI; the CLI sends it as a Bearer token in the HTTP Authorization header.
  name: CLI Environment Variable Bearer Token
  scopes:
  - models
  - read
  - generate
  type: http-bearer
slug: offlinecreatorstudio-com-authentication
source_filename: offlinecreatorstudio-com-authentication.yml
source_heading: Authentication Profile
source_url: https://offlinecreatorstudio.com/solutions/oauth-mcp-image-generator
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://offlinecreatorstudio.com/solutions/oauth-mcp-image-generator\nsources:\n- https://offlinecreatorstudio.com/solutions/oauth-mcp-image-generator\n- https://offlinecreatorstudio.com/integrations/remote-oauth-mcp-client-setup\n- https://offlinecreatorstudio.com/integrations/api-key-mcp-client-fallback\n- https://offlinecreatorstudio.com/cli/cli-authentication\ndescription: Authentication methods for OfflineCreator Studio MCP clients\nschemes:\n- type: http-bearer\n  name: Legacy API‑key Bearer Header\n  evidence: 'Send a legacy remote key in the Authorization header A remote fallback needs a client that can attach `Authorization: Bearer <API\n    key>` to requests for `https://offlinecreatorstudio.com/mcp`.'\n  header: Authorization\n  scopes:\n  - models\n  - read\n  - generate\n  how_to_obtain: 'Create a personal API key in Studio Settings and provide it to the client via\
  \ an environment variable or configuration that\n    injects `Authorization: Bearer <API key>` on each request.'\n- type: http-bearer\n  name: CLI Environment Variable Bearer Token\n  evidence: For the plain CLI and local stdio package, OfflineCreator requires a personal key in the `OFFLINECREATOR_API_KEY` process environment.\n  header: Authorization\n  scopes:\n  - models\n  - read\n  - generate\n  how_to_obtain: Export `OFFLINECREATOR_API_KEY` with the personal API key value in the shell that runs the CLI; the CLI sends it as a Bearer\n    token in the HTTP Authorization header.\ndocs: https://offlinecreatorstudio.com/solutions/oauth-mcp-image-generator\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/offlinecreatorstudio-com/authentication/offlinecreatorstudio-com-authentication.yml
summary_line: 2 schemes
tags:
- AI Image Generation
- AI Video Generation
- AI 3D Generation
- cloud AI routing
- offline generation
---
