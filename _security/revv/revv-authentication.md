---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Revv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revv secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Revv
provider_slug: revv
scheme_count: 2
schemes:
- authorization_url: null
  evidence: '"OAuth 2.0" listed among Revv API plan capabilities on https://www.revv.so/developers/api-pricing.html (HTTP 200, fetched 2026-08-14)'
  flows: []
  name: OAuth 2.0
  scopes: []
  token_url: null
  type: oauth2
- evidence: '"Single sign-on (SSO) — OAuth and SAML2.0 support" on https://www.revv.so/pricing.html (HTTP 200, fetched 2026-08-14)'
  name: SSO (SAML 2.0)
  scope: application sign-in, not API authorization
  type: saml2
slug: revv-authentication
source_filename: revv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://www.revv.so/developers/api-pricing.html\ndocs: https://www.revv.so/docs/authenticate-your-revv-api\ndocs_status: 502\nnote: >-\n  Revv has no published OpenAPI, so this profile is not derived from a spec — it is what\n  Revv itself still states in public about API authentication. The developer API-pricing\n  page (live, 200) lists \"OAuth 2.0\" as an API plan capability, and the product pricing\n  page lists \"Single sign-on (SSO) — OAuth and SAML2.0 support for one login access\n  between your business apps and Revv\". The dedicated auth article,\n  /docs/authenticate-your-revv-api, is still listed in Revv's sitemap.xml but the origin\n  now returns nginx 502 Bad Gateway, and the API reference host named in Revv's own API\n  pricing FAQ (https://build.revv.so) returns 404 from a Postman \"Not found\" page. No\n  scheme names, token endpoints, scopes, or header formats are reachable anywhere, so\n  none are recorded\
  \ here.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows: []\n  spec_backed: false\nschemes:\n- name: OAuth 2.0\n  type: oauth2\n  flows: []\n  authorization_url: null\n  token_url: null\n  scopes: []\n  evidence: >-\n    \"OAuth 2.0\" listed among Revv API plan capabilities on\n    https://www.revv.so/developers/api-pricing.html (HTTP 200, fetched 2026-08-14)\n- name: SSO (SAML 2.0)\n  type: saml2\n  scope: application sign-in, not API authorization\n  evidence: >-\n    \"Single sign-on (SSO) — OAuth and SAML2.0 support\" on\n    https://www.revv.so/pricing.html (HTTP 200, fetched 2026-08-14)\nunverified_claims:\n- claim: >-\n    Revv APIs follow the OAuth 2.0 authentication process and each API request carries an\n    access_token in the authentication header.\n  attributed_to: https://www.revv.so/docs/authenticate-your-revv-api\n  verified: false\n  reason: >-\n    Recovered from a search-engine index of that page; the live URL returns 502 so the\n    wording could\
  \ not be fetched and confirmed on 2026-08-14. Recorded as an unverified\n    claim, not as a captured contract.\nx-evidence:\n- url: https://www.revv.so/developers/api-pricing.html\n  status: 200\n  fetched: '2026-08-14'\n- url: https://www.revv.so/pricing.html\n  status: 200\n  fetched: '2026-08-14'\n- url: https://www.revv.so/docs/authenticate-your-revv-api\n  status: 502\n  fetched: '2026-08-14'\n- url: https://build.revv.so/\n  status: 404\n  fetched: '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revv/refs/heads/main/authentication/revv-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Document Automation
- Electronic Signature
- Contract Management
- Sales Enablement
- Workflow Automation
- SaaS
---
