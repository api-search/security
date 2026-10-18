---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fiskil-auth-api-openapi.yml
  format: yaml
  label: FISKIL Auth API
  slug: fiskil-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-auth-api-openapi.yml
- filename: fiskil-banking-api-openapi.yml
  format: yaml
  label: FISKIL Banking API
  slug: fiskil-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-banking-api-openapi.yml
- filename: fiskil-common-api-openapi.yml
  format: yaml
  label: FISKIL Common API
  slug: fiskil-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-common-api-openapi.yml
- filename: fiskil-consent-api-openapi.yml
  format: yaml
  label: FISKIL Consent API
  slug: fiskil-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-consent-api-openapi.yml
- filename: fiskil-end-users-api-openapi.yml
  format: yaml
  label: FISKIL End users API
  slug: fiskil-end-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-end-users-api-openapi.yml
- filename: fiskil-energy-api-openapi.yml
  format: yaml
  label: FISKIL Energy API
  slug: fiskil-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-energy-api-openapi.yml
- filename: fiskil-institutions-api-openapi.yml
  format: yaml
  label: FISKIL Institutions API
  slug: fiskil-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-institutions-api-openapi.yml
- filename: fiskil-transactions-api-openapi.yml
  format: yaml
  label: FISKIL Transactions API
  slug: fiskil-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/openapi/fiskil-transactions-api-openapi.yml
auth_types: []
description: Fiskil uses OAuth2 client‑credentials flow to obtain a bearer token which must be sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fiskil Authentication
name_suffix: Authentication
oauth_flows: []
overview: FISKIL declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FISKIL
provider_slug: fiskil
scheme_count: 1
schemes:
- evidence: To access the Fiskil API, all requests must be authenticated using a bearer token. This token is obtained by exchanging your API credentials ( client_id and client_secret ) via the /v1/token endpoint.
  flows:
  - client_credentials
  how_to_obtain: Generate client_id and client_secret in the Fiskil Developer Console, then POST them to the token endpoint to receive a token.
  name: Fiskil OAuth2
  token_url: https://api.fiskil.com/v1/token
  type: oauth2
slug: fiskil-authentication
source_filename: fiskil-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fiskil.com/data-api/api-reference/authentication
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fiskil.com/data-api/api-reference/authentication\nsources:\n- https://docs.fiskil.com/data-api/api-reference/authentication\n- https://docs.fiskil.com/data-api/guides/getting-started/authentication\n- https://docs.fiskil.com/data-api/api-reference/auth-session\n- https://docs.fiskil.com/data-api/guides/core-concepts/auth-sessions\ndescription: Fiskil uses OAuth2 client‑credentials flow to obtain a bearer token which must be sent in the Authorization header.\nschemes:\n- type: oauth2\n  name: Fiskil OAuth2\n  evidence: To access the Fiskil API, all requests must be authenticated using a bearer token. This token is obtained by exchanging your API credentials\n    ( client_id and client_secret ) via the /v1/token endpoint.\n  flows:\n  - client_credentials\n  token_url: https://api.fiskil.com/v1/token\n  how_to_obtain: Generate client_id and client_secret in the Fiskil\
  \ Developer Console, then POST them to the token endpoint to receive a token.\nnote: All subsequent API requests must include the token in the Authorization header as \"Bearer {access_token}\".\ndocs: https://docs.fiskil.com/data-api/api-reference/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiskil/refs/heads/main/authentication/fiskil-authentication.yml
summary_line: 1 scheme
tags:
- Open Banking
- Data Sharing
- Financial Services
- API Platform
- North America
---
