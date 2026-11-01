---
anonymous_access: false
api_key_in: []
api_specs:
- filename: talopay-openapi-generated.yml
  format: yaml
  label: Talo Pay API
  slug: talopay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/talopay/openapi/_ae-authored/talopay-openapi-generated.yml
auth_types: []
description: Authentication methods for Talo Pay API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Talopay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Talo Pay declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Talo Pay
provider_slug: talopay
scheme_count: 2
schemes:
- authorize_url: https://app.talo.com.ar/authorize/{partner_id}?referred_user_id={external_user_id}
  evidence: Una vez que el usuario confirma, Talo lo redirigirá a la url de redirección que proporcionaste, con un code en el query string.
  flows:
  - authorization_code
  how_to_obtain: Create partner credentials (partner_id and client_secret) in the sandbox form, then redirect the user to the authorize URL to obtain a code, and exchange the code for an access token via POST to https://sandbox-api.talo.com.ar/auth/tokens.
  name: OAuth2 Authorization Code
  type: oauth2
- evidence: Una vez que tienes un token de autenticación, debes incluirlo en el encabezado Authorization de todas las solicitudes a nuestra API, utilizando el esquema “Bearer”.
  how_to_obtain: POST to https://api.talo.com.ar/users/:user_id/tokens with client_id and client_secret in the JSON body to receive a token, then include it in the Authorization header as "Bearer <token>".
  name: Bearer Token
  type: http-bearer
slug: talopay-authentication
source_filename: talopay-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.talo.com.ar/partners/authentication
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.talo.com.ar/partners/authentication\nsources:\n- https://docs.talo.com.ar/partners/authentication\n- https://docs.talo.com.ar/ecommerce/API/API_Reference/authentication\n- https://docs.talo.com.ar/getting_started\n- https://docs.talo.com.ar/ecommerce/API/getting_started\ndescription: Authentication methods for Talo Pay API\nschemes:\n- type: oauth2\n  name: OAuth2 Authorization Code\n  evidence: Una vez que el usuario confirma, Talo lo redirigirá a la url de redirección que proporcionaste, con un code en el query string.\n  flows:\n  - authorization_code\n  authorize_url: https://app.talo.com.ar/authorize/{partner_id}?referred_user_id={external_user_id}\n  how_to_obtain: Create partner credentials (partner_id and client_secret) in the sandbox form, then redirect the user to the authorize URL to\n    obtain a code, and exchange the code for an access token via POST to\
  \ https://sandbox-api.talo.com.ar/auth/tokens.\n- type: http-bearer\n  name: Bearer Token\n  evidence: Una vez que tienes un token de autenticación, debes incluirlo en el encabezado Authorization de todas las solicitudes a nuestra API,\n    utilizando el esquema “Bearer”.\n  how_to_obtain: POST to https://api.talo.com.ar/users/:user_id/tokens with client_id and client_secret in the JSON body to receive a token, then\n    include it in the Authorization header as \"Bearer <token>\".\ndocs: https://docs.talo.com.ar/partners/authentication\n"
source_yaml_url: https://artifacts.apis.io/talopay/authentication/talopay-authentication.yml
summary_line: 2 schemes
tags:
- Fintech
- Payments
- Argentina
- E-commerce
- Bank Transfers
---
