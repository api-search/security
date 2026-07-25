---
api_key_in:
- body
auth_types:
- credentials
- jwt
description: ''
kind: authentication
layout: security
method: searched
name: Trust Payments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trust Payments secures its APIs with credentials and jwt across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trust Payments
provider_slug: trust-payments
scheme_count: 2
schemes:
- fields:
    alias: Webservices API username (e.g. an email-style alias) supplied on the outer JSON request.
    password: Webservices API password paired with the alias (exchanged during onboarding; not self-serve).
    sitereference: Site identifier that also selects the test vs live environment.
  location: request body
  name: WebservicesCredentials
  notes: Production Webservices access requires PCI certification, account approval, and credential (key) exchange. The alias/password pair is scoped to one or more sitereferences; a test sitereference targets the test bank.
  scheme: alias-password
  transport: HTTPS POST to https://webservices.securetrading.net/json/
  type: credentials
- bearerFormat: JWT
  location: client-side request generated server-side
  name: JavaScriptLibraryJWT
  notes: The JavaScript Library (ST.js) authorises browser-side tokenisation and hosted card fields with a JSON Web Token minted on the merchant server (see the @trustpayments/jwt-generator package), keeping raw card data off the merchant server and reducing PCI scope. JWT signing uses a site-specific secret; errorcodes 10300-10302 cover JWT decode/encode/algorithm failures.
  scheme: bearer
  type: jwt
slug: trust-payments-authentication
source_filename: trust-payments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://help.trustpayments.com/hc/en-us/articles/11569681677713-Webservices-API-Guide-for-POS-developers\ndocs: https://help.trustpayments.com/hc/en-us/sections/360005821218-Webservices-API\nnote: >-\n  Trust Payments does not publish an OpenAPI definition, so this profile is derived\n  from the published Webservices API and JavaScript Library documentation rather\n  than from spec securitySchemes. Two distinct authentication models exist:\n  server-to-server alias + password credentials for the Webservices (STPP) JSON API,\n  and a server-generated JWT for the client-side JavaScript Library.\nsummary:\n  types: [credentials, jwt]\n  api_key_in: [body]\n  oauth2_flows: []\nschemes:\n  - name: WebservicesCredentials\n    type: credentials\n    scheme: alias-password\n    location: request body\n    fields:\n      alias: Webservices API username (e.g. an email-style alias) supplied on the outer JSON request.\n      password:\
  \ Webservices API password paired with the alias (exchanged during onboarding; not self-serve).\n      sitereference: Site identifier that also selects the test vs live environment.\n    transport: HTTPS POST to https://webservices.securetrading.net/json/\n    notes: >-\n      Production Webservices access requires PCI certification, account approval, and\n      credential (key) exchange. The alias/password pair is scoped to one or more\n      sitereferences; a test sitereference targets the test bank.\n  - name: JavaScriptLibraryJWT\n    type: jwt\n    scheme: bearer\n    bearerFormat: JWT\n    location: client-side request generated server-side\n    notes: >-\n      The JavaScript Library (ST.js) authorises browser-side tokenisation and hosted\n      card fields with a JSON Web Token minted on the merchant server (see the\n      @trustpayments/jwt-generator package), keeping raw card data off the merchant\n      server and reducing PCI scope. JWT signing uses a site-specific secret;\
  \ errorcodes\n      10300-10302 cover JWT decode/encode/algorithm failures.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trust-payments/refs/heads/main/authentication/trust-payments-authentication.yml
summary_line: credentials/jwt · 2 schemes
tags:
- Payments
- United Kingdom
- Payment Gateway
- Payment Processing
- Acquiring
- Card Payments
- Tokenization
- Subscriptions
- 3-D Secure
- Point of Sale
- Webhooks
- Payouts
---
