---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kwnva-design-catalog-api-openapi.yml
  format: yaml
  label: kwnva.design Catalog API
  slug: kwnva-design-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kwnva-design/openapi/kwnva-design-catalog-api-openapi.yml
- filename: kwnva-design-inquiries-api-openapi.yml
  format: yaml
  label: kwnva.design Inquiries API
  slug: kwnva-design-inquiries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kwnva-design/openapi/kwnva-design-inquiries-api-openapi.yml
- filename: kwnva-design-meta-api-openapi.yml
  format: yaml
  label: kwnva.design Meta API
  slug: kwnva-design-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kwnva-design/openapi/kwnva-design-meta-api-openapi.yml
auth_types: []
description: Authentication methods for kwnva.design
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: kwnva.design Authentication
name_suffix: Authentication
oauth_flows: []
overview: kwnva.design declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: kwnva.design
provider_slug: kwnva-design
scheme_count: 2
schemes:
- evidence: Register at POST /oauth/register , then POST /oauth/token with grant_type=client_credentials .
  flows:
  - client_credentials
  how_to_obtain: Register a public client via POST https://kwnva.design/oauth/register and request a token with grant_type=client_credentials.
  name: OAuth2 client_credentials
  scopes:
  - catalog:read
  - inquiries:write
  - sandbox:write
  token_url: https://kwnva.design/oauth/token
  type: oauth2
- evidence: Use the key as a bearer token for attributed writes.
  header: Authorization
  how_to_obtain: POST https://kwnva.design/api/v1/keys (or GET) to mint a free API key.
  location: header
  name: Free API key
  type: http-bearer
slug: kwnva-design-authentication
source_filename: kwnva-design-authentication.yml
source_heading: Authentication Profile
source_url: https://kwnva.design/auth.md
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kwnva.design/auth.md\nsources:\n- https://kwnva.design/auth.md\n- https://kwnva.design/onboarding\n- https://kwnva.design/api/v1/keys.md\n- https://kwnva.design/auth\ndescription: Authentication methods for kwnva.design\nschemes:\n- type: oauth2\n  name: OAuth2 client_credentials\n  evidence: Register at POST /oauth/register , then POST /oauth/token with grant_type=client_credentials .\n  flows:\n  - client_credentials\n  token_url: https://kwnva.design/oauth/token\n  scopes:\n  - catalog:read\n  - inquiries:write\n  - sandbox:write\n  how_to_obtain: Register a public client via POST https://kwnva.design/oauth/register and request a token with grant_type=client_credentials.\n- type: http-bearer\n  name: Free API key\n  evidence: Use the key as a bearer token for attributed writes.\n  location: header\n  header: Authorization\n  how_to_obtain: POST https://kwnva.design/api/v1/keys\
  \ (or GET) to mint a free API key.\ndocs: https://kwnva.design/auth.md\n"
source_yaml_url: https://artifacts.apis.io/kwnva-design/authentication/kwnva-design-authentication.yml
summary_line: 2 schemes
tags:
- Design
- Branding
- 3D Art
- UI/UX
- Studio
---
