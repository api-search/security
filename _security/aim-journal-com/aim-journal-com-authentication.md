---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for AIm Workout Journal MCP server uses OAuth 2.1 Bearer tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AIm Workout Journal Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIm Workout Journal declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AIm Workout Journal
provider_slug: aim-journal-com
scheme_count: 1
schemes:
- evidence: 'HTTP/1.1 401 Unauthorized

    www-authenticate: Bearer resource_metadata="https://example.com/.well-known/oauth-protected-resource"'
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Client registers itself via dynamic registration (enabled by oauth_server_allow_dynamic_registration) and then follows the OAuth 2.1 authorization code flow with PKCE to obtain an access token.
  location: header
  name: Bearer
  type: http-bearer
slug: aim-journal-com-authentication
source_filename: aim-journal-com-authentication.yml
source_heading: Authentication Profile
source_url: https://aim-journal.com/guides/en/mcp-server-oauth-supabase/
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://aim-journal.com/guides/en/mcp-server-oauth-supabase/\nsources:\n- https://aim-journal.com/guides/en/mcp-server-oauth-supabase/\ndescription: Authentication for AIm Workout Journal MCP server uses OAuth 2.1 Bearer tokens.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'HTTP/1.1 401 Unauthorized\n\n    www-authenticate: Bearer resource_metadata=\"https://example.com/.well-known/oauth-protected-resource\"'\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  how_to_obtain: Client registers itself via dynamic registration (enabled by oauth_server_allow_dynamic_registration) and then follows the OAuth\n    2.1 authorization code flow with PKCE to obtain an access token.\ndocs: https://aim-journal.com/guides/en/mcp-server-oauth-supabase/\n"
source_yaml_url: https://artifacts.apis.io/aim-journal-com/authentication/aim-journal-com-authentication.yml
summary_line: 1 scheme
tags:
- Fitness
- Artificial Intelligence
- Workouts
- Health
- Personalization
---
