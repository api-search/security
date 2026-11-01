---
anonymous_access: false
api_key_in: []
api_specs:
- filename: emailverifier-dev-domains-api-openapi.yml
  format: yaml
  label: emailverifier-dev Domains API
  slug: emailverifier-dev-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailverifier-dev/openapi/emailverifier-dev-domains-api-openapi.yml
- filename: emailverifier-dev-usage-api-openapi.yml
  format: yaml
  label: emailverifier-dev Usage API
  slug: emailverifier-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailverifier-dev/openapi/emailverifier-dev-usage-api-openapi.yml
- filename: emailverifier-dev-verification-api-openapi.yml
  format: yaml
  label: emailverifier-dev Verification API
  slug: emailverifier-dev-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailverifier-dev/openapi/emailverifier-dev-verification-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Emailverifier Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: emailverifier-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: emailverifier-dev
provider_slug: emailverifier-dev
scheme_count: 2
schemes:
- description: API key for project authentication
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: Bearer token authentication (OAuth2 not provided)
  scheme: bearer
  type: http
slug: emailverifier-dev-authentication
source_filename: emailverifier-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://emailverifier.dev/api/openapi.json\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key for project authentication\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token authentication (OAuth2 not provided)"
source_yaml_url: https://artifacts.apis.io/emailverifier-dev/authentication/emailverifier-dev-authentication.yml
summary_line: 2 schemes
tags:
- Email
- Verification
- API
- SaaS
- DataQuality
---
