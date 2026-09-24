---
anonymous_access: false
api_key_in: []
api_specs:
- filename: terna-openapi-generated.yml
  format: yaml
  label: Terna API
  slug: terna-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terna/refs/heads/main/openapi/_ae-authored/terna-openapi-generated.yml
auth_types: []
description: Terna uses OAuth2 client credentials flow to obtain access tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Terna Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terna declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Terna
provider_slug: terna
scheme_count: 1
schemes:
- evidence: Access to our services is controlled by tokens for via Oauth2.0. To obtain a token you must invoke the associated endpoint and provide your client key and client secret.
  flows:
  - client_credentials
  how_to_obtain: Create an application to receive a client_id (client key) and client_secret, then POST them with grant_type=client_credentials to the token endpoint.
  name: OAuth2 Client Credentials
  token_url: https://api.terna.it/public-api/access-token
  type: oauth2
slug: terna-authentication
source_filename: terna-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.terna.it/docs/read/Access_Token
source_yaml: "generated: '2026-09-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.terna.it/docs/read/Access_Token\nsources:\n- https://developer.terna.it/docs/read/Access_Token\n- https://developer.terna.it/docs/read/Getting_Started\n- https://developer.terna.it/docs/read/getting_started/Oauth2\n- https://developer.terna.it/docs/read/getting_started/OIDC\ndescription: Terna uses OAuth2 client credentials flow to obtain access tokens.\nschemes:\n- type: oauth2\n  name: OAuth2 Client Credentials\n  evidence: Access to our services is controlled by tokens for via Oauth2.0. To obtain a token you must invoke the associated endpoint and provide\n    your client key and client secret.\n  flows:\n  - client_credentials\n  token_url: https://api.terna.it/public-api/access-token\n  how_to_obtain: Create an application to receive a client_id (client key) and client_secret, then POST them with grant_type=client_credentials\n    to the token endpoint.\n\
  docs: https://developer.terna.it/docs/read/Access_Token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terna/refs/heads/main/authentication/terna-authentication.yml
summary_line: 1 scheme
tags:
- Energy
- Transmission
- Infrastructure
- Italy
- Renewable
---
