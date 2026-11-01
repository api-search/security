---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Traceabledocs Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: traceabledocs-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: traceabledocs-com
provider_slug: traceabledocs-com
scheme_count: 1
schemes:
- authorizationUrl: https://app.traceabledocs.com/oauth/authorize
  flow: authorizationCode
  scopes:
    documents:read: Read documents
    documents:write: Write documents
  tokenUrl: https://app.traceabledocs.com/oauth/token
  type: oauth2
slug: traceabledocs-com-authentication
source_filename: traceabledocs-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://traceabledocs.com/docs/mcp-reference.md\nschemes:\n  - type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://app.traceabledocs.com/oauth/authorize\n    tokenUrl: https://app.traceabledocs.com/oauth/token\n    scopes:\n      documents:read: Read documents\n      documents:write: Write documents\n"
source_yaml_url: https://artifacts.apis.io/traceabledocs-com/authentication/traceabledocs-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Requirements Management
- Document Control
- Regulatory Compliance
- AI Integration
---
