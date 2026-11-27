---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 24sevenoffice-openapi-generated.yml
  format: yaml
  label: Finago API
  slug: 24sevenoffice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/24sevenoffice/openapi/_ae-authored/24sevenoffice-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Finago Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finago declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Finago
provider_slug: 24sevenoffice
scheme_count: 1
schemes:
- evidence: 'grant_type'': ''client_credentials'''
  flows:
  - client_credentials
  how_to_obtain: Obtain a client ID, client secret, and organization ID (login_organization) from Finago, then request a token from the token URL using the client_credentials grant.
  name: OAuth2 Client Credentials
  token_url: https://login.24sevenoffice.com/oauth/token
  type: oauth2
slug: 24sevenoffice-authentication
source_filename: 24sevenoffice-authentication.yml
source_heading: Authentication Profile
source_url: https://finago.no/developer/implement-access-token
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://finago.no/developer/implement-access-token\nsources:\n- https://finago.no/developer/implement-access-token\n- https://finago.no/developer/obtain-access-token-python\nschemes:\n- type: oauth2\n  name: OAuth2 Client Credentials\n  evidence: 'grant_type'': ''client_credentials'''\n  flows:\n  - client_credentials\n  token_url: https://login.24sevenoffice.com/oauth/token\n  how_to_obtain: Obtain a client ID, client secret, and organization ID (login_organization) from Finago, then request a token from the token\n    URL using the client_credentials grant.\nnote: Credentials are sent in the request body as JSON and the resulting access token is used in the 'Authorization' header as a Bearer token.\ndocs: https://finago.no/developer/implement-access-token\n"
source_yaml_url: https://artifacts.apis.io/24sevenoffice/authentication/24sevenoffice-authentication.yml
summary_line: 1 scheme
tags:
- Accounting
- Payroll
- Business Management
- Norway
- Sweden
- Finland
---
