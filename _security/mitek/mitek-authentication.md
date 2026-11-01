---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mitek Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mitek declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mitek
provider_slug: mitek
scheme_count: 1
schemes:
- description: Mitek uses OAuth 2.0 with JWT tokens for authorization. The client credential flow is used for server-to-server communication where a client_id and client_secret are issued. Tokens are valid for 5 minutes from issuance.
  documentation: 'Token retrieval requires a basic POST request to our OAuth 2.0 based authentication server.

    Mitek recommends that developers pro-actively refresh tokens to ensure a valid token is always available for submission to the API.


    In the authentication request, scopes must be included that the token will provide permissions to access.

    The token generated will only provide access to the specific operations for which the scope was requested.

    Mitek recommends that the token is requested with only the scopes that are minimally required to perform a specific operation.'
  flow: client_credentials
  name: OAuth 2.0 Client Credentials
  scopes:
  - standard.scope
  - additional.scope
  token_url: /connect/token
  type: oauth2
slug: mitek-authentication
source_filename: mitek-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: searched\nsource: https://docs.us.mitekcloud.com/#authentication\ndocs: https://docs.us.mitekcloud.com/#authentication\nschemes:\n  - type: oauth2\n    name: OAuth 2.0 Client Credentials\n    description: Mitek uses OAuth 2.0 with JWT tokens for authorization. The client credential flow is used for server-to-server communication where a client_id and client_secret are issued. Tokens are valid for 5 minutes from issuance.\n    flow: client_credentials\n    token_url: /connect/token\n    scopes:\n      - standard.scope\n      - additional.scope\n    documentation: |\n      Token retrieval requires a basic POST request to our OAuth 2.0 based authentication server.\n      Mitek recommends that developers pro-actively refresh tokens to ensure a valid token is always available for submission to the API.\n      \n      In the authentication request, scopes must be included that the token will provide permissions to access.\n      The token generated\
  \ will only provide access to the specific operations for which the scope was requested.\n      Mitek recommends that the token is requested with only the scopes that are minimally required to perform a specific operation."
source_yaml_url: https://artifacts.apis.io/mitek/authentication/mitek-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Identity Verification
- Fraud Prevention
- Biometric Authentication
- KYC
- Check Fraud
- Financial Services
---
