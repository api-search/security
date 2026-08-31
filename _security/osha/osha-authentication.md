---
api_key_in:
- header
- query
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Osha Authentication
name_suffix: Authentication
oauth_flows: []
overview: OSHA secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OSHA
provider_slug: osha
scheme_count: 3
schemes:
- api: OSHA Injury Tracking Application (ITA) API
  applies_to: every ITA API call (establishments, forms/form300A, forms/caseData, submissions)
  base_url: https://www.osha.gov/oshaApi/v1
  header: 'Authorization: Bearer [ITA API Token]'
  name: ITABearerToken
  observed:
    fetched: '2026-08-27'
    unauthenticated_status: 403
    url: https://www.osha.gov/oshaApi/v1/establishments
  rotation: OSHA reissued every token in July 2018; the pre-2018 token format was invalidated outright. No rotation cadence or expiry is documented for the current format.
  scheme: bearer
  source: https://www.osha.gov/sites/default/files/ita/documentation/osha_injury-tracking-application-api-documentation-v1.pdf
  token_issuance: 'Self-service, but account-gated: create an ITA account, log in at https://www.osha.gov/injuryreporting/ita and read the token from the API Token page. There is no public/anonymous read tier — the ITA API is a submission API for employers reporting their own 300A/300/301 injury and illness records.'
  type: http
- api: OSHA Enforcement Data API (DOL data.dol.gov RESTful interface)
  base_url: https://data.dol.gov/get/
  in: header
  name: DOLDataApiKeyHeader
  note: Key issuance is at https://devtools.dol.gov/developer, which the DOL developer portal itself flags as "New API Token Creation is Temporarily Disabled". A new integrator cannot obtain a credential for this surface today.
  parameter_name: X-API-KEY
  source: https://usdepartmentoflabor.github.io/Developer/experienced/
  type: apiKey
- api: DOL OData interface (api.dol.gov/V1)
  base_url: https://api.dol.gov/V1
  in: query
  name: DOLDataApiKeyQuery
  note: 'Credential in the query string, so it lands in logs, proxies and browser history. Probed 2026-08-27: https://api.dol.gov/V1/DOLAgency/Agencies?KEY=test returns HTTP 403 {"message":"Missing Authentication Token"} from AWS API Gateway.'
  parameter_name: KEY
  source: https://usdepartmentoflabor.github.io/Developer/experienced/
  type: apiKey
slug: osha-authentication
source_filename: osha-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://www.osha.gov/sites/default/files/ita/documentation/osha_injury-tracking-application-api-documentation-v1.pdf\ndocs:\n  - https://www.osha.gov/sites/default/files/ita/documentation/osha_injury-tracking-application-api-documentation-v1.pdf\n  - https://usdepartmentoflabor.github.io/Developer/beginner/\nnote: >-\n  Derived from the provider's own published API documentation, not from an OpenAPI —\n  neither OSHA nor DOL publishes a machine-readable contract for either surface.\n  Two different auth models are in play across the two APIs this repo catalogs.\nsummary:\n  types: [http, apiKey]\n  http_schemes: [bearer]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  oidc: false\n  mutual_tls: false\nschemes:\n  - name: ITABearerToken\n    type: http\n    scheme: bearer\n    api: OSHA Injury Tracking Application (ITA) API\n    base_url: https://www.osha.gov/oshaApi/v1\n    header: 'Authorization: Bearer [ITA API Token]'\n\
  \    applies_to: every ITA API call (establishments, forms/form300A, forms/caseData, submissions)\n    token_issuance: >-\n      Self-service, but account-gated: create an ITA account, log in at\n      https://www.osha.gov/injuryreporting/ita and read the token from the API Token page.\n      There is no public/anonymous read tier — the ITA API is a submission API for employers\n      reporting their own 300A/300/301 injury and illness records.\n    rotation: >-\n      OSHA reissued every token in July 2018; the pre-2018 token format was invalidated\n      outright. No rotation cadence or expiry is documented for the current format.\n    source: https://www.osha.gov/sites/default/files/ita/documentation/osha_injury-tracking-application-api-documentation-v1.pdf\n    observed:\n      url: https://www.osha.gov/oshaApi/v1/establishments\n      unauthenticated_status: 403\n      fetched: '2026-08-27'\n  - name: DOLDataApiKeyHeader\n    type: apiKey\n    in: header\n    parameter_name: X-API-KEY\n\
  \    api: OSHA Enforcement Data API (DOL data.dol.gov RESTful interface)\n    base_url: https://data.dol.gov/get/\n    source: https://usdepartmentoflabor.github.io/Developer/experienced/\n    note: >-\n      Key issuance is at https://devtools.dol.gov/developer, which the DOL developer portal\n      itself flags as \"New API Token Creation is Temporarily Disabled\". A new integrator\n      cannot obtain a credential for this surface today.\n  - name: DOLDataApiKeyQuery\n    type: apiKey\n    in: query\n    parameter_name: KEY\n    api: DOL OData interface (api.dol.gov/V1)\n    base_url: https://api.dol.gov/V1\n    source: https://usdepartmentoflabor.github.io/Developer/experienced/\n    note: >-\n      Credential in the query string, so it lands in logs, proxies and browser history.\n      Probed 2026-08-27: https://api.dol.gov/V1/DOLAgency/Agencies?KEY=test returns HTTP 403\n      {\"message\":\"Missing Authentication Token\"} from AWS API Gateway.\ngaps:\n  - No OAuth 2.0, OpenID Connect\
  \ or mTLS on any OSHA/DOL API surface.\n  - No documented token expiry, refresh, scope or least-privilege model on the ITA bearer token.\n  - No /.well-known/oauth-authorization-server or /.well-known/openid-configuration on any host (see well-known/osha-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osha/refs/heads/main/authentication/osha-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Compliance
- Government
- Health Standards
- Regulatory
- Workplace Safety
- Federal
- Open Data
- Enforcement
- Occupational Health
- Injury Reporting
---
