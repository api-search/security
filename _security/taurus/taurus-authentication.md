---
api_key_in: []
auth_types:
- http
- hmac
- openIdConnect
- saml
description: ''
kind: authentication
layout: security
method: searched
name: Taurus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Taurus secures its APIs with http, hmac, openIdConnect, and saml across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Taurus
provider_slug: taurus
scheme_count: 3
schemes:
- description: Bearer access token presented on API requests.
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.taurushq.com/protect-capital/reference/api-structure-and-concepts
  type: http
- description: Requests are signed with an HMAC over the request; a signing/authentication proxy is provided to compute and attach the signature.
  name: hmacRequestSigning
  sources:
  - https://docs.taurushq.com/protect-capital/reference/api-structure-and-concepts
  type: hmac
- description: Governed actions require one or more digital signatures satisfying the tenant's governance ruleset before execution.
  name: governanceDigitalSignatures
  sources:
  - https://docs.taurushq.com/protect-capital/docs/introduction
  type: digital-signature
slug: taurus-authentication
source_filename: taurus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.taurushq.com/protect-capital/reference/api-structure-and-concepts\ndocs: https://docs.taurushq.com/protect-capital/reference/api-structure-and-concepts\nsummary:\n  types: [http, hmac, openIdConnect, saml]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Taurus-PROTECT API calls authenticate with a bearer token and additionally require HMAC\n    request signing (a signing proxy computes the request signature). Sensitive/governed actions\n    (creating a transaction request, initiating staking, etc.) are further authorized by digital\n    signatures under configurable governance rules. Human/console access is federated via SSO.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: Bearer access token presented on API requests.\n    sources: [https://docs.taurushq.com/protect-capital/reference/api-structure-and-concepts]\n  - name: hmacRequestSigning\n    type: hmac\n    description:\
  \ >-\n      Requests are signed with an HMAC over the request; a signing/authentication proxy\n      is provided to compute and attach the signature.\n    sources: [https://docs.taurushq.com/protect-capital/reference/api-structure-and-concepts]\n  - name: governanceDigitalSignatures\n    type: digital-signature\n    description: >-\n      Governed actions require one or more digital signatures satisfying the tenant's\n      governance ruleset before execution.\n    sources: [https://docs.taurushq.com/protect-capital/docs/introduction]\nsso:\n  protocols: [OpenID Connect, SAML]\n  provisioning: SCIM 2.0\n  identity_providers_documented: [Okta, Azure AD]\n  source: https://docs.taurushq.com/protect-capital/docs/introduction-2\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taurus/refs/heads/main/authentication/taurus-authentication.yml
summary_line: http/hmac/openIdConnect/saml · 3 schemes
tags:
- Company
- Digital Assets
- Cryptocurrency
- Custody
- Tokenization
- Blockchain
- Trading
- Financial Services
- FinTech
- Institutional
---
