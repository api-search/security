---
anonymous_access: false
api_key_in: []
api_specs:
- filename: immich-openapi-generated.yml
  format: yaml
  label: Immich API
  slug: immich-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immich/openapi/_ae-authored/immich-openapi-generated.yml
auth_types: []
description: Immich supports authentication via OpenID Connect (OIDC), which is built on top of OAuth2.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Immich Authentication
name_suffix: Authentication
oauth_flows: []
overview: Immich declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Immich
provider_slug: immich
scheme_count: 1
schemes:
- evidence: Immich supports 3rd party authentication via OpenID Connect (OIDC), an identity layer built on top of OAuth2.
  flows:
  - authorization_code
  how_to_obtain: Create a new confidential web client in the external identity provider with the Authorization Code grant type, then configure the issuer_url, client_id, client_secret, and scope in Immich’s Administration Settings.
  name: OpenID Connect
  scopes:
  - openid
  - email
  - profile
  type: oauth2
slug: immich-authentication
source_filename: immich-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.immich.app/administration/oauth/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.immich.app/administration/oauth/\nsources:\n- https://docs.immich.app/administration/oauth/\n- https://docs.immich.app/developer/setup/\n- https://docs.immich.app/overview/quick-start/\ndescription: Immich supports authentication via OpenID Connect (OIDC), which is built on top of OAuth2.\nschemes:\n- type: oauth2\n  name: OpenID Connect\n  evidence: Immich supports 3rd party authentication via OpenID Connect (OIDC), an identity layer built on top of OAuth2.\n  flows:\n  - authorization_code\n  scopes:\n  - openid\n  - email\n  - profile\n  how_to_obtain: Create a new confidential web client in the external identity provider with the Authorization Code grant type, then configure\n    the issuer_url, client_id, client_secret, and scope in Immich’s Administration Settings.\ndocs: https://docs.immich.app/administration/oauth/\n"
source_yaml_url: https://artifacts.apis.io/immich/authentication/immich-authentication.yml
summary_line: 1 scheme
tags:
- Self-Hosted
- Photo Management
- Video Management
- Privacy
- Open Source
---
