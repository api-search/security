---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nexatron-io-auth-api-openapi.yml
  format: yaml
  label: Nexatron Auth API
  slug: nexatron-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-auth-api-openapi.yml
- filename: nexatron-io-connections-api-openapi.yml
  format: yaml
  label: Nexatron Connections API
  slug: nexatron-io-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-connections-api-openapi.yml
- filename: nexatron-io-contact-api-openapi.yml
  format: yaml
  label: Nexatron Contact API
  slug: nexatron-io-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-contact-api-openapi.yml
- filename: nexatron-io-conversations-api-openapi.yml
  format: yaml
  label: Nexatron Conversations API
  slug: nexatron-io-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-conversations-api-openapi.yml
- filename: nexatron-io-feedback-api-openapi.yml
  format: yaml
  label: Nexatron Feedback API
  slug: nexatron-io-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-feedback-api-openapi.yml
- filename: nexatron-io-query-api-openapi.yml
  format: yaml
  label: Nexatron Query API
  slug: nexatron-io-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-query-api-openapi.yml
- filename: nexatron-io-semantic-api-openapi.yml
  format: yaml
  label: Nexatron Semantic API
  slug: nexatron-io-semantic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-semantic-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Nexatron Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nexatron declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Nexatron
provider_slug: nexatron-io
scheme_count: 2
schemes:
- evidence: The server uses OAuth 2.1 with the authorization code flow and PKCE (S256).
  header: Authorization
  how_to_obtain: Clients can register themselves with dynamic client registration and discover the authorization server from the protected resource metadata and authorization server metadata URLs.
  location: header
  name: OAuth 2.1 Authorization Code with PKCE
  scopes:
  - mcp:read
  - mcp:query
  - openid
  - offline_access
  - mcp:metrics:execute
  - mcp:federation
  - actions:execute_low
  - actions:execute_medium
  - actions:execute_high
  - actions:compose_workflow
  - mcp:reports:read
  - mcp:conversations
  type: oauth2
- evidence: Send an API key as a bearer token in the Authorization header.
  header: Authorization
  how_to_obtain: Create a token in Settings → API tokens, copy the shown token, and use it as a Bearer token.
  location: header
  name: Personal API token
  type: apiKey
slug: nexatron-io-authentication
source_filename: nexatron-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.nexatron.io/integrations/mcp-reference/
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.nexatron.io/integrations/mcp-reference/\nsources:\n- https://docs.nexatron.io/integrations/mcp-reference/\n- https://docs.nexatron.io/quickstart/api-tokens/\n- https://docs.nexatron.io/api/reference/me-api-v-1-auth-me-get/\n- https://docs.nexatron.io/api/reference/refresh-token-api-v-1-auth-refresh-post/\nschemes:\n- type: oauth2\n  name: OAuth 2.1 Authorization Code with PKCE\n  evidence: The server uses OAuth 2.1 with the authorization code flow and PKCE (S256).\n  location: header\n  header: Authorization\n  scopes:\n  - mcp:read\n  - mcp:query\n  - openid\n  - offline_access\n  - mcp:metrics:execute\n  - mcp:federation\n  - actions:execute_low\n  - actions:execute_medium\n  - actions:execute_high\n  - actions:compose_workflow\n  - mcp:reports:read\n  - mcp:conversations\n  how_to_obtain: Clients can register themselves with dynamic client registration and discover\
  \ the authorization server from the protected resource\n    metadata and authorization server metadata URLs.\n- type: apiKey\n  name: Personal API token\n  evidence: Send an API key as a bearer token in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token in Settings → API tokens, copy the shown token, and use it as a Bearer token.\ndocs: https://docs.nexatron.io/integrations/mcp-reference/\n"
source_yaml_url: https://artifacts.apis.io/nexatron-io/authentication/nexatron-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Enterprise
- Context
- Data Integration
---
