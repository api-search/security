---
anonymous_access: false
api_key_in: []
api_specs:
- filename: linkedmash-com-analytics-api-openapi.yml
  format: yaml
  label: LinkedMash Analytics API
  slug: linkedmash-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-analytics-api-openapi.yml
- filename: linkedmash-com-bookmarks-api-openapi.yml
  format: yaml
  label: LinkedMash Bookmarks API
  slug: linkedmash-com-bookmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-bookmarks-api-openapi.yml
- filename: linkedmash-com-drafts-api-openapi.yml
  format: yaml
  label: LinkedMash Drafts API
  slug: linkedmash-com-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-drafts-api-openapi.yml
- filename: linkedmash-com-labels-api-openapi.yml
  format: yaml
  label: LinkedMash Labels API
  slug: linkedmash-com-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-labels-api-openapi.yml
- filename: linkedmash-com-media-api-openapi.yml
  format: yaml
  label: LinkedMash Media API
  slug: linkedmash-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-media-api-openapi.yml
- filename: linkedmash-com-queue-api-openapi.yml
  format: yaml
  label: LinkedMash Queue API
  slug: linkedmash-com-queue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-queue-api-openapi.yml
- filename: linkedmash-com-schedule-api-openapi.yml
  format: yaml
  label: LinkedMash Schedule API
  slug: linkedmash-com-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkedmash-com/openapi/linkedmash-com-schedule-api-openapi.yml
auth_types: []
description: Authentication methods for LinkedMash API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LinkedMash Authentication
name_suffix: Authentication
oauth_flows: []
overview: LinkedMash declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LinkedMash
provider_slug: linkedmash-com
scheme_count: 2
schemes:
- evidence: 'REST and MCP continue to accept `Authorization: Bearer <api-key>`.'
  header: Authorization
  how_to_obtain: Create an API key at https://www.linkedmash.com/integrations/api.
  location: header
  name: API Key
  type: apiKey
- evidence: Use scoped OAuth 2.0 client credentials for new confidential agents and server-side integrations.
  flows:
  - client_credentials
  how_to_obtain: Create an API key at https://www.linkedmash.com/integrations/api and use its key ID as the client ID and its secret as the client secret.
  name: OAuth2 Client Credentials
  scopes:
  - library:read
  - library:write
  - content:read
  - content:write
  - analytics:read
  - exports:read
  - exports:write
  token_url: https://api.linkedmash.com/auth/oauth/token
  type: oauth2
slug: linkedmash-com-authentication
source_filename: linkedmash-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.linkedmash.com/auth.md
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.linkedmash.com/auth.md\nsources:\n- https://www.linkedmash.com/auth.md\n- https://www.linkedmash.com/.well-known/oauth-authorization-server\n- https://www.linkedmash.com/.well-known/oauth-protected-resource\n- https://www.linkedmash.com/api-docs/getting-started\ndescription: Authentication methods for LinkedMash API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'REST and MCP continue to accept `Authorization: Bearer <api-key>`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key at https://www.linkedmash.com/integrations/api.\n- type: oauth2\n  name: OAuth2 Client Credentials\n  evidence: Use scoped OAuth 2.0 client credentials for new confidential agents and server-side integrations.\n  flows:\n  - client_credentials\n  token_url: https://api.linkedmash.com/auth/oauth/token\n  scopes:\n  - library:read\n  - library:write\n  -\
  \ content:read\n  - content:write\n  - analytics:read\n  - exports:read\n  - exports:write\n  how_to_obtain: Create an API key at https://www.linkedmash.com/integrations/api and use its key ID as the client ID and its secret as the client\n    secret.\ndocs: https://www.linkedmash.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/linkedmash-com/authentication/linkedmash-com-authentication.yml
summary_line: 2 schemes
tags:
- LinkedIn Integration
- Content Management
- Data Export
- AI Integration
- Productivity
---
