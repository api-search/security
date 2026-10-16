---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for the Discourse MCP server
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Springshare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Springshare declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Springshare
provider_slug: springshare
scheme_count: 3
schemes:
- evidence: 'Admin API Keys (require admin permissions): --auth_pairs ''[{"site":"https://example.com","api_key":"...","api_username":"system"}]'''
  how_to_obtain: Provide an admin API key and username in the --auth_pairs CLI argument.
  name: Admin API Key
  type: apiKey
- evidence: 'User API Keys (any user can generate): --auth_pairs ''[{"site":"https://example.com","user_api_key":"...","user_api_client_id":"..."}]'''
  how_to_obtain: Generate a user API key and client ID from the Discourse site and provide them in the --auth_pairs CLI argument.
  name: User API Key
  type: apiKey
- evidence: 'HTTP Basic Auth (for sites behind a reverse proxy): Add http_basic_user and http_basic_pass to any auth_pairs entry.'
  how_to_obtain: Supply a username and password via http_basic_user and http_basic_pass fields in the --auth_pairs CLI argument.
  name: HTTP Basic Auth
  type: http-basic
slug: springshare-authentication
source_filename: springshare-authentication.yml
source_heading: Authentication Profile
source_url: https://github.com/discourse/discourse-mcp#quick-start-release
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://github.com/discourse/discourse-mcp#quick-start-release\nsources:\n- https://github.com/discourse/discourse-mcp#quick-start-release\ndescription: Authentication methods for the Discourse MCP server\nschemes:\n- type: apiKey\n  name: Admin API Key\n  evidence: 'Admin API Keys (require admin permissions): --auth_pairs ''[{\"site\":\"https://example.com\",\"api_key\":\"...\",\"api_username\":\"system\"}]'''\n  how_to_obtain: Provide an admin API key and username in the --auth_pairs CLI argument.\n- type: apiKey\n  name: User API Key\n  evidence: 'User API Keys (any user can generate): --auth_pairs ''[{\"site\":\"https://example.com\",\"user_api_key\":\"...\",\"user_api_client_id\":\"...\"}]'''\n  how_to_obtain: Generate a user API key and client ID from the Discourse site and provide them in the --auth_pairs CLI argument.\n- type: http-basic\n  name: HTTP Basic Auth\n  evidence:\
  \ 'HTTP Basic Auth (for sites behind a reverse proxy): Add http_basic_user and http_basic_pass to any auth_pairs entry.'\n  how_to_obtain: Supply a username and password via http_basic_user and http_basic_pass fields in the --auth_pairs CLI argument.\nnote: The documentation does not specify the exact header name or query parameter used for the API keys or basic auth; those fields are left null.\ndocs: https://github.com/discourse/discourse-mcp#quick-start-release\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/springshare/refs/heads/main/authentication/springshare-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Library Services
- SaaS
- Education
- Open Source
---
