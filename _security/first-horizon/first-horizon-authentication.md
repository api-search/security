---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: First Horizon Authentication
name_suffix: Authentication
oauth_flows: []
overview: First Horizon secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: First Horizon
provider_slug: first-horizon
scheme_count: 1
schemes:
- applies_to:
  - Move Money Transfer v1
  - ACH Origination
  - Account Information
  - ABA Lookup v1
  - BIC Lookup v1
  authorization_url: null
  documented: true
  flows: []
  name: OAuth2
  scopes: []
  sources:
  - https://developers-test.firsthorizon.com/apis/v0/oauth
  token_url: null
  type: oauth2
slug: first-horizon-authentication
source_filename: first-horizon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developers-test.firsthorizon.com/apis/v0/oauth\ndocs: https://developers-test.firsthorizon.com/apis/v0/oauth\nnote: >-\n  No public OpenAPI is downloadable, so the securityScheme could not be derived\n  mechanically. First Horizon's API Banking developer portal documents that all\n  API Banking endpoints are authorized with OAuth 2.0 access tokens. The specific\n  grant/flow, authorization and token URLs, and scope names are behind\n  partner/relationship-gated onboarding and are not published anonymously; they\n  are recorded here as unspecified rather than fabricated.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: OAuth2\n  type: oauth2\n  documented: true\n  flows: []\n  authorization_url: null\n  token_url: null\n  scopes: []\n  applies_to:\n  - Move Money Transfer v1\n  - ACH Origination\n  - Account Information\n  - ABA Lookup v1\n  - BIC Lookup v1\n  sources:\n  - https://developers-test.firsthorizon.com/apis/v0/oauth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-horizon/refs/heads/main/authentication/first-horizon-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- United States
- Banking
- Financial Services
- Treasury Management
- API Banking
- ACH
- Payments
- Open Banking
- Super-Regional Bank
- Fortune 500
- Wealth Management
- Capital Markets
---
