---
anonymous_access: false
api_key_in: []
api_specs:
- filename: boardwalkai-com-account-api-openapi.yml
  format: yaml
  label: Boardwalk Account API
  slug: boardwalkai-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boardwalkai-com/openapi/boardwalkai-com-account-api-openapi.yml
- filename: boardwalkai-com-alerts-api-openapi.yml
  format: yaml
  label: Boardwalk Alerts API
  slug: boardwalkai-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boardwalkai-com/openapi/boardwalkai-com-alerts-api-openapi.yml
- filename: boardwalkai-com-analytics-api-openapi.yml
  format: yaml
  label: Boardwalk Analytics API
  slug: boardwalkai-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boardwalkai-com/openapi/boardwalkai-com-analytics-api-openapi.yml
- filename: boardwalkai-com-documents-api-openapi.yml
  format: yaml
  label: Boardwalk Documents API
  slug: boardwalkai-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boardwalkai-com/openapi/boardwalkai-com-documents-api-openapi.yml
- filename: boardwalkai-com-enrichment-api-openapi.yml
  format: yaml
  label: Boardwalk Enrichment API
  slug: boardwalkai-com-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boardwalkai-com/openapi/boardwalkai-com-enrichment-api-openapi.yml
- filename: boardwalkai-com-exports-api-openapi.yml
  format: yaml
  label: Boardwalk Exports API
  slug: boardwalkai-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boardwalkai-com/openapi/boardwalkai-com-exports-api-openapi.yml
- filename: boardwalkai-com-lists-api-openapi.yml
  format: yaml
  label: Boardwalk Lists API
  slug: boardwalkai-com-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boardwalkai-com/openapi/boardwalkai-com-lists-api-openapi.yml
- filename: boardwalkai-com-locations-api-openapi.yml
  format: yaml
  label: Boardwalk Locations API
  slug: boardwalkai-com-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boardwalkai-com/openapi/boardwalkai-com-locations-api-openapi.yml
- filename: boardwalkai-com-project-types-api-openapi.yml
  format: yaml
  label: Boardwalk Project types API
  slug: boardwalkai-com-project-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boardwalkai-com/openapi/boardwalkai-com-project-types-api-openapi.yml
- filename: boardwalkai-com-projects-api-openapi.yml
  format: yaml
  label: Boardwalk Projects API
  slug: boardwalkai-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boardwalkai-com/openapi/boardwalkai-com-projects-api-openapi.yml
- filename: boardwalkai-com-reference-api-openapi.yml
  format: yaml
  label: Boardwalk Reference API
  slug: boardwalkai-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boardwalkai-com/openapi/boardwalkai-com-reference-api-openapi.yml
auth_types: []
description: Boardwalk uses a single API key credential. The key can be sent either as a bearer token in the Authorization header or as a raw key in the X‑API‑Key header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Boardwalkai Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boardwalk declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Boardwalk
provider_slug: boardwalkai-com
scheme_count: 2
schemes:
- evidence: Every request carries an API key, as a bearer token or in X-API-Key.
  header: Authorization
  how_to_obtain: Create a key under Settings → API (or via POST /api/user/api-keys/{id}/rotate).
  location: header
  name: Bearer
  type: http-bearer
- evidence: Every request carries an API key, as a bearer token or in X-API-Key.
  header: X-API-Key
  how_to_obtain: Create a key under Settings → API (or via POST /api/user/api-keys/{id}/rotate).
  location: header
  name: X-API-Key
  type: apiKey
slug: boardwalkai-com-authentication
source_filename: boardwalkai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://boardwalkai.com/docs/api/authentication/
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://boardwalkai.com/docs/api/authentication/\nsources:\n- https://boardwalkai.com/docs/api/authentication/\n- https://boardwalkai.com/docs/api/quickstart/\ndescription: Boardwalk uses a single API key credential. The key can be sent either as a bearer token in the Authorization header or as a raw\n  key in the X‑API‑Key header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Every request carries an API key, as a bearer token or in X-API-Key.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key under Settings → API (or via POST /api/user/api-keys/{id}/rotate).\n- type: apiKey\n  name: X-API-Key\n  evidence: Every request carries an API key, as a bearer token or in X-API-Key.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a key under Settings → API (or via POST /api/user/api-keys/{id}/rotate).\nnote: No OAuth2 flows, JWT,\
  \ HMAC, MTLS, or other authentication mechanisms are documented.\ndocs: https://boardwalkai.com/docs/api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/boardwalkai-com/authentication/boardwalkai-com-authentication.yml
summary_line: 2 schemes
tags:
- Real Estate
- Construction
- Data Platform
- Mapping
- Analytics
---
