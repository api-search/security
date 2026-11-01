---
anonymous_access: false
api_key_in: []
api_specs:
- filename: penneo-case-file-creation-api-openapi.yml
  format: yaml
  label: Penneo Case File Creation API
  slug: penneo-case-file-creation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/penneo/openapi/penneo-case-file-creation-api-openapi.yml
- filename: penneo-oauth-api-openapi.yml
  format: yaml
  label: Penneo OAuth API
  slug: penneo-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/penneo/openapi/penneo-oauth-api-openapi.yml
- filename: penneo-penneo-collect-api-api-openapi.yml
  format: yaml
  label: Penneo Penneo Collect API
  slug: penneo-penneo-collect-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/penneo/openapi/penneo-penneo-collect-api-api-openapi.yml
- filename: penneo-queue-status-check-api-openapi.yml
  format: yaml
  label: Penneo Queue Status Check API
  slug: penneo-queue-status-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/penneo/openapi/penneo-queue-status-check-api-openapi.yml
- filename: penneo-version-api-openapi.yml
  format: yaml
  label: Penneo Version API
  slug: penneo-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/penneo/openapi/penneo-version-api-openapi.yml
auth_types: []
description: Authentication methods as published on Penneo documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Penneo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Penneo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Penneo
provider_slug: penneo
scheme_count: 1
schemes:
- authorize_url: https://login-sandbox.penneo.com/oauth/authorize
  evidence: The recommended authentication method with the Penneo API is OAuth 2.0.
  flows:
  - authorization_code
  - api_keys
  how_to_obtain: Create an OAuth client in the Penneo web application (Configure > OAuth Clients) and use the client_id and client_secret. For the API Keys grant, generate an API key and secret in Penneo user settings and compute the required digest as described.
  name: OAuth 2.0
  type: oauth2
slug: penneo-authentication
source_filename: penneo-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.penneo.com/docs/authentication.md
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.penneo.com/docs/authentication.md\nsources:\n- https://developer.penneo.com/docs/authentication.md\n- https://developer.penneo.com/docs/using-oauth.md\n- https://developer.penneo.com/reference/oauth-authenticate-user.md\n- https://developer.penneo.com/reference/oauth-refresh-token.md\ndescription: Authentication methods as published on Penneo documentation.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: The recommended authentication method with the Penneo API is OAuth 2.0.\n  flows:\n  - authorization_code\n  - api_keys\n  authorize_url: https://login-sandbox.penneo.com/oauth/authorize\n  how_to_obtain: Create an OAuth client in the Penneo web application (Configure > OAuth Clients) and use the client_id and client_secret. For\n    the API Keys grant, generate an API key and secret in Penneo user settings and compute the required digest as described.\n\
  docs: https://developer.penneo.com/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/penneo/authentication/penneo-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Digital Signing
- eIDAS
- API
- Compliance
---
