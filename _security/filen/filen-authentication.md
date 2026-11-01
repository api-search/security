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
- filename: filen-items-directories-api-openapi.yml
  format: yaml
  label: 'Filen Items: Directories API'
  slug: filen-items-directories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-items-directories-api-openapi.yml
- filename: filen-items-files-api-openapi.yml
  format: yaml
  label: 'Filen Items: Files API'
  slug: filen-items-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-items-files-api-openapi.yml
- filename: filen-public-links-api-openapi.yml
  format: yaml
  label: Filen Public Links API
  slug: filen-public-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-public-links-api-openapi.yml
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
