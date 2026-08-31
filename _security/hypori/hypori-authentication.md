---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Hypori Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hypori declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hypori
provider_slug: hypori
scheme_count: 2
schemes:
- description: An administrator-role account is issued a ".p12" client certificate file and passphrase by the customer's Hypori Site Administrator. The certificate is presented on the TLS handshake (curl --cert mycert.p12:passphrase). Clients that require PEM can convert with "openssl pkcs12 -in mycert.p12 -out mycert.pem -nodes".
  documented: true
  id: admin_client_certificate
  issued_by: customer Hypori Site Administrator
  self_service: false
  transport: https
  type: mutualTLS
- description: Session token returned in the JSON body ("token" field) of a bodyless POST to /api/v2/authenticate/adminuilogin made with the client certificate. Included in the X-AUTH-TOKEN HTTP header on all subsequent Management API requests.
  documented: true
  id: x_auth_token
  in: header
  name: X-AUTH-TOKEN
  type: apiKey
slug: hypori-authentication
source_filename: hypori-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://docs.hypori.com/Configure/managementAPI\ndocs: https://docs.hypori.com/Configure/managementAPI\napi: Hypori Management API\nnote: >-\n  Derived from Hypori's own published Management API page, not from a specification —\n  Hypori publishes no OpenAPI, so there are no securitySchemes to read. Everything below is\n  stated verbatim in the documentation. The Hypori client app (end-user side) and the admin\n  console use a separate, related certificate model documented at\n  https://docs.hypori.com/Plan/integration.\nsummary: >-\n  Two-step administrator authentication: mutual TLS with a .p12 client certificate issued by\n  the customer's Hypori Site Administrator, exchanged once for a bearer-style token that is\n  then carried in a proprietary X-AUTH-TOKEN header on every subsequent request.\nschemes:\n- id: admin_client_certificate\n  type: mutualTLS\n  transport: https\n  description: >-\n    An administrator-role account\
  \ is issued a \".p12\" client certificate file and passphrase by\n    the customer's Hypori Site Administrator. The certificate is presented on the TLS handshake\n    (curl --cert mycert.p12:passphrase). Clients that require PEM can convert with\n    \"openssl pkcs12 -in mycert.p12 -out mycert.pem -nodes\".\n  issued_by: customer Hypori Site Administrator\n  self_service: false\n  documented: true\n- id: x_auth_token\n  type: apiKey\n  in: header\n  name: X-AUTH-TOKEN\n  description: >-\n    Session token returned in the JSON body (\"token\" field) of a bodyless POST to\n    /api/v2/authenticate/adminuilogin made with the client certificate. Included in the\n    X-AUTH-TOKEN HTTP header on all subsequent Management API requests.\n  documented: true\ntoken_endpoint:\n  method: POST\n  path: /api/v2/authenticate/adminuilogin\n  request_body: none\n  response_field: token\n  documented_example: |\n    curl --cert mycert.p12:passphrase --request POST \\\n      'https://mgmt.example.com:443/api/v2/authenticate/adminuilogin'\n\
  oauth2: false\nopenid_connect: false\napi_keys: false\nscopes:\n  model: role-based\n  note: >-\n    Access is granted to accounts holding the Administrator role; Hypori documents no OAuth\n    scopes and no scope/permission reference page, so no scopes/ artifact is emitted.\ntoken_lifetime: not documented\nrefresh: not documented\nrotation: not documented\nmfa:\n  admin_console: >-\n    Administrators authenticate to the Hypori Admin Console with the same p12 certificate\n    uploaded to the browser, or with a Common Access Card (CAC) and reader.\n  end_user_client: >-\n    The Hypori client app uses certificate-based (mTLS) authentication with a certificate\n    minted on first connect; TOTP and biometric secondary authentication are configurable.\n  source: https://docs.hypori.com/Plan/integration\ngaps:\n- No OpenAPI securitySchemes published, so the auth model cannot be machine-verified.\n- Token lifetime, refresh and revocation semantics are not documented.\n- No self-service credential\
  \ issuance; certificates come from the Site Administrator.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hypori/refs/heads/main/authentication/hypori-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Security
- Mobile
- Virtualization
- Zero Trust
- BYOD
- Government
- Defense
- Compliance
- Identity
- Software-as-a-Service
---
