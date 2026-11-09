---
anonymous_access: false
api_key_in: []
api_specs:
- filename: filen-health-api-openapi.yml
  format: yaml
  label: Filen Health API
  slug: filen-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-health-api-openapi.yml
- filename: filen-items-api-openapi.yml
  format: yaml
  label: Filen Items API
  slug: filen-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-items-api-openapi.yml
- filename: filen-shared-api-openapi.yml
  format: yaml
  label: Filen Shared API
  slug: filen-shared-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-shared-api-openapi.yml
- filename: filen-user-api-openapi.yml
  format: yaml
  label: Filen User API
  slug: filen-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-user-api-openapi.yml
- filename: filen-auth-api-openapi.yml
  format: yaml
  label: Filen Auth API
  slug: filen-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-auth-api-openapi.yml
- filename: filen-chat-api-openapi.yml
  format: yaml
  label: Filen Chat API
  slug: filen-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-chat-api-openapi.yml
- filename: filen-contacts-api-openapi.yml
  format: yaml
  label: Filen Contacts API
  slug: filen-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-contacts-api-openapi.yml
- filename: filen-dir-api-openapi.yml
  format: yaml
  label: Filen Dir API
  slug: filen-dir-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-dir-api-openapi.yml
- filename: filen-directories-api-openapi.yml
  format: yaml
  label: Filen Directories API
  slug: filen-directories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-directories-api-openapi.yml
- filename: filen-file-api-openapi.yml
  format: yaml
  label: Filen File API
  slug: filen-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-file-api-openapi.yml
- filename: filen-file-transfers-api-openapi.yml
  format: yaml
  label: Filen File Transfers API
  slug: filen-file-transfers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-file-transfers-api-openapi.yml
- filename: filen-internal-api-openapi.yml
  format: yaml
  label: Filen (internal) API
  slug: filen-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-internal-api-openapi.yml
- filename: filen-item-api-openapi.yml
  format: yaml
  label: Filen Item API
  slug: filen-item-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-item-api-openapi.yml
- filename: filen-misc-api-openapi.yml
  format: yaml
  label: Filen Misc API
  slug: filen-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-misc-api-openapi.yml
- filename: filen-mobile-api-openapi.yml
  format: yaml
  label: Filen Mobile API
  slug: filen-mobile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-mobile-api-openapi.yml
- filename: filen-notes-api-openapi.yml
  format: yaml
  label: Filen Notes API
  slug: filen-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-notes-api-openapi.yml
auth_types: []
description: Authentication for Filen API uses an API key passed as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Filen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Filen declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Filen
provider_slug: filen
scheme_count: 1
schemes:
- evidence: For API requests that require authentication, pass the API key in the Authorization HTTP header set to Bearer <api_key> .
  header: Authorization
  how_to_obtain: Call /v3/login with the user's email, derived and hashed password, and optional two‑factor code to receive an API key.
  location: header
  name: Bearer
  type: http-bearer
slug: filen-authentication
source_filename: filen-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.filen.io/docs/api/guides/authentication/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.filen.io/docs/api/guides/authentication/\nsources:\n- https://docs.filen.io/docs/api/guides/authentication/\n- https://docs.filen.io/docs/sdk/authentication/\n- https://docs.filen.io/docs/api/specs/get-auth-info/\n- https://docs.filen.io/docs/cli-rs/auth/\ndescription: Authentication for Filen API uses an API key passed as a Bearer token.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: For API requests that require authentication, pass the API key in the Authorization HTTP header set to Bearer <api_key> .\n  location: header\n  header: Authorization\n  how_to_obtain: Call /v3/login with the user's email, derived and hashed password, and optional two‑factor code to receive an API key.\nnote: No OAuth2 flows are described on the referenced pages.\ndocs: https://docs.filen.io/docs/api/guides/authentication/\n"
source_yaml_url: https://artifacts.apis.io/filen/authentication/filen-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Cloud Storage
- Encryption
- Zero Knowledge
- File Sync
---
