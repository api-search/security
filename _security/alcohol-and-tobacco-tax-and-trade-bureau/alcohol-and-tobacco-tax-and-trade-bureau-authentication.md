---
api_key_in: []
auth_types:
- none
- session-login
description: ''
kind: authentication
layout: security
method: searched
name: Alcohol And Tobacco Tax And Trade Bureau Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alcohol and Tobacco Tax and Trade Bureau secures its APIs with none and session-login across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Alcohol and Tobacco Tax and Trade Bureau
provider_slug: alcohol-and-tobacco-tax-and-trade-bureau
scheme_count: 2
schemes:
- applies_to:
  - TTB Open Data files (XML / CSV / JSON)
  - TTB Public COLA Registry read access
  evidence: https://www.ttb.gov/images/foia/cola_stats.xml and https://www.ttb.gov/images/foia/form_stats.csv both return HTTP 200 with no Authorization header, no cookie and no API key (probed 2026-09-01). The COLA Public Registry page states no registration or password is required to use it.
  name: anonymous-public-data
  sources:
  - https://www.ttb.gov/regulated-commodities/labeling/cola-public-registry
  type: none
- applies_to:
  - Permits Online (PONL)
  - COLAs Online (filing)
  - Formulas Online (FONL)
  evidence: TTB Online applications require a registered TTB.gov user account and are entered through a form login at https://www.ttbonline.gov/permitsonline/. No token, key or OAuth endpoint is documented; /.well-known/oauth-authorization-server and /.well-known/openid-configuration are not served on www.ttb.gov (404 each).
  login_url: https://www.ttbonline.gov/permitsonline/
  name: ttb-online-session-login
  programmatic_access: false
  scheme: form-login
  sources:
  - https://www.ttb.gov/online-services/ponl/permits-online-help
  type: session
slug: alcohol-and-tobacco-tax-and-trade-bureau-authentication
source_filename: alcohol-and-tobacco-tax-and-trade-bureau-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: https://www.ttb.gov/data\ndocs: https://www.ttb.gov/regulated-commodities/labeling/cola-public-registry\nnote: >-\n  Derived by search, not from a spec — TTB publishes no OpenAPI, so there are no\n  securitySchemes to aggregate. The auth model is nonetheless well-defined and worth recording:\n  TTB's machine-readable open data is entirely anonymous and issues no credentials of any kind,\n  while its two transactional web applications are session-login only with no programmatic\n  access path.\nsummary:\n  types: [none, session-login]\n  api_key_in: []\n  oauth2_flows: []\n  api_keys_issued: false\n  registration_required_for_data: false\nschemes:\n  - name: anonymous-public-data\n    type: none\n    applies_to:\n      - TTB Open Data files (XML / CSV / JSON)\n      - TTB Public COLA Registry read access\n    evidence: >-\n      https://www.ttb.gov/images/foia/cola_stats.xml and\n      https://www.ttb.gov/images/foia/form_stats.csv\
  \ both return HTTP 200 with no\n      Authorization header, no cookie and no API key (probed 2026-09-01). The COLA Public\n      Registry page states no registration or password is required to use it.\n    sources: [https://www.ttb.gov/regulated-commodities/labeling/cola-public-registry]\n  - name: ttb-online-session-login\n    type: session\n    scheme: form-login\n    applies_to:\n      - Permits Online (PONL)\n      - COLAs Online (filing)\n      - Formulas Online (FONL)\n    login_url: https://www.ttbonline.gov/permitsonline/\n    evidence: >-\n      TTB Online applications require a registered TTB.gov user account and are entered through\n      a form login at https://www.ttbonline.gov/permitsonline/. No token, key or OAuth endpoint\n      is documented; /.well-known/oauth-authorization-server and\n      /.well-known/openid-configuration are not served on www.ttb.gov (404 each).\n    programmatic_access: false\n    sources: [https://www.ttb.gov/online-services/ponl/permits-online-help]\n\
  absent:\n  - api_key\n  - bearer_token\n  - oauth2\n  - openid_connect\n  - mutual_tls\n  - hmac_signing\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alcohol-and-tobacco-tax-and-trade-bureau/refs/heads/main/authentication/alcohol-and-tobacco-tax-and-trade-bureau-authentication.yml
summary_line: none/session-login · 2 schemes
tags:
- Alcohol
- Tobacco
- Federal-Government
- Excise Tax
- Regulations
- Treasury
---
