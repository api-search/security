---
anonymous_access: false
api_key_in: []
api_specs:
- filename: changegamer-ai-openapi-generated.yml
  format: yaml
  label: ChangeGamer API
  slug: changegamer-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/changegamer-ai/openapi/_ae-authored/changegamer-ai-openapi-generated.yml
auth_types: []
description: Authentication methods described for ChangeGamer
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Changegamer Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChangeGamer declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ChangeGamer
provider_slug: changegamer-ai
scheme_count: 2
schemes:
- evidence: JWT-SVID — a signed JWT carrying the SPIFFE ID, presented as a plain bearer token in an Authorization header
  header: Authorization
  location: header
  name: JWT-SVID
  type: http-bearer
- evidence: ChangeGamer's own /mcp endpoint is currently unauthenticated, with no OAuth flow and no RFC 9728 metadata implemented, gating only paid resource content via an application-layer `api_key` argument rather than OAuth.
  location: query
  name: api_key
  type: apiKey
slug: changegamer-ai-authentication
source_filename: changegamer-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://changegamer.ai/resources/agent-identity-authentication.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://changegamer.ai/resources/agent-identity-authentication.md\nsources:\n- https://changegamer.ai/resources/agent-identity-authentication.md\n- https://changegamer.ai/resources/mcp-server-authentication.md\n- https://changegamer.ai/articles/api-key-issuance-for-agents.md\n- https://changegamer.ai/articles/mcp-server-in-production.md\ndescription: Authentication methods described for ChangeGamer\nschemes:\n- type: http-bearer\n  name: JWT-SVID\n  evidence: JWT-SVID — a signed JWT carrying the SPIFFE ID, presented as a plain bearer token in an Authorization header\n  location: header\n  header: Authorization\n- type: apiKey\n  name: api_key\n  evidence: ChangeGamer's own /mcp endpoint is currently unauthenticated, with no OAuth flow and no RFC 9728 metadata implemented, gating only\n    paid resource content via an application-layer `api_key` argument rather than OAuth.\n  location:\
  \ query\nnote: No OAuth2 flows are described on the referenced pages.\ndocs: https://changegamer.ai/resources/agent-identity-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/changegamer-ai/authentication/changegamer-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Infrastructure
- Agents
- Platform
- Reference
- Company
---
