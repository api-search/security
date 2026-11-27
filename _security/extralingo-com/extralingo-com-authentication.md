---
anonymous_access: false
api_key_in: []
api_specs:
- filename: extralingo-com-bookings-api-openapi.yml
  format: yaml
  label: Extralingo Bookings API
  slug: extralingo-com-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/extralingo-com/openapi/extralingo-com-bookings-api-openapi.yml
- filename: extralingo-com-destinations-api-openapi.yml
  format: yaml
  label: Extralingo Destinations API
  slug: extralingo-com-destinations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/extralingo-com/openapi/extralingo-com-destinations-api-openapi.yml
- filename: extralingo-com-meta-api-openapi.yml
  format: yaml
  label: Extralingo Meta API
  slug: extralingo-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/extralingo-com/openapi/extralingo-com-meta-api-openapi.yml
- filename: extralingo-com-schools-api-openapi.yml
  format: yaml
  label: Extralingo Schools API
  slug: extralingo-com-schools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/extralingo-com/openapi/extralingo-com-schools-api-openapi.yml
- filename: extralingo-com-trips-api-openapi.yml
  format: yaml
  label: Extralingo Trips API
  slug: extralingo-com-trips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/extralingo-com/openapi/extralingo-com-trips-api-openapi.yml
auth_types: []
description: Extralingo agents use OAuth 2.1 authorization code flow with PKCE and Bearer tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Extralingo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Extralingo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Extralingo
provider_slug: extralingo-com
scheme_count: 1
schemes:
- authorize_url: https://www.extralingo.com/oauth/authorize
  evidence: 'Write tools require OAuth 2.1: authorization code with PKCE S256, scopes trips, requests and bookings.'
  header: Authorization
  how_to_obtain: Dynamic client registration via POST https://www.extralingo.com/oauth/register.
  location: header
  name: OAuth 2.1 Authorization Code with PKCE
  scopes:
  - trips
  - requests
  - bookings
  token_url: https://www.extralingo.com/oauth/token
  type: http-bearer
slug: extralingo-com-authentication
source_filename: extralingo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.extralingo.com/auth.md
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.extralingo.com/auth.md\nsources:\n- https://www.extralingo.com/auth.md\n- https://www.extralingo.com/en/developers\ndescription: Extralingo agents use OAuth 2.1 authorization code flow with PKCE and Bearer tokens.\nschemes:\n- type: http-bearer\n  name: OAuth 2.1 Authorization Code with PKCE\n  evidence: 'Write tools require OAuth 2.1: authorization code with PKCE S256, scopes trips, requests and bookings.'\n  location: header\n  header: Authorization\n  token_url: https://www.extralingo.com/oauth/token\n  authorize_url: https://www.extralingo.com/oauth/authorize\n  scopes:\n  - trips\n  - requests\n  - bookings\n  how_to_obtain: Dynamic client registration via POST https://www.extralingo.com/oauth/register.\ndocs: https://www.extralingo.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/extralingo-com/authentication/extralingo-com-authentication.yml
summary_line: 1 scheme
tags:
- Education
- Language Learning
- Travel
- Comparison
- Reviews
---
