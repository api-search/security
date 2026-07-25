---
api_key_in: []
auth_types:
- mutualTLS
- http
- oauth2
description: 'American Express developer APIs are onboarding-gated and secured with a layered scheme: mutual TLS (two-way client-certificate authentication), request-level HMAC message authentication (MAC) signatures, and OAuth 2.0 bearer tokens for authorization. No public OpenAPI is published, so this profile is captured from the Amex for Developers API Security documentation rather than derived from a machine-readable spec.'
kind: authentication
layout: security
method: searched
name: American Express Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: American Express secures its APIs with mutualTLS, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: American Express
provider_slug: american-express
scheme_count: 3
schemes:
- description: Two-way TLS. Partners are issued client certificates during onboarding and must present them on every API call; American Express validates the client certificate alongside the server certificate.
  docs: https://developer.americanexpress.com/documentation/api-security/certificates
  name: mutualTLS
  type: mutualTLS
- description: HMAC / Message Authentication Code (MAC) request signing. Each request carries an Authorization header containing an HMAC signature computed over the request using the partner's issued MAC ID and secret, protecting message integrity and authenticity.
  docs: https://developer.americanexpress.com/documentation/api-security/hmac
  name: hmac
  scheme: hmac
  type: http
- description: OAuth 2.0 access tokens are used for authorization on APIs that require them; tokens are obtained via the Amex token endpoint and presented as bearer credentials. Scope and grant details are provisioned per partner onboarding.
  docs: https://developer.americanexpress.com/documentation/api-security/oauth-2
  flows:
  - flow: clientCredentials
  name: oauth2
  scheme: bearer
  type: oauth2
slug: american-express-authentication
source_filename: american-express-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.americanexpress.com/documentation/api-security\ndocs:\n  - https://developer.americanexpress.com/documentation/api-security/certificates\n  - https://developer.americanexpress.com/documentation/api-security/hmac\n  - https://developer.americanexpress.com/documentation/api-security/oauth-2\ndescription: >-\n  American Express developer APIs are onboarding-gated and secured with a\n  layered scheme: mutual TLS (two-way client-certificate authentication),\n  request-level HMAC message authentication (MAC) signatures, and OAuth 2.0\n  bearer tokens for authorization. No public OpenAPI is published, so this\n  profile is captured from the Amex for Developers API Security documentation\n  rather than derived from a machine-readable spec.\nsummary:\n  types: [mutualTLS, http, oauth2]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\nschemes:\n  - name: mutualTLS\n    type: mutualTLS\n    description: >-\n \
  \     Two-way TLS. Partners are issued client certificates during onboarding and\n      must present them on every API call; American Express validates the client\n      certificate alongside the server certificate.\n    docs: https://developer.americanexpress.com/documentation/api-security/certificates\n  - name: hmac\n    type: http\n    scheme: hmac\n    description: >-\n      HMAC / Message Authentication Code (MAC) request signing. Each request\n      carries an Authorization header containing an HMAC signature computed over\n      the request using the partner's issued MAC ID and secret, protecting\n      message integrity and authenticity.\n    docs: https://developer.americanexpress.com/documentation/api-security/hmac\n  - name: oauth2\n    type: oauth2\n    scheme: bearer\n    description: >-\n      OAuth 2.0 access tokens are used for authorization on APIs that require\n      them; tokens are obtained via the Amex token endpoint and presented as\n      bearer credentials. Scope\
  \ and grant details are provisioned per partner\n      onboarding.\n    docs: https://developer.americanexpress.com/documentation/api-security/oauth-2\n    flows:\n      - flow: clientCredentials\nnotes:\n  - Client SDKs (packages/american-express-packages.yml) implement the mTLS + HMAC\n    request-signing so partners do not hand-roll the signature.\n  - Access is partner-gated; credentials, certificates, and MAC secrets are issued\n    during onboarding rather than self-service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-express/refs/heads/main/authentication/american-express-authentication.yml
summary_line: mutualTLS/http/oauth2 · 3 schemes
tags:
- Credit Cards
- Financial Services
- Payments
- Card Network
- Tokenization
- Fraud Prevention
- Open Banking
- Rewards
- United States
- Fortune 100
---
