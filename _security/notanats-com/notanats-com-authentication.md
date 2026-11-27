---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: notanats-com-agent-api-candidates-api-openapi.yml
  format: yaml
  label: notanATS Agent API — candidates API
  slug: notanats-com-agent-api-candidates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-agent-api-candidates-api-openapi.yml
- filename: notanats-com-agent-api-directory-api-openapi.yml
  format: yaml
  label: notanATS Agent API — directory API
  slug: notanats-com-agent-api-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-agent-api-directory-api-openapi.yml
- filename: notanats-com-agent-api-positions-api-openapi.yml
  format: yaml
  label: notanATS Agent API — positions API
  slug: notanats-com-agent-api-positions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-agent-api-positions-api-openapi.yml
- filename: notanats-com-agent-api-proposals-api-openapi.yml
  format: yaml
  label: notanATS Agent API — proposals API
  slug: notanats-com-agent-api-proposals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-agent-api-proposals-api-openapi.yml
- filename: notanats-com-credential-management-manager-session-api-openapi.yml
  format: yaml
  label: notanATS Credential management — manager session API
  slug: notanats-com-credential-management-manager-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-credential-management-manager-session-api-openapi.yml
- filename: notanats-com-legacy-api-v1-data-reads-api-openapi.yml
  format: yaml
  label: notanATS Legacy /api/v1 — data reads API
  slug: notanats-com-legacy-api-v1-data-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-legacy-api-v1-data-reads-api-openapi.yml
- filename: notanats-com-oauth-admin-review-api-openapi.yml
  format: yaml
  label: notanATS OAuth — admin review API
  slug: notanats-com-oauth-admin-review-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-oauth-admin-review-api-openapi.yml
- filename: notanats-com-oauth-discovery-api-openapi.yml
  format: yaml
  label: notanATS OAuth — discovery API
  slug: notanats-com-oauth-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-oauth-discovery-api-openapi.yml
- filename: notanats-com-oauth-flow-api-openapi.yml
  format: yaml
  label: notanATS OAuth — flow API
  slug: notanats-com-oauth-flow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notanats-com/openapi/notanats-com-oauth-flow-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: notanATS Authentication
name_suffix: Authentication
oauth_flows: []
overview: notanATS secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: notanATS
provider_slug: notanats-com
scheme_count: 2
schemes:
- description: 'A static delegated agent key (prefix nagt_) minted by an organization admin for a named delegated manager. This is the ONLY credential class the REST agent API authenticates: the REST guard resolves nagt_ (and, on the legacy /api/v1 data routes, nats_) keys only. An OAuth access token (noat_) does NOT authenticate REST — it resolves only in the MCP seam at /mcp.'
  name: agentBearer
  scheme: bearer
  sources:
  - openapi/notanats-com-openapi.json
  type: http
- description: The signed-in manager/admin webapp session, carried by the app’s Supabase SSR session cookies (the sb-<project>-auth-token cookie and any chunked companions, set at sign-in; the exact cookie name is derived from the Supabase project, so the name shown is a pattern, not a literal). These surfaces are not callable with an agent credential.
  in: cookie
  name: managerSession
  parameter: sb-*-auth-token
  sources:
  - openapi/notanats-com-openapi.json
  type: apiKey
slug: notanats-com-authentication
source_filename: notanats-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/notanats-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: agentBearer\n  type: http\n  scheme: bearer\n  description: 'A static delegated agent key (prefix nagt_) minted by an organization admin\n    for a named delegated manager. This is the ONLY credential class the REST agent API authenticates:\n    the REST guard resolves nagt_ (and, on the legacy /api/v1 data routes, nats_) keys only.\n    An OAuth access token (noat_) does NOT authenticate REST — it resolves only in the MCP seam\n    at /mcp.'\n  sources:\n  - openapi/notanats-com-openapi.json\n- name: managerSession\n  type: apiKey\n  in: cookie\n  parameter: sb-*-auth-token\n  description: The signed-in manager/admin webapp session, carried by the app’s Supabase SSR\n    session cookies (the sb-<project>-auth-token cookie and any chunked companions, set at sign-in;\n    the exact cookie name is derived from\
  \ the Supabase project, so the name shown is a pattern,\n    not a literal). These surfaces are not callable with an agent credential.\n  sources:\n  - openapi/notanats-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/notanats-com/authentication/notanats-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Screening
- Hiring
- Hiring Managers
- Agents
- AI Screening
---
