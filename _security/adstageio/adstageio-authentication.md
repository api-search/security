---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Adstageio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AdStage.io secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AdStage.io
provider_slug: adstageio
scheme_count: 2
schemes:
- description: HTTP header bearer token for API authentication. Tokens are provisioned by the AdStage Customer Success team (support@adstage.io) or an organization account manager; there is no self-service token issuance.
  in: header
  name: bearerToken
  scheme: bearer
  sources:
  - https://github.com/adstage/api-documentation/blob/master/src/adstage_api_concepts/authentication.apib
  type: http
- description: For applications serving multiple AdStage users, the AdStage API acts as an OAuth 2 provider. client_id / client_secret pairs are provisioned manually by the Customer Success team (support@adstage.io); there is no self-service OAuth application registration.
  flows:
  - flow: authorizationCode
  name: oauth2
  sources:
  - https://github.com/adstage/api-documentation/blob/master/src/adstage_api_concepts/authentication.apib
  type: oauth2
slug: adstageio-authentication
source_filename: adstageio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://github.com/adstage/api-documentation/blob/master/src/adstage_api_concepts/authentication.apib\ndocs: https://github.com/adstage/api-documentation\nnote: >-\n  AdStage (acquired by TapClicks, April 2020) documented the AdStage Data API in\n  API Blueprint. The standalone API host (platform.adstage.io) no longer\n  resolves; this profile captures the published authentication model verbatim\n  from the surviving public documentation.\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  http_location: header\n  oauth2_flows: [authorizationCode]\n  self_service_registration: false\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    in: header\n    description: >-\n      HTTP header bearer token for API authentication. Tokens are provisioned by\n      the AdStage Customer Success team (support@adstage.io) or an organization\n      account manager; there is no self-service token issuance.\n  \
  \  sources:\n      - https://github.com/adstage/api-documentation/blob/master/src/adstage_api_concepts/authentication.apib\n  - name: oauth2\n    type: oauth2\n    description: >-\n      For applications serving multiple AdStage users, the AdStage API acts as an\n      OAuth 2 provider. client_id / client_secret pairs are provisioned manually\n      by the Customer Success team (support@adstage.io); there is no self-service\n      OAuth application registration.\n    flows:\n      - flow: authorizationCode\n    sources:\n      - https://github.com/adstage/api-documentation/blob/master/src/adstage_api_concepts/authentication.apib\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adstageio/refs/heads/main/authentication/adstageio-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Advertising
- AdTech
- Marketing
- Analytics
- Reporting
- Advertising Data
- Cross-Network Advertising
- Acquired
---
