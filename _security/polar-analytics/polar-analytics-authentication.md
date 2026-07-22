---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Polar Analytics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Polar Analytics secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Polar Analytics
provider_slug: polar-analytics
scheme_count: 2
schemes:
- description: 'API key generated on the Polar MCP page (https://app.polaranalytics.com/mcp), passed as `Authorization: Bearer <API_KEY>`. Used for direct calls to the Polar MCP tool endpoints (https://api.polaranalytics.com/mcp/tool/<tool_name>).'
  name: apiKeyBearer
  scheme: bearer
  source: https://intercom.help/polar-app/en/articles/12960325-using-mcp-tools-as-an-api
  type: http
- description: OAuth 2.0 authorization server (RFC 8414) advertised at https://api.polaranalytics.com/.well-known/oauth-authorization-server for the hosted MCP connector. Supports Dynamic Client Registration (RFC 7591) and PKCE (S256).
  flows:
  - authorizationUrl: https://ai-service.polaranalytics.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://ai-service.polaranalytics.com/oauth/register
    tokenUrl: https://ai-service.polaranalytics.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://ai-service.polaranalytics.com/oauth/token
  name: oauth2
  source: https://api.polaranalytics.com/.well-known/oauth-authorization-server
  type: oauth2
slug: polar-analytics-authentication
source_filename: polar-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://intercom.help/polar-app/en/articles/12960325-using-mcp-tools-as-an-api\ndocs: https://intercom.help/polar-app/en/articles/12892599-use-polar-mcp-in-claude-claude-tag\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode, clientCredentials]\nschemes:\n  - name: apiKeyBearer\n    type: http\n    scheme: bearer\n    description: >-\n      API key generated on the Polar MCP page (https://app.polaranalytics.com/mcp),\n      passed as `Authorization: Bearer <API_KEY>`. Used for direct calls to the\n      Polar MCP tool endpoints (https://api.polaranalytics.com/mcp/tool/<tool_name>).\n    source: https://intercom.help/polar-app/en/articles/12960325-using-mcp-tools-as-an-api\n  - name: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0 authorization server (RFC 8414) advertised at\n      https://api.polaranalytics.com/.well-known/oauth-authorization-server for the\n   \
  \   hosted MCP connector. Supports Dynamic Client Registration (RFC 7591) and PKCE (S256).\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://ai-service.polaranalytics.com/oauth/authorize\n        tokenUrl: https://ai-service.polaranalytics.com/oauth/token\n        registrationUrl: https://ai-service.polaranalytics.com/oauth/register\n        pkce: S256\n      - flow: clientCredentials\n        tokenUrl: https://ai-service.polaranalytics.com/oauth/token\n    source: https://api.polaranalytics.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polar-analytics/refs/heads/main/authentication/polar-analytics-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Analytics
- Ecommerce
- Shopify
- Business Intelligence
- MCP
- AI Agents
- Data
---
