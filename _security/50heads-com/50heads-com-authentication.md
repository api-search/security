---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for 50heads APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: 50Heads Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: 50heads declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: 50heads
provider_slug: 50heads-com
scheme_count: 2
schemes:
- evidence: 'The key starts fh_live_ and is shown once: copy it into your secret store right away.'
  header: Authorization
  how_to_obtain: Create a key in the Developers portal; the key is displayed once with the prefix fh_live_.
  location: header
  name: API Key
  type: http-bearer
- evidence: The server is an OAuth 2.1 resource server. Hosts discover everything from https://mcp.50heads.com/.well-known/oauth-protected-resource, which points at the authorization server https://auth.50heads.com.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Sign in with OAuth in the browser via the hosted MCP server or supported agents; PKCE (S256) and the resource parameter are required.
  location: header
  name: MCP OAuth
  scopes:
  - questions:read
  - questions:write
  - templates:read
  - account:read
  - webhooks:read
  - webhooks:write
  - apps:read
  - apps:write
  - organization:read
  - organization:write
  - members:read
  - members:write
  - audit:read
  - events:read
  type: oauth2
slug: 50heads-com-authentication
source_filename: 50heads-com-authentication.yml
source_heading: Authentication Profile
source_url: https://50heads.com/en-us/help/api-and-mcp/api-keys
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://50heads.com/en-us/help/api-and-mcp/api-keys\nsources:\n- https://50heads.com/en-us/help/api-and-mcp/api-keys\n- https://50heads.com/en-us/help/account/sign-in-options\n- https://50heads.com/en-us/docs/mcp\n- https://50heads.com/en-us/help/getting-started/what-is-50heads\ndescription: Authentication methods for 50heads APIs\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'The key starts fh_live_ and is shown once: copy it into your secret store right away.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the Developers portal; the key is displayed once with the prefix fh_live_.\n- type: oauth2\n  name: MCP OAuth\n  evidence: The server is an OAuth 2.1 resource server. Hosts discover everything from https://mcp.50heads.com/.well-known/oauth-protected-resource,\n    which points at the authorization server https://auth.50heads.com.\n\
  \  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  scopes:\n  - questions:read\n  - questions:write\n  - templates:read\n  - account:read\n  - webhooks:read\n  - webhooks:write\n  - apps:read\n  - apps:write\n  - organization:read\n  - organization:write\n  - members:read\n  - members:write\n  - audit:read\n  - events:read\n  how_to_obtain: Sign in with OAuth in the browser via the hosted MCP server or supported agents; PKCE (S256) and the resource parameter are required.\ndocs: https://50heads.com/en-us/help/api-and-mcp/api-keys\n"
source_yaml_url: https://artifacts.apis.io/50heads-com/authentication/50heads-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Verification
- Surveys
- Platform
---
