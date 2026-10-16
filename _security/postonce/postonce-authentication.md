---
anonymous_access: false
api_key_in: []
api_specs:
- filename: postonce-api-openapi.json
  format: json
  label: PostOnce Public API API
  slug: postonce-public-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postonce/refs/heads/main/openapi/_original/postonce-api-openapi.json
auth_types: []
description: Authentication for the PostOnce Public API uses dashboard‑generated API keys sent as a bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Postonce Authentication
name_suffix: Authentication
oauth_flows: []
overview: PostOnce declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PostOnce
provider_slug: postonce
scheme_count: 1
schemes:
- evidence: 'Send your API key as a bearer token on every request:'
  header: Authorization
  how_to_obtain: Create an API key in the PostOnce dashboard under Preferences → API Keys, then copy the token immediately.
  location: header
  name: API key
  scopes:
  - accounts:read
  - accounts:write
  - media:read
  - media:write
  - posts:read
  - posts:write
  - workflows:read
  - workflows:write
  type: http-bearer
slug: postonce-authentication
source_filename: postonce-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.postonce.to/getting-started/authentication.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.postonce.to/getting-started/authentication.md\nsources:\n- https://docs.postonce.to/getting-started/authentication.md\n- https://docs.postonce.to/help/getting-started.md\n- https://docs.postonce.to/getting-started/response-format.md\n- https://docs.postonce.to/getting-started/data-structures.md\ndescription: Authentication for the PostOnce Public API uses dashboard‑generated API keys sent as a bearer token.\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Send your API key as a bearer token on every request:'\n  location: header\n  header: Authorization\n  scopes:\n  - accounts:read\n  - accounts:write\n  - media:read\n  - media:write\n  - posts:read\n  - posts:write\n  - workflows:read\n  - workflows:write\n  how_to_obtain: Create an API key in the PostOnce dashboard under Preferences → API Keys, then copy the token immediately.\nnote: No OAuth2, apiKey,\
  \ http-basic, jwt, hmac, mtls, or other authentication schemes are documented.\ndocs: https://docs.postonce.to/getting-started/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postonce/refs/heads/main/authentication/postonce-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Social Media
- Automation
- Marketing
- API
---
