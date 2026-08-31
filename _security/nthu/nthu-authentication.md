---
api_key_in: []
api_specs:
- filename: nthu-oauth-api-openapi.yml
  format: yaml
  label: NTHU Academic Information System OAuth 2.0 Service
  slug: nthu-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/nthu-oauth-api-openapi.yml
- filename: nthu-data-api.yaml
  format: yaml
  label: NTHU Data API
  slug: nthu-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/_original/nthu-data-api.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Nthu Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Tsing Hua University secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: National Tsing Hua University
provider_slug: nthu
scheme_count: 2
schemes:
- credential_lifetime: Secret keys are valid for one year and must be re-applied for on expiry (policy article 5).
  flows:
  - authorizationUrl: https://oauth.ccxp.nthu.edu.tw/v1.1/authorize.php
    flow: authorizationCode
    pkce: not_documented
    refreshUrl: https://oauth.ccxp.nthu.edu.tw/v1.1/token.php
    refresh_tokens: true
    tokenUrl: https://oauth.ccxp.nthu.edu.tw/v1.1/token.php
    token_type: Bearer
  name: nthuOAuth
  onboarding: gated
  onboarding_detail: Not self-service. Applicants must be current NTHU faculty, staff or enrolled students, must have the request signed off by their unit head, and must pass review by the Computer and Communication Center plus every unit that owns a requested data field. Application form published as https://oauth.ccxp.nthu.edu.tw/v1.1/doc/OAuth-Apply.docx.
  operator_detail: Run by NTHU's Computer and Communication Center against the Academic Information System (CCXP). Host oauth.ccxp.nthu.edu.tw resolves to 140.114.68.19, inside NTHU's own TANet allocation.
  prohibited: Proxying or harvesting a user's account and password on the client's own login form is prohibited; violation suspends the account and bars the unit from the service for one year (policy article 6).
  sources:
  - https://oauth.ccxp.nthu.edu.tw/v1.1/doc/
  - https://law.site.nthu.edu.tw/p/406-1326-197509,r6923.php
  - openapi/nthu-oauth-api-openapi.yml
  transport_requirement: Callback URLs must use an encrypted connection (policy article 3).
  type: oauth2
  x-operator: institution
- description: The NTHU Data API at api.nthusa.tw requires no authentication. All 22 documented paths were probed keyless on 2026-08-30 and returned 200 with live campus data.
  name: none
  sources:
  - openapi/_original/nthu-data-api.yaml
  type: none
  x-operator: tenant
slug: nthu-authentication
source_filename: nthu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: derived\nsource: https://oauth.ccxp.nthu.edu.tw/v1.1/doc/\nnote: >-\n  Derived from National Tsing Hua University's own published OAuth interface manual and confirmed by\n  live probes of the three endpoints on 2026-08-30. NTHU publishes no OpenAPI or OIDC discovery\n  document; there is no .well-known/openid-configuration on the host (403).\nsummary:\n  types:\n  - oauth2\nschemes:\n- name: nthuOAuth\n  type: oauth2\n  x-operator: institution\n  operator_detail: >-\n    Run by NTHU's Computer and Communication Center against the Academic Information System (CCXP).\n    Host oauth.ccxp.nthu.edu.tw resolves to 140.114.68.19, inside NTHU's own TANet allocation.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.ccxp.nthu.edu.tw/v1.1/authorize.php\n    tokenUrl: https://oauth.ccxp.nthu.edu.tw/v1.1/token.php\n    refreshUrl: https://oauth.ccxp.nthu.edu.tw/v1.1/token.php\n    refresh_tokens: true\n    token_type: Bearer\n\
  \    pkce: not_documented\n  onboarding: gated\n  onboarding_detail: >-\n    Not self-service. Applicants must be current NTHU faculty, staff or enrolled students, must have\n    the request signed off by their unit head, and must pass review by the Computer and Communication\n    Center plus every unit that owns a requested data field. Application form published as\n    https://oauth.ccxp.nthu.edu.tw/v1.1/doc/OAuth-Apply.docx.\n  credential_lifetime: >-\n    Secret keys are valid for one year and must be re-applied for on expiry (policy article 5).\n  transport_requirement: >-\n    Callback URLs must use an encrypted connection (policy article 3).\n  prohibited: >-\n    Proxying or harvesting a user's account and password on the client's own login form is\n    prohibited; violation suspends the account and bars the unit from the service for one year\n    (policy article 6).\n  sources:\n  - https://oauth.ccxp.nthu.edu.tw/v1.1/doc/\n  - https://law.site.nthu.edu.tw/p/406-1326-197509,r6923.php\n\
  \  - openapi/nthu-oauth-api-openapi.yml\n- name: none\n  type: none\n  x-operator: tenant\n  description: >-\n    The NTHU Data API at api.nthusa.tw requires no authentication. All 22 documented paths were\n    probed keyless on 2026-08-30 and returned 200 with live campus data.\n  sources:\n  - openapi/_original/nthu-data-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/authentication/nthu-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Education
- Higher Education
- University
- Taiwan
- Public Research University
- Identity
- OAuth
- Open Data
- Campus
- Course Catalog
- Research Repository
- Library
---
