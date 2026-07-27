---
api_key_in: []
api_specs:
- filename: street-co-open-api-openapi.yml
  format: yaml
  label: Street Open API
  slug: street-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/street-co/refs/heads/main/openapi/street-co-open-api-openapi.yml
- filename: street-co-property-feed-api-openapi.yml
  format: yaml
  label: Street Property Feed API
  slug: street-property-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/street-co/refs/heads/main/openapi/street-co-property-feed-api-openapi.yml
- filename: street-co-spectre-api-openapi.yml
  format: yaml
  label: Spectre API
  slug: spectre-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/street-co/refs/heads/main/openapi/street-co-spectre-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Street Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Street.co.uk secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Street.co.uk
provider_slug: street-co
scheme_count: 2
schemes:
- format: 'Authorization: Bearer YOUR_API_TOKEN_HERE'
  header: Authorization
  name: your-api-token
  scheme: bearer
  sources:
  - openapi/street-co-open-api-openapi.yml
  - openapi/street-co-spectre-api-openapi.yml
  type: http
- header: Authorization
  name: your_api_token
  scheme: bearer
  sources:
  - openapi/street-co-property-feed-api-openapi.yml
  type: http
slug: street-co-authentication
source_filename: street-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\ndocs: https://developers.street.co.uk/docs/street-open-api\nsource: openapi/street-co-open-api-openapi.yml, openapi/street-co-property-feed-api-openapi.yml,\n  openapi/street-co-spectre-api-openapi.yml\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  api_key_in: []\n  scopes: false\nmodel: >-\n  A single HTTP bearer token per application, applied globally in all three OpenAPI documents\n  via a root-level security requirement. There is no OAuth 2.0 flow, no OIDC discovery, no\n  scope vocabulary and no refresh mechanism published — a token is a long-lived opaque bearer\n  credential carrying the permissions of the issuing Street account, which is why Street's own\n  help centre warns that handing a Public API token to a third party gives that supplier access\n  to client data in the account.\nschemes:\n- name: your-api-token\n  type: http\n  scheme: bearer\n\
  \  header: Authorization\n  format: 'Authorization: Bearer YOUR_API_TOKEN_HERE'\n  sources:\n  - openapi/street-co-open-api-openapi.yml\n  - openapi/street-co-spectre-api-openapi.yml\n- name: your_api_token\n  type: http\n  scheme: bearer\n  header: Authorization\n  sources:\n  - openapi/street-co-property-feed-api-openapi.yml\ntoken_issuance:\n- api: Street Open API\n  method: self-serve-in-product\n  path: Settings > Account Administration > Applications\n  requires: An active Street.co.uk subscription and a company-admin user in that account.\n  docs: https://intercom.help/streetcouk/en/articles/8474378-generating-an-api-token\n  note: >-\n    The help centre asks the admin to name the application and pick the relevant feed from an\n    \"API token scope\" drop-down — that selects between the Property Feed API and the Public\n    (Open) API. It is a feed selector, not an OAuth scope vocabulary; no scope strings are\n    published.\n- api: Street Open API (staging)\n  method: email-request\n\
  \  contact: apis@street.co.uk\n  quote: >-\n    \"if you would like a sandbox account on our staging environment, please email\n    apis@street.co.uk to request a token.\"\n- api: Street Property Feed API\n  method: self-serve-in-product\n  path: Settings > Applications\n- api: Spectre API\n  method: email-request\n  contact: apis@spectre.uk.com\n  quote: If you do not have an API token, please contact the Spectre team at apis@spectre.uk.com.\ntoken_handling:\n  rotation_policy: undocumented\n  expiry: undocumented\n  revocation: Delete the application in the Street CRM Applications screen.\n  transport: HTTPS only (HSTS enabled on street.co.uk, max-age 31536000)\nunverified_third_party_claim: >-\n  A third-party supplier directory describes Street's API as offering \"OAuth\". No OAuth flow,\n  authorization endpoint or scope list exists anywhere on developers.street.co.uk and all three\n  contracts declare HTTP bearer only. Recorded as an unverified external claim.\nrelated:\n  scopes:\
  \ null\n  conventions: conventions/street-co-conventions.yml\n  sandbox: sandbox/street-co-sandbox.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/street-co/refs/heads/main/authentication/street-co-authentication.yml
summary_line: http · 2 schemes
tags:
- Real Estate
- United Kingdom
- PropTech
- CRM
- Property Listings
- Property Management
- Rentals
- Lettings
- Estate Agency
- Valuation
- Conveyancing
---
