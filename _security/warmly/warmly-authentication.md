---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Warmly Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Warmly secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Warmly
provider_slug: warmly
scheme_count: 2
schemes:
- description: 'REST API authenticates with a Bearer API key issued per organization, sent as `Authorization: Bearer <api-key>` against the REST base URL https://opps-api.getwarmly.com/api.'
  name: RestApiBearer
  scheme: bearer
  type: http
  used_by: REST API (agent-tools endpoints)
- description: The hosted MCP server at https://opps-api.getwarmly.com/api/mcp uses a browser-based OAuth login on first call, authorizing the connecting agent per Warmly organization.
  flows:
  - flow: authorizationCode
  name: McpOAuth
  type: oauth2
  used_by: MCP server
slug: warmly-authentication
source_filename: warmly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://help.warmly.ai/articles/9641856032-warmly-technical-documentation-rest-api\ndocs: https://help.warmly.ai/en/collections/5275235549-mcp_api\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  oauth2_flows: [authorizationCode]\n  org_scoping: [X-Warmly-Organization-Id header, organization_id query param, organizationId body field]\nschemes:\n  - name: RestApiBearer\n    type: http\n    scheme: bearer\n    description: >-\n      REST API authenticates with a Bearer API key issued per organization,\n      sent as `Authorization: Bearer <api-key>` against the REST base URL\n      https://opps-api.getwarmly.com/api.\n    used_by: REST API (agent-tools endpoints)\n  - name: McpOAuth\n    type: oauth2\n    description: >-\n      The hosted MCP server at https://opps-api.getwarmly.com/api/mcp uses a\n      browser-based OAuth login on first call, authorizing the connecting agent\n      per Warmly organization.\n   \
  \ flows:\n      - flow: authorizationCode\n    used_by: MCP server\norganization_scoping:\n  header: X-Warmly-Organization-Id\n  query_param: organization_id\n  body_field: organizationId\n  note: Multi-organization users must scope every call to a single organization.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warmly/refs/heads/main/authentication/warmly-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Sales
- Marketing
- Intent Data
- Revenue Orchestration
- Website Visitor Identification
- AI Agents
- Go To Market
- MCP
- Lead Generation
- CRM
---
