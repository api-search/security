---
anonymous_access: false
api_key_in: []
api_specs:
- filename: factuarea-com-openapi-generated.yml
  format: yaml
  label: Factuarea API
  slug: factuarea-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/factuarea-com/openapi/_ae-authored/factuarea-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Factuarea API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Factuarea Authentication
name_suffix: Authentication
oauth_flows: []
overview: Factuarea declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Factuarea
provider_slug: factuarea-com
scheme_count: 1
schemes:
- evidence: For agent integrations and third‑party apps that act on behalf of a Factuarea user, the API also supports the OAuth 2.1 authorization‑code flow with PKCE (code_challenge_method=S256) as an alternative to a static API key.
  how_to_obtain: Register an OAuth client and follow the authorization‑code flow as described in the discovery metadata at /.well-known/oauth-authorization-server.
  name: OAuth 2.1
  type: oauth2
slug: factuarea-com-authentication
source_filename: factuarea-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.factuarea.com/guides/authentication
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.factuarea.com/guides/authentication\nsources:\n- https://docs.factuarea.com/guides/authentication\n- https://docs.factuarea.com/api-reference/account/public-api.v1.account.api_keys.update_nif_scope\n- https://docs.factuarea.com/api-reference/account/public-api.v1.account.api_keys.create\n- https://docs.factuarea.com/api-reference/account/public-api.v1.account.api_keys.list\ndescription: Authentication methods for Factuarea API\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: For agent integrations and third‑party apps that act on behalf of a Factuarea user, the API also supports the OAuth 2.1 authorization‑code\n    flow with PKCE (code_challenge_method=S256) as an alternative to a static API key.\n  how_to_obtain: Register an OAuth client and follow the authorization‑code flow as described in the discovery metadata at /.well-known/oauth-authorization-server.\n\
  docs: https://docs.factuarea.com/guides/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/factuarea-com/authentication/factuarea-com-authentication.yml
summary_line: 1 scheme
tags:
- Invoicing
- Software
- Spain
- Fintech
- Software-as-a-Service
---
