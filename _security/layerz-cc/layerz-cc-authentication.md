---
anonymous_access: false
api_key_in: []
api_specs:
- filename: layerz-cc-openapi-generated.yml
  format: yaml
  label: Layerz API
  slug: layerz-cc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layerz-cc/openapi/_ae-authored/layerz-cc-openapi-generated.yml
auth_types: []
description: Authentication methods for Layerz REST API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Layerz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Layerz declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Layerz
provider_slug: layerz-cc
scheme_count: 2
schemes:
- evidence: "Every request carries a Bearer token: \n Authorization: Bearer lz_0123456789abcdef0123456789abcdef01234567"
  header: Authorization
  how_to_obtain: 'Created in the app: account menu, then API. A key is lz_ followed by 40 hex characters, shown once, and stored hashed.'
  location: header
  name: Bearer
  type: http-bearer
- evidence: 'Applications that act for other users use OAuth 2.1 with PKCE: dynamic client registration, the authorization endpoint, then the token endpoint.'
  header: Authorization
  how_to_obtain: Dynamic client registration via discovery documents served at /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource.
  location: header
  name: OAuth 2.1 with PKCE
  type: oauth2
slug: layerz-cc-authentication
source_filename: layerz-cc-authentication.yml
source_heading: Authentication Profile
source_url: https://layerz.cc/docs/api/authentication
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://layerz.cc/docs/api/authentication\nsources:\n- https://layerz.cc/docs/api/authentication\n- https://layerz.cc/docs/get-started/quickstart-api\n- https://layerz.cc/blog/token-efficiency-finance-ai\n- https://layerz.cc/blog/save-tokens-building-financial-models-with-ai\ndescription: Authentication methods for Layerz REST API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: \"Every request carries a Bearer token: \\n Authorization: Bearer lz_0123456789abcdef0123456789abcdef01234567\"\n  location: header\n  header: Authorization\n  how_to_obtain: 'Created in the app: account menu, then API. A key is lz_ followed by 40 hex characters, shown once, and stored hashed.'\n- type: oauth2\n  name: OAuth 2.1 with PKCE\n  evidence: 'Applications that act for other users use OAuth 2.1 with PKCE: dynamic client registration, the authorization endpoint, then the\n    token endpoint.'\n\
  \  location: header\n  header: Authorization\n  how_to_obtain: Dynamic client registration via discovery documents served at /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource.\ndocs: https://layerz.cc/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/layerz-cc/authentication/layerz-cc-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Spreadsheets
- Artificial Intelligence
- CFO
- FP&A
---
