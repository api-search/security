---
api_key_in: []
auth_types:
- oauth1
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lexisnexis Risk Solutions Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: LexisNexis Risk Solutions secures its APIs with oauth1 and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: LexisNexis Risk Solutions
provider_slug: lexisnexis-risk-solutions
scheme_count: 2
schemes:
- credentials:
  - Account SID (consumer key)
  - Auth token (consumer secret)
  deprecated_signature_methods:
  - HMAC-SHA1
  evidence: Emailage_Python/emailage/client.py hard-codes ApiDomains.sandbox = https://sandbox.emailage.com and ApiDomains.production = https://api.emailage.com; Emailage_Go/README.md states the package no longer supports HMAC-SHA1 and recommends HMAC-SHA256/384/512.
  hosts:
    production: https://api.emailage.com
    sandbox: https://sandbox.emailage.com
  name: EmailageOAuth1
  product: LexisNexis Emailage
  signature_methods:
  - HMAC-SHA256
  - HMAC-SHA384
  - HMAC-SHA512
  sources:
  - https://github.com/lexisnexis-risk-solutions/emailage-public-clients/tree/main/Emailage_Python
  - https://github.com/lexisnexis-risk-solutions/emailage-public-clients/tree/main/Emailage_Go
  type: oauth1
- evidence: Emailage_Go/emailage.go defines Endpoint + TokenEndpoint and an OAUTH2 AuthType; Emailage_Java carries model/OAuth2Token.java and utilities/OAuth2Wrapper.java.
  flows:
  - flow: clientCredentials
    note: The Go client exposes a configurable TokenEndpoint (opts.TokenEndpoint) used when AuthType is OAUTH2; the token URL itself is issued per customer under contract and is not published.
    tokenUrl: null
  name: EmailageOAuth2
  product: LexisNexis Emailage
  sources:
  - https://github.com/lexisnexis-risk-solutions/emailage-public-clients/tree/main/Emailage_Go
  - https://github.com/lexisnexis-risk-solutions/emailage-public-clients/tree/main/Emailage_Java
  type: oauth2
slug: lexisnexis-risk-solutions-authentication
source_filename: lexisnexis-risk-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  Emailage first-party SDK source (github.com/lexisnexis-risk-solutions/emailage-public-clients)\n  plus anonymous probes of developer.lexisnexisrisk.com\nnote: >-\n  There is no OpenAPI in this repo, so nothing here is derived from a spec. The insurance API\n  products have NO publicly documented authentication scheme; the only LexisNexis Risk Solutions\n  auth model readable on the open web is the one implemented in the company's own published\n  Emailage client libraries.\nsummary:\n  types:\n  - oauth1\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  gated: true\nschemes:\n- name: EmailageOAuth1\n  type: oauth1\n  product: LexisNexis Emailage\n  signature_methods:\n  - HMAC-SHA256\n  - HMAC-SHA384\n  - HMAC-SHA512\n  deprecated_signature_methods:\n  - HMAC-SHA1\n  credentials:\n  - Account SID (consumer key)\n  - Auth token (consumer secret)\n  hosts:\n    production: https://api.emailage.com\n\
  \    sandbox: https://sandbox.emailage.com\n  sources:\n  - https://github.com/lexisnexis-risk-solutions/emailage-public-clients/tree/main/Emailage_Python\n  - https://github.com/lexisnexis-risk-solutions/emailage-public-clients/tree/main/Emailage_Go\n  evidence: >-\n    Emailage_Python/emailage/client.py hard-codes ApiDomains.sandbox = https://sandbox.emailage.com\n    and ApiDomains.production = https://api.emailage.com; Emailage_Go/README.md states the package\n    no longer supports HMAC-SHA1 and recommends HMAC-SHA256/384/512.\n- name: EmailageOAuth2\n  type: oauth2\n  product: LexisNexis Emailage\n  flows:\n  - flow: clientCredentials\n    tokenUrl: null\n    note: >-\n      The Go client exposes a configurable TokenEndpoint (opts.TokenEndpoint) used when AuthType is\n      OAUTH2; the token URL itself is issued per customer under contract and is not published.\n  sources:\n  - https://github.com/lexisnexis-risk-solutions/emailage-public-clients/tree/main/Emailage_Go\n  - https://github.com/lexisnexis-risk-solutions/emailage-public-clients/tree/main/Emailage_Java\n\
  \  evidence: >-\n    Emailage_Go/emailage.go defines Endpoint + TokenEndpoint and an OAUTH2 AuthType;\n    Emailage_Java carries model/OAuth2Token.java and utilities/OAuth2Wrapper.java.\ninsurance_products:\n  documented: false\n  scheme: null\n  note: >-\n    The six insurance API products on developer.lexisnexisrisk.com (clue_auto, clue_auto_cc,\n    driver_discovery, insurview, mvr, vin_services) expose no anonymous authentication\n    documentation. Every product route answers 302 to /sp-portal/session-expired, and the\n    react-router data route (/mvr.data, /clue_auto.data) returns the same SingleFetchRedirect.\n    Credentials are issued under commercial contract.\nportal_login:\n  url: https://developer.lexisnexisrisk.com/services/api/login?external=true\n  status: 302\n  mechanism: SwaggerHub Portal external identity-provider login (SmartBear IdP federation)\n  note: Portal session login for humans, not an API authentication scheme.\ndiscovery_probes:\n- url: https://developer.lexisnexisrisk.com/.well-known/openid-configuration\n\
  \  status: 404\n- url: https://developer.lexisnexisrisk.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://risk.lexisnexis.com/.well-known/openid-configuration\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lexisnexis-risk-solutions/refs/heads/main/authentication/lexisnexis-risk-solutions-authentication.yml
summary_line: oauth1/oauth2 · 2 schemes
tags:
- Insurance
- United States
- Risk Data
- Property and Casualty
- Underwriting
- Claims
- Life Insurance
- Auto Insurance
- Data Analytics
- Partner Gated
---
