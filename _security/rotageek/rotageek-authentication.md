---
anonymous_access: false
api_key_in: []
api_specs:
- filename: rotageek-openapi-generated.yml
  format: yaml
  label: Rotageek API
  slug: rotageek-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rotageek/refs/heads/main/openapi/_ae-authored/rotageek-openapi-generated.yml
auth_types: []
description: Authentication for Rotageek public API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Rotageek Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rotageek declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Rotageek
provider_slug: rotageek
scheme_count: 1
schemes:
- evidence: To authenticate with the API, you must obtain an access token by sending a POST request to the authentication endpoint at /api/v1/auth.
  flows:
  - password
  how_to_obtain: 'Send a POST request to /api/v1/auth with form parameters grant_type=password, username and password to receive an access_token and refresh_token. Include the access token in subsequent requests as an HTTP header: Authorization: Bearer <access_token>.'
  name: Rotageek API OAuth2 Password Grant
  token_url: /api/v1/auth
  type: oauth2
slug: rotageek-authentication
source_filename: rotageek-authentication.yml
source_heading: Authentication Profile
source_url: https://support.rotageek.com/en/articles/6682375-multi-factor-authentication.md
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://support.rotageek.com/en/articles/6682375-multi-factor-authentication.md\nsources:\n- https://support.rotageek.com/en/articles/6682375-multi-factor-authentication.md\n- https://support.rotageek.com/en/articles/7182704-setting-up-multi-factor-authentication-for-rotageek.md\n- https://support.rotageek.com/en/articles/11513847-public-api-getting-started.md\ndescription: Authentication for Rotageek public API\nschemes:\n- type: oauth2\n  name: Rotageek API OAuth2 Password Grant\n  evidence: To authenticate with the API, you must obtain an access token by sending a POST request to the authentication endpoint at /api/v1/auth.\n  flows:\n  - password\n  token_url: /api/v1/auth\n  how_to_obtain: 'Send a POST request to /api/v1/auth with form parameters grant_type=password, username and password to receive an access_token\n    and refresh_token. Include the access token in subsequent\
  \ requests as an HTTP header: Authorization: Bearer <access_token>.'\ndocs: https://support.rotageek.com/en/articles/6682375-multi-factor-authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rotageek/refs/heads/main/authentication/rotageek-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Workforce-Management
- Scheduling
- AI-Insights
- HR-Integration
---
