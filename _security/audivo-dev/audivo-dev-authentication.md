---
anonymous_access: false
api_key_in: []
api_specs:
- filename: audivo-dev-account-api-openapi.yml
  format: yaml
  label: audivo-dev Account API
  slug: audivo-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-account-api-openapi.yml
- filename: audivo-dev-api-keys-api-openapi.yml
  format: yaml
  label: audivo-dev API Keys API
  slug: audivo-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-api-keys-api-openapi.yml
- filename: audivo-dev-billing-api-openapi.yml
  format: yaml
  label: audivo-dev Billing API
  slug: audivo-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-billing-api-openapi.yml
- filename: audivo-dev-catalog-api-openapi.yml
  format: yaml
  label: audivo-dev Catalog API
  slug: audivo-dev-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-catalog-api-openapi.yml
- filename: audivo-dev-connected-apps-api-openapi.yml
  format: yaml
  label: audivo-dev Connected Apps API
  slug: audivo-dev-connected-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-connected-apps-api-openapi.yml
- filename: audivo-dev-data-api-openapi.yml
  format: yaml
  label: audivo-dev Data API
  slug: audivo-dev-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-data-api-openapi.yml
- filename: audivo-dev-groups-api-openapi.yml
  format: yaml
  label: audivo-dev Groups API
  slug: audivo-dev-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-groups-api-openapi.yml
- filename: audivo-dev-quotes-api-openapi.yml
  format: yaml
  label: audivo-dev Quotes API
  slug: audivo-dev-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-quotes-api-openapi.yml
- filename: audivo-dev-session-api-openapi.yml
  format: yaml
  label: audivo-dev Session API
  slug: audivo-dev-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-session-api-openapi.yml
- filename: audivo-dev-transcripts-api-openapi.yml
  format: yaml
  label: audivo-dev Transcripts API
  slug: audivo-dev-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-transcripts-api-openapi.yml
- filename: audivo-dev-uploads-api-openapi.yml
  format: yaml
  label: audivo-dev Uploads API
  slug: audivo-dev-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audivo-dev/openapi/audivo-dev-uploads-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Audivo Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: audivo-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: audivo-dev
provider_slug: audivo-dev
scheme_count: 2
schemes:
- evidence: 'Two authentication schemes, and which an operation takes is part of what it is: `apiKeyBearer` — an `hk_live_` key sent as `Authorization: Bearer` — authenticates the public API'
  header: Authorization
  how_to_obtain: Create a key in the dashboard; the plaintext key is shown once at creation.
  location: header
  name: apiKeyBearer
  type: http-bearer
- evidence: '`dashboardJwt` authenticates the dashboard''s own operations.'
  header: Authorization
  how_to_obtain: Obtain a JWT via the dashboard's sign‑in flow (Cognito).
  location: header
  name: dashboardJwt
  type: http-bearer
slug: audivo-dev-authentication
source_filename: audivo-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.audivo.dev/authentication.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.audivo.dev/authentication.md\nsources:\n- https://docs.audivo.dev/authentication.md\n- https://docs.audivo.dev/api-reference/api-keys/list-api-keys-for-the-account.md\n- https://docs.audivo.dev/api-reference/api-keys/create-a-labeled-api-key.md\n- https://docs.audivo.dev/api-reference/api-keys/revoke-an-api-key.md\nschemes:\n- type: http-bearer\n  name: apiKeyBearer\n  evidence: 'Two authentication schemes, and which an operation takes is part of what it is: `apiKeyBearer` — an `hk_live_` key sent as `Authorization:\n    Bearer` — authenticates the public API'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the dashboard; the plaintext key is shown once at creation.\n- type: http-bearer\n  name: dashboardJwt\n  evidence: '`dashboardJwt` authenticates the dashboard''s own operations.'\n  location: header\n  header: Authorization\n  how_to_obtain:\
  \ Obtain a JWT via the dashboard's sign‑in flow (Cognito).\ndocs: https://docs.audivo.dev/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/audivo-dev/authentication/audivo-dev-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Podcast
- Transcripts
- API
- Audio
---
