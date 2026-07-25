---
api_key_in:
- header
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Eway Authentication
name_suffix: Authentication
oauth_flows: []
overview: eWAY secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: eWAY
provider_slug: eway
scheme_count: 2
schemes:
- description: All server-to-server calls to the Rapid API authenticate with HTTP Basic auth. The eWAY API Key is sent as the username and the matching API Password as the password. Credentials are issued per environment (live vs sandbox) from MYeWAY.
  name: RapidBasicAuth
  scheme: basic
  sources:
  - docs
  type: http
- description: Client-side integrations (Secure Fields, Client Side Encryption, the responsive Secure Panel) authenticate with a public API key rather than the Basic-auth secret, so the card secret never touches the merchant server. Method availability is restricted for public-key auth (see error V6144).
  in: header
  name: RapidPublicApiKey
  sources:
  - docs
  type: apiKey
slug: eway-authentication
source_filename: eway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://eway.io/api-v3/\ndocs: https://eway.io/api-v3/#authentication\nnote: >-\n  No OpenAPI is published by eWAY, so this profile is captured from the Rapid\n  API reference documentation rather than derived from a securitySchemes block.\nsummary:\n  types: [http, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  primary: HTTP Basic authentication\nschemes:\n  - name: RapidBasicAuth\n    type: http\n    scheme: basic\n    description: >-\n      All server-to-server calls to the Rapid API authenticate with HTTP Basic\n      auth. The eWAY API Key is sent as the username and the matching API\n      Password as the password. Credentials are issued per environment (live vs\n      sandbox) from MYeWAY.\n    sources: [docs]\n  - name: RapidPublicApiKey\n    type: apiKey\n    in: header\n    description: >-\n      Client-side integrations (Secure Fields, Client Side Encryption, the\n      responsive Secure Panel) authenticate\
  \ with a public API key rather than\n      the Basic-auth secret, so the card secret never touches the merchant\n      server. Method availability is restricted for public-key auth (see error\n      V6144).\n    sources: [docs]\nrequired_headers:\n  - name: X-EWAY-APIVERSION\n    description: Selects the Rapid API version (current 47; default 31 when omitted).\n    required: false\n  - name: Authorization\n    description: HTTP Basic, base64(APIKey:Password).\n    required: true\noauth: false\nscopes: none\nnotes:\n  - eWAY does not document OAuth 2.0, OpenID Connect, or scoped tokens; there is no scope surface.\n  - Sandbox and live use separate API key/password pairs and separate base hosts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eway/refs/heads/main/authentication/eway-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Card Payments
- Tokenization
- E-commerce
- Recurring Payments
- Subscriptions
---
