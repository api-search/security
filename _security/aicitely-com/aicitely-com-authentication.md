---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aicitely-com-health-api-openapi.yml
  format: yaml
  label: Citely Health API
  slug: aicitely-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicitely-com/openapi/aicitely-com-health-api-openapi.yml
- filename: aicitely-com-public-api-openapi.yml
  format: yaml
  label: Citely Public API
  slug: aicitely-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicitely-com/openapi/aicitely-com-public-api-openapi.yml
auth_types: []
description: Citely uses a single authentication method – an API key sent as an HTTP Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aicitely Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Citely declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Citely
provider_slug: aicitely-com
scheme_count: 1
schemes:
- authorize_url: https://aicitely.com/oauth/authorize
  evidence: 'There is exactly one method: an **API key**, sent as an HTTP bearer credential.'
  header: Authorization
  how_to_obtain: Obtain via the OAuth 2.1 authorization code flow (PKCE) or direct provisioning with a signed‑in human session token.
  location: header
  name: API key
  scopes:
  - read
  token_url: https://aicitely.com/oauth/token
  type: http-bearer
slug: aicitely-com-authentication
source_filename: aicitely-com-authentication.yml
source_heading: Authentication Profile
source_url: https://aicitely.com/auth.md
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://aicitely.com/auth.md\nsources:\n- https://aicitely.com/auth.md\ndescription: Citely uses a single authentication method – an API key sent as an HTTP Bearer token.\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'There is exactly one method: an **API key**, sent as an HTTP bearer credential.'\n  location: header\n  header: Authorization\n  token_url: https://aicitely.com/oauth/token\n  authorize_url: https://aicitely.com/oauth/authorize\n  scopes:\n  - read\n  how_to_obtain: Obtain via the OAuth 2.1 authorization code flow (PKCE) or direct provisioning with a signed‑in human session token.\nnote: No other authentication schemes are documented.\ndocs: https://aicitely.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/aicitely-com/authentication/aicitely-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- BrandCitation
- SEO
- Analytics
---
