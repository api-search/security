---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clearlist-me-account-api-openapi.yml
  format: yaml
  label: ClearList Account API
  slug: clearlist-me-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-account-api-openapi.yml
- filename: clearlist-me-jobs-api-openapi.yml
  format: yaml
  label: ClearList Jobs API
  slug: clearlist-me-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-jobs-api-openapi.yml
- filename: clearlist-me-listings-api-openapi.yml
  format: yaml
  label: ClearList Listings API
  slug: clearlist-me-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-listings-api-openapi.yml
- filename: clearlist-me-onboarding-api-openapi.yml
  format: yaml
  label: ClearList Onboarding API
  slug: clearlist-me-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-onboarding-api-openapi.yml
- filename: clearlist-me-orders-api-openapi.yml
  format: yaml
  label: ClearList Orders API
  slug: clearlist-me-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-orders-api-openapi.yml
- filename: clearlist-me-publishing-api-openapi.yml
  format: yaml
  label: ClearList Publishing API
  slug: clearlist-me-publishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-publishing-api-openapi.yml
- filename: clearlist-me-scheduling-api-openapi.yml
  format: yaml
  label: ClearList Scheduling API
  slug: clearlist-me-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-scheduling-api-openapi.yml
- filename: clearlist-me-system-api-openapi.yml
  format: yaml
  label: ClearList System API
  slug: clearlist-me-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-system-api-openapi.yml
auth_types: []
description: Authentication methods for ClearList
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Clearlist Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClearList declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ClearList
provider_slug: clearlist-me
scheme_count: 3
schemes:
- evidence: 'Header: `X-ClearList-API-Key`, or `Authorization: Bearer cl_<64-hex>` (the same credential; OAuth access tokens are sent this way)'
  header: X-ClearList-API-Key
  how_to_obtain: '1. POST /api/auth/send-code { email } → emails a 6-digit code. 2. POST /api/auth/verify-code { email, code, agent: true } → returns { apiKey }. 3. Pass apiKey in X-ClearList-API-Key header on subsequent requests.'
  location: header
  name: API Key
  type: apiKey
- authorize_url: https://clearlist.me/oauth/authorize
  evidence: '`Authorization: Bearer cl_<64-hex>` access token, scoped `read` / `write`'
  header: Authorization
  how_to_obtain: Apps a seller connects, e.g. an AI assistant connector, register dynamically or with a client ID metadata document and use the standard OAuth 2.1 authorization code flow with PKCE S256.
  location: header
  name: OAuth 2.1
  scopes:
  - read
  - write
  token_url: https://clearlist.me/api/oauth/token
  type: oauth2
- evidence: '`Authorization: Bearer <firebase_id_token>`'
  header: Authorization
  how_to_obtain: Used by ClearList web UI / PWA only.
  location: header
  name: Firebase ID token
  type: http-bearer
slug: clearlist-me-authentication
source_filename: clearlist-me-authentication.yml
source_heading: Authentication Profile
source_url: https://clearlist.me/auth.md
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://clearlist.me/auth.md\nsources:\n- https://clearlist.me/auth.md\n- https://clearlist.me/.well-known/oauth-authorization-server\n- https://clearlist.me/.well-known/oauth-protected-resource\ndescription: Authentication methods for ClearList\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Header: `X-ClearList-API-Key`, or `Authorization: Bearer cl_<64-hex>` (the same credential; OAuth access tokens are sent this way)'\n  location: header\n  header: X-ClearList-API-Key\n  how_to_obtain: '1. POST /api/auth/send-code { email } → emails a 6-digit code. 2. POST /api/auth/verify-code { email, code, agent: true } →\n    returns { apiKey }. 3. Pass apiKey in X-ClearList-API-Key header on subsequent requests.'\n- type: oauth2\n  name: OAuth 2.1\n  evidence: '`Authorization: Bearer cl_<64-hex>` access token, scoped `read` / `write`'\n  location: header\n  header: Authorization\n\
  \  token_url: https://clearlist.me/api/oauth/token\n  authorize_url: https://clearlist.me/oauth/authorize\n  scopes:\n  - read\n  - write\n  how_to_obtain: Apps a seller connects, e.g. an AI assistant connector, register dynamically or with a client ID metadata document and use the\n    standard OAuth 2.1 authorization code flow with PKCE S256.\n- type: http-bearer\n  name: Firebase ID token\n  evidence: '`Authorization: Bearer <firebase_id_token>`'\n  location: header\n  header: Authorization\n  how_to_obtain: Used by ClearList web UI / PWA only.\ndocs: https://clearlist.me/auth.md\n"
source_yaml_url: https://artifacts.apis.io/clearlist-me/authentication/clearlist-me-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Resale
- Marketplace
- Automation
- E-Commerce
- Company
---
