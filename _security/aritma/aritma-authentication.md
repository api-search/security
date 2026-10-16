---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aritma-openapi-generated.yml
  format: yaml
  label: Aritma API
  slug: aritma-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aritma/refs/heads/main/openapi/_ae-authored/aritma-openapi-generated.yml
auth_types: []
description: Aritma APIs use OpenID Connect / OAuth 2.0 client credentials flow. Clients obtain an access token by POSTing client_id and client_secret to the token endpoint and then send the token in the Authorization header as a Bearer token.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Aritma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aritma declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Aritma
provider_slug: aritma
scheme_count: 2
schemes:
- evidence: The Data Gateway API uses OpenID Connect with the OAuth 2.0 standard for authenticating access tokens.
  flows:
  - client_credentials
  how_to_obtain: POST client_id and client_secret (and optional scope) to the token endpoint using application/x-www-form-urlencoded.
  name: Data Gateway OAuth2
  scopes:
  - api
  token_url: https://id.aritma.io/connect/token
  type: oauth2
- evidence: The Banking API uses OpenID Connect with the OAuth 2.0 standard for authenticating access tokens.
  flows:
  - client_credentials
  how_to_obtain: POST client_id and client_secret (and optional scope) to the token endpoint using application/x-www-form-urlencoded, replacing {tenantId} with your tenant ID.
  name: Banking API OAuth2
  scopes:
  - api
  token_url: https://id.aritma.io/{tenantId}/connect/token
  type: oauth2
slug: aritma-authentication
source_filename: aritma-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.aritma.com/apis/platform/ids/acr_values.md
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.aritma.com/apis/platform/ids/acr_values.md\nsources:\n- https://developer.aritma.com/apis/platform/ids/acr_values.md\n- https://developer.aritma.com/apis/banking/data-gateway/development/authentication.md\n- https://developer.aritma.com/apis/banking/v3/development/2-authentication.md\n- https://developer.aritma.com/apis/banking/v4/development/authentication.md\ndescription: Aritma APIs use OpenID Connect / OAuth 2.0 client credentials flow. Clients obtain an access token by POSTing client_id and client_secret\n  to the token endpoint and then send the token in the Authorization header as a Bearer token.\nschemes:\n- type: oauth2\n  name: Data Gateway OAuth2\n  evidence: The Data Gateway API uses OpenID Connect with the OAuth 2.0 standard for authenticating access tokens.\n  flows:\n  - client_credentials\n  token_url: https://id.aritma.io/connect/token\n  scopes:\n\
  \  - api\n  how_to_obtain: POST client_id and client_secret (and optional scope) to the token endpoint using application/x-www-form-urlencoded.\n- type: oauth2\n  name: Banking API OAuth2\n  evidence: The Banking API uses OpenID Connect with the OAuth 2.0 standard for authenticating access tokens.\n  flows:\n  - client_credentials\n  token_url: https://id.aritma.io/{tenantId}/connect/token\n  scopes:\n  - api\n  how_to_obtain: POST client_id and client_secret (and optional scope) to the token endpoint using application/x-www-form-urlencoded, replacing\n    {tenantId} with your tenant ID.\nnote: 'All APIs require the access token to be sent in the HTTP Authorization header as: Authorization: Bearer <token>. 1 extracted row(s) were\n  dropped because their quote was not on the page.'\ndocs: https://developer.aritma.com/apis/platform/ids/acr_values.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aritma/refs/heads/main/authentication/aritma-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- Automation
- B2B
- Payments
---
