---
anonymous_access: false
api_key_in: []
api_specs:
- filename: easy2257-com-collab-scenes-api-openapi.yml
  format: yaml
  label: Easy2257 Collab Scenes API
  slug: easy2257-com-collab-scenes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easy2257-com/openapi/easy2257-com-collab-scenes-api-openapi.yml
- filename: easy2257-com-hosted-attestation-api-openapi.yml
  format: yaml
  label: Easy2257 Hosted Attestation API
  slug: easy2257-com-hosted-attestation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easy2257-com/openapi/easy2257-com-hosted-attestation-api-openapi.yml
- filename: easy2257-com-productions-api-openapi.yml
  format: yaml
  label: Easy2257 Productions API
  slug: easy2257-com-productions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easy2257-com/openapi/easy2257-com-productions-api-openapi.yml
- filename: easy2257-com-solo-accounts-api-openapi.yml
  format: yaml
  label: Easy2257 Solo Accounts API
  slug: easy2257-com-solo-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easy2257-com/openapi/easy2257-com-solo-accounts-api-openapi.yml
- filename: easy2257-com-talent-api-openapi.yml
  format: yaml
  label: Easy2257 Talent API
  slug: easy2257-com-talent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easy2257-com/openapi/easy2257-com-talent-api-openapi.yml
auth_types: []
description: Authentication schemes as published on the provider's pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Easy2257 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Easy2257 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Easy2257
provider_slug: easy2257-com
scheme_count: 1
schemes:
- authorize_url: https://easy2257.com/oauth/authorize
  evidence: '"authorization_endpoint":"https://easy2257.com/oauth/authorize"'
  flows:
  - authorization_code
  - refresh_token
  name: OAuth2
  scopes:
  - mcp:read
  type: oauth2
slug: easy2257-com-authentication
source_filename: easy2257-com-authentication.yml
source_heading: Authentication Profile
source_url: https://easy2257.com/auth/login?callbackUrl=https%3A%2F%2Fpartner.easy2257.com
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://easy2257.com/auth/login?callbackUrl=https%3A%2F%2Fpartner.easy2257.com\nsources:\n- https://easy2257.com/auth/login?callbackUrl=https%3A%2F%2Fpartner.easy2257.com\n- https://easy2257.com/auth/login?callbackUrl=/profile\n- https://easy2257.com/.well-known/oauth-authorization-server\n- https://easy2257.com/.well-known/oauth-protected-resource\ndescription: Authentication schemes as published on the provider's pages.\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: '\"authorization_endpoint\":\"https://easy2257.com/oauth/authorize\"'\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://easy2257.com/oauth/authorize\n  scopes:\n  - mcp:read\ndocs: https://easy2257.com/auth/login?callbackUrl=https%3A%2F%2Fpartner.easy2257.com\n"
source_yaml_url: https://artifacts.apis.io/easy2257-com/authentication/easy2257-com-authentication.yml
summary_line: 1 scheme
tags:
- Compliance
- Records
- Adult Content
- Software
- Platform
---
