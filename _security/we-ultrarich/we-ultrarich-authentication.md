---
api_key_in: []
api_specs:
- filename: 6a68bfdcf1d9df57e26c3545
  format: yaml
  label: We > Ultrarich MCP Server
  slug: we-ultrarich-mcp-server
  spec_type: Postman
  url: https://www.postman.com/wegtultrarich/we-ultrarich-extreme-wealth-api-mcp/collection/6a68bfdcf1d9df57e26c3545
- filename: we-ultrarich-comparison-api-openapi.yml
  format: yaml
  label: We > Ultrarich Comparison API
  slug: we-ultrarich-comparison-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/we-ultrarich/refs/heads/main/openapi/we-ultrarich-comparison-api-openapi.yml
- filename: we-ultrarich-discovery-api-openapi.yml
  format: yaml
  label: We > Ultrarich Discovery API
  slug: we-ultrarich-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/we-ultrarich/refs/heads/main/openapi/we-ultrarich-discovery-api-openapi.yml
- filename: we-ultrarich-wealth-expression-api-openapi.yml
  format: yaml
  label: We > Ultrarich Wealth Expression API
  slug: we-ultrarich-wealth-expression-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/we-ultrarich/refs/heads/main/openapi/we-ultrarich-wealth-expression-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: We Ultrarich Authentication
name_suffix: Authentication
oauth_flows: []
overview: We > Ultrarich secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: We > Ultrarich
provider_slug: we-ultrarich
scheme_count: 0
schemes: []
slug: we-ultrarich-authentication
source_filename: we-ultrarich-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\ndocs: https://api.wegtultrarich.org/README.md#access-and-rate-limits\nsource: openapi/we-ultrarich-openapi-original.yml\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  public: true\nschemes: []\nmodel:\n  authentication: none\n  authorization: none\n  account_required: false\n  api_key_required: false\n  detail: >-\n    \"No authentication. No account. No personal information requested.\" The OpenAPI 3.0.4 document declares\n    an empty top-level `security: []` and no `components.securitySchemes`, which matches the documented\n    posture exactly — this is a deliberate open, read-only, computation-only API rather than a thin spec\n    that omits its auth.\n  mcp:\n    url: https://api.wegtultrarich.org/mcp\n    authentication: none\n    session_state: none\n    detail: 'No Mcp-Session-Id and no initialize handshake required; tools/list answers anonymously.'\n  oauth_discovery_probed:\n    - {url: 'https://api.wegtultrarich.org/.well-known/oauth-authorization-server',\
  \ status: 404}\n    - {url: 'https://api.wegtultrarich.org/.well-known/oauth-protected-resource', status: 404}\n    - {url: 'https://api.wegtultrarich.org/.well-known/openid-configuration', status: 404}\n  note_no_scopes: >-\n    There is no OAuth surface, so no scopes/ artifact is emitted — an empty scopes file would misrepresent\n    the model.\naccess_controls_in_place_of_auth:\n  - control: per-IP rate limiting\n    detail: '100 req/min across /v1, 300 req/min for MCP, 500 req/min for docs'\n    see_also: rate-limits/we-ultrarich-rate-limits.yml\n  - control: CORS open by design\n    detail: 'Access-Control-Allow-Origin: * so browser-side and agent-generated code can call directly'\n  - control: read-only surface\n    detail: 'GET-only; no state is created, so there is nothing to authorize'\nprivacy:\n  personal_data_collected: false\n  detail: >-\n    Technical request data is processed transiently for rate limiting, security and operations; the site\n    uses privacy-first analytics\
  \ only.\n  policy: https://wegtultrarich.org/privacy-policy.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/we-ultrarich/refs/heads/main/authentication/we-ultrarich-authentication.yml
summary_line: none · 0 schemes
tags:
- wealth inequality
- economic inequality
- finance
- economics
- education
- journalism
- open data
- comparison
- mcp
- model context protocol
- agents
---
