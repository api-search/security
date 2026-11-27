---
anonymous_access: false
api_key_in: []
api_specs:
- filename: passtru-openapi-generated.yml
  format: yaml
  label: Passtru API
  slug: passtru-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/passtru/openapi/_ae-authored/passtru-openapi-generated.yml
auth_types: []
description: Passtru uses the standard OpenID Connect Authorization Code flow with PKCE (S256) and supports both public and confidential clients.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Passtru Authentication
name_suffix: Authentication
oauth_flows: []
overview: Passtru declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Passtru
provider_slug: passtru
scheme_count: 1
schemes:
- authorize_url: https://login.passtru.io/oauth/v2/authorize
  evidence: Passtru uses the standard OpenID Connect Authorization Code flow with Proof Key for Code Exchange (PKCE).
  flows:
  - authorization_code
  how_to_obtain: Contact developers@passtru.io to register your application and receive a client ID (and client secret for confidential clients).
  name: Passtru OpenID Connect
  scopes:
  - openid
  - email
  - profile
  type: oauth2
slug: passtru-authentication
source_filename: passtru-authentication.yml
source_heading: Authentication Profile
source_url: https://passtru.io/en/developers/authentication
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://passtru.io/en/developers/authentication\nsources:\n- https://passtru.io/en/developers/authentication\n- https://passtru.io/en/developers/nextjs\ndescription: Passtru uses the standard OpenID Connect Authorization Code flow with PKCE (S256) and supports both public and confidential clients.\nschemes:\n- type: oauth2\n  name: Passtru OpenID Connect\n  evidence: Passtru uses the standard OpenID Connect Authorization Code flow with Proof Key for Code Exchange (PKCE).\n  flows:\n  - authorization_code\n  authorize_url: https://login.passtru.io/oauth/v2/authorize\n  scopes:\n  - openid\n  - email\n  - profile\n  how_to_obtain: Contact developers@passtru.io to register your application and receive a client ID (and client secret for confidential clients).\ndocs: https://passtru.io/en/developers/authentication\n"
source_yaml_url: https://artifacts.apis.io/passtru/authentication/passtru-authentication.yml
summary_line: 1 scheme
tags:
- Identity Verification
- Age Verification
- KYC
- Document Verification
- Sanctions Screening
---
