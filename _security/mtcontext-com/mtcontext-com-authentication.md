---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mtcontext-com-openapi-generated.yml
  format: yaml
  label: MTContext API
  slug: mtcontext-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mtcontext-com/openapi/_ae-authored/mtcontext-com-openapi-generated.yml
auth_types: []
description: Authentication for MTContext uses HTTP Bearer tokens sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: MTContext Authentication
name_suffix: Authentication
oauth_flows: []
overview: MTContext declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MTContext
provider_slug: mtcontext-com
scheme_count: 2
schemes:
- evidence: 'Your client sends it as Authorization: Bearer MTMCP-YOUR-TERMINAL-KEY , exactly.'
  header: Authorization
  how_to_obtain: Generate a terminal key in the MTContext dashboard (Dashboard → Generate a Terminal Key). The key must start with "MTMCP-".
  location: header
  name: Terminal Key Bearer
  type: http-bearer
- evidence: 'Every request needs an Authorization: Bearer <token> header. You can use either: API key (recommended): a mtmcp_api_ -prefixed key.'
  header: Authorization
  how_to_obtain: Create an API key in the MTContext dashboard (Dashboard → API Keys). The key is prefixed with "mtmcp_api_".
  location: header
  name: API Key Bearer
  type: http-bearer
slug: mtcontext-com-authentication
source_filename: mtcontext-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.mtcontext.com/docs/tools/api-token
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.mtcontext.com/docs/tools/api-token\nsources:\n- https://docs.mtcontext.com/docs/tools/api-token\n- https://help.mtcontext.com/hc/knowledge-base/articles/metatrader-mcp-auth-errors-expired-token\n- https://docs.mtcontext.com/docs/setup\n- https://docs.mtcontext.com/docs/api\ndescription: Authentication for MTContext uses HTTP Bearer tokens sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Terminal Key Bearer\n  evidence: 'Your client sends it as Authorization: Bearer MTMCP-YOUR-TERMINAL-KEY , exactly.'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a terminal key in the MTContext dashboard (Dashboard → Generate a Terminal Key). The key must start with \"MTMCP-\".\n- type: http-bearer\n  name: API Key Bearer\n  evidence: 'Every request needs an Authorization: Bearer <token> header. You can use either: API key (recommended):\
  \ a mtmcp_api_ -prefixed key.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the MTContext dashboard (Dashboard → API Keys). The key is prefixed with \"mtmcp_api_\".\nnote: Both schemes require the token to be placed in the Authorization header as a Bearer token.\ndocs: https://docs.mtcontext.com/docs/tools/api-token\n"
source_yaml_url: https://artifacts.apis.io/mtcontext-com/authentication/mtcontext-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Trading
- Artificial Intelligence
- MetaTrader
- MCP
- Automation
---
