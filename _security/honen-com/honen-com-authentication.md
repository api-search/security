---
anonymous_access: false
api_key_in: []
api_specs:
- filename: honen-com-agents-api-openapi.yml
  format: yaml
  label: Honen Agents API
  slug: honen-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-agents-api-openapi.yml
- filename: honen-com-analytics-api-openapi.yml
  format: yaml
  label: Honen Analytics API
  slug: honen-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-analytics-api-openapi.yml
- filename: honen-com-assignments-api-openapi.yml
  format: yaml
  label: Honen Assignments API
  slug: honen-com-assignments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-assignments-api-openapi.yml
- filename: honen-com-course-editor-api-openapi.yml
  format: yaml
  label: Honen Course Editor API
  slug: honen-com-course-editor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-course-editor-api-openapi.yml
- filename: honen-com-courses-api-openapi.yml
  format: yaml
  label: Honen Courses API
  slug: honen-com-courses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-courses-api-openapi.yml
- filename: honen-com-explore-api-openapi.yml
  format: yaml
  label: Honen Explore API
  slug: honen-com-explore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-explore-api-openapi.yml
- filename: honen-com-groups-api-openapi.yml
  format: yaml
  label: Honen Groups API
  slug: honen-com-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-groups-api-openapi.yml
- filename: honen-com-invites-api-openapi.yml
  format: yaml
  label: Honen Invites API
  slug: honen-com-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-invites-api-openapi.yml
- filename: honen-com-kb-api-openapi.yml
  format: yaml
  label: Honen Kb API
  slug: honen-com-kb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-kb-api-openapi.yml
- filename: honen-com-learning-api-openapi.yml
  format: yaml
  label: Honen Learning API
  slug: honen-com-learning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-learning-api-openapi.yml
- filename: honen-com-members-api-openapi.yml
  format: yaml
  label: Honen Members API
  slug: honen-com-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-members-api-openapi.yml
- filename: honen-com-performance-api-openapi.yml
  format: yaml
  label: Honen Performance API
  slug: honen-com-performance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-performance-api-openapi.yml
- filename: honen-com-workspace-api-openapi.yml
  format: yaml
  label: Honen Workspace API
  slug: honen-com-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-workspace-api-openapi.yml
- filename: honen-com-workspace-assistant-api-openapi.yml
  format: yaml
  label: Honen Workspace Assistant API
  slug: honen-com-workspace-assistant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honen-com/openapi/honen-com-workspace-assistant-api-openapi.yml
auth_types: []
description: Authentication methods for Honen
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Honen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Honen declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Honen
provider_slug: honen-com
scheme_count: 2
schemes:
- authorize_url: https://honen.com/api/oauth/authorize
  evidence: Honen uses user-authorized OAuth 2.0 with PKCE for MCP access.
  flows:
  - authorization_code
  how_to_obtain: Register a public OAuth client at the registration_endpoint, then perform the authorization‑code grant with PKCE (S256) to obtain an access token.
  name: OAuth 2.0 Authorization Code with PKCE
  scopes:
  - honen:mcp
  - course:edit
  - site:edit
  - knowledgebase.read
  - knowledgebase.write
  - workspace-assistant
  type: oauth2
- evidence: 'For the Connector HTTP API described at https://honen.com/openapi.json, send its workspace‑issued Connector secret or child token in the same `Authorization: Bearer` header.'
  header: Authorization
  how_to_obtain: A workspace administrator creates a Connector credential (secret) in the Honen dashboard; the raw secret is shown once at creation or rotation.
  location: header
  name: Connector secret
  type: http-bearer
slug: honen-com-authentication
source_filename: honen-com-authentication.yml
source_heading: Authentication Profile
source_url: https://honen.com/auth.md
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://honen.com/auth.md\nsources:\n- https://honen.com/auth.md\n- https://honen.com/.well-known/oauth-protected-resource\n- https://honen.com/.well-known/oauth-authorization-server\n- https://honen.com/developers.txt\ndescription: Authentication methods for Honen\nschemes:\n- type: oauth2\n  name: OAuth 2.0 Authorization Code with PKCE\n  evidence: Honen uses user-authorized OAuth 2.0 with PKCE for MCP access.\n  flows:\n  - authorization_code\n  authorize_url: https://honen.com/api/oauth/authorize\n  scopes:\n  - honen:mcp\n  - course:edit\n  - site:edit\n  - knowledgebase.read\n  - knowledgebase.write\n  - workspace-assistant\n  how_to_obtain: Register a public OAuth client at the registration_endpoint, then perform the authorization‑code grant with PKCE (S256) to obtain\n    an access token.\n- type: http-bearer\n  name: Connector secret\n  evidence: 'For the Connector HTTP\
  \ API described at https://honen.com/openapi.json, send its workspace‑issued Connector secret or child token\n    in the same `Authorization: Bearer` header.'\n  location: header\n  header: Authorization\n  how_to_obtain: A workspace administrator creates a Connector credential (secret) in the Honen dashboard; the raw secret is shown once at creation\n    or rotation.\ndocs: https://honen.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/honen-com/authentication/honen-com-authentication.yml
summary_line: 2 schemes
tags:
- Course Authoring
- Workforce Training
---
