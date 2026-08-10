---
api_key_in: []
auth_types:
- visitor-token
description: ''
kind: authentication
layout: security
method: probed
name: Jobget Authentication
name_suffix: Authentication
oauth_flows: []
overview: JobGet secures its APIs with visitor-token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JobGet
provider_slug: jobget
scheme_count: 1
schemes:
- name: WixVisitorToken
  sources:
  - https://blog.jobget.com/llms.txt
  - live tools/list probe 2026-08-04
  surface: JobGet Site MCP Server
  type: bearer-like
slug: jobget-authentication
source_filename: jobget-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: 'anonymous HTTP probes of https://api.jobget.com and\n  https://blog.jobget.com/_api/mcp + https://blog.jobget.com/llms.txt'\nsummary:\n  types: [visitor-token]\n  api_key_in: []\n  oauth2_flows: []\n  documented: false\n  note: 'JobGet publishes no authentication documentation for its platform API. The only\n    authentication model that could be established from the public surface is the\n    anonymous visitor-token model of the Wix-provided site MCP endpoint. This artifact\n    is derived from live probes rather than from an OpenAPI, because JobGet publishes no\n    specification.'\nsurfaces:\n- surface: JobGet Platform API\n  host: https://api.jobget.com\n  documented: false\n  scheme: unknown\n  discovery:\n  - {path: /.well-known/openid-configuration, status: 404}\n  - {path: /.well-known/oauth-authorization-server, status: 404}\n  observed: 'Unknown paths return a 404 problem document rather than a 401/403 challenge\n\
  \    and emit no WWW-Authenticate header, so no authentication scheme is advertised at the\n    edge. The scheme protecting real routes cannot be determined without credentials, and\n    this pipeline does not use credentials.'\n  gaps:\n  - No public authentication guide.\n  - No OAuth 2.0 authorization-server metadata (RFC 8414).\n  - No OpenID Connect discovery document.\n  - No WWW-Authenticate challenge on unauthenticated requests.\n- surface: JobGet Site MCP Server\n  host: https://blog.jobget.com/_api/mcp\n  documented: true\n  documented_at: https://blog.jobget.com/llms.txt\n  scheme: visitor-token\n  anonymous_connect: true\n  observed: 'An anonymous POST tools/list returned HTTP 200 with the full tool set, so\n    connecting and discovering tools requires no credential. JobGet''s llms.txt states\n    verbatim: \"No authentication required to connect to the MCP endpoint\" and \"Only\n    public information accessible on the site is available\".'\n  token_acquisition:\n    tool:\
  \ GenerateVisitorToken\n    description: 'Creates a new visitor session and returns a visitor access token for\n      the site. Must be called before any CallWixSiteAPI or ExecuteWixAPI request.'\n    inputs: []\n  token_use:\n    parameter: visitorToken\n    used_by: [CallWixSiteAPI, ExecuteWixAPI]\n  scopes:\n    model: none\n    note: 'No OAuth scopes. Access is bounded by what the Wix site exposes publicly to a\n      visitor session, not by a scope grant, so there is no scopes/ artifact for this\n      provider.'\nschemes:\n- name: WixVisitorToken\n  type: bearer-like\n  surface: JobGet Site MCP Server\n  sources: [https://blog.jobget.com/llms.txt, 'live tools/list probe 2026-08-04']\nx-evidence:\n- fetched: '2026-08-04'\n  url: https://blog.jobget.com/_api/mcp\n  method: POST tools/list\n  http_status: 200\n- fetched: '2026-08-04'\n  url: https://api.jobget.com/.well-known/openid-configuration\n  http_status: 404\n- fetched: '2026-08-04'\n  url: https://api.jobget.com/.well-known/oauth-authorization-server\n\
  \  http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jobget/refs/heads/main/authentication/jobget-authentication.yml
summary_line: visitor-token · 1 scheme
tags:
- Company
- Jobs
- Recruiting
- Hiring
- Human Resources
- Talent Acquisition
- Job Search
- Hourly Work
- Applicant Tracking
- Marketplace
- Mobile
---
