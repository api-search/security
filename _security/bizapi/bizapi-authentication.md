---
api_key_in: []
api_specs:
- filename: bizapi-company-search-api-openapi.yml
  format: yaml
  label: BizAPI Company Search API
  slug: bizapi-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bizapi/refs/heads/main/openapi/bizapi-company-search-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Bizapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: BizAPI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BizAPI
provider_slug: bizapi
scheme_count: 1
schemes:
- applies_to:
  - https://www.naics.com/wp-json/naicsapi/v1/cosearch
  - https://www.naics.com/wp-json/naicsapi/v1/cosearchtest
  - https://www.naics.com/wp-json/naicsapi/v2/cosearch
  - https://www.naics.com/wp-json/naicsapi/v2/cosearchtest
  description: HTTP Basic Authentication. "The BizAPI Utilizes Basic Authentication. Credentials are given to you during your Account Activation." The username is an account identifier (the manual's worked example is JohnDoeInc) and the password is a provider-issued secret.
  format: Basic base64(username:password)
  gotcha: '"Spaces in Password MUST be kept." The issued password contains significant whitespace, published in the manual as six space-separated groups. Trimming or collapsing it — which many config loaders and secret managers do by default — produces a 401.'
  header: Authorization
  name: basicAuth
  scheme: basic
  sources:
  - openapi/bizapi-company-search-api-openapi.yml
  - https://www.naics.com/wp-content/uploads/2021/09/BizAPI-V2-Documentation.pdf
  type: http
slug: bizapi-authentication
source_filename: bizapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://www.naics.com/wp-content/uploads/2021/09/BizAPI-V2-Documentation.pdf\ndocs: https://www.naics.com/business-intelligence-api/bizapi-documents/\nderived_from: openapi/bizapi-company-search-api-openapi.yml\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  api_key_in: []\n  oauth2_flows: []\n  scopes: false\n  mtls: false\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  header: Authorization\n  format: 'Basic base64(username:password)'\n  description: >-\n    HTTP Basic Authentication. \"The BizAPI Utilizes Basic Authentication. Credentials are given\n    to you during your Account Activation.\" The username is an account identifier (the manual's\n    worked example is JohnDoeInc) and the password is a provider-issued secret.\n  sources:\n  - openapi/bizapi-company-search-api-openapi.yml\n  - https://www.naics.com/wp-content/uploads/2021/09/BizAPI-V2-Documentation.pdf\n  applies_to:\n  - https://www.naics.com/wp-json/naicsapi/v1/cosearch\n\
  \  - https://www.naics.com/wp-json/naicsapi/v1/cosearchtest\n  - https://www.naics.com/wp-json/naicsapi/v2/cosearch\n  - https://www.naics.com/wp-json/naicsapi/v2/cosearchtest\n  gotcha: >-\n    \"Spaces in Password MUST be kept.\" The issued password contains significant whitespace,\n    published in the manual as six space-separated groups. Trimming or collapsing it — which\n    many config loaders and secret managers do by default — produces a 401.\nissuance:\n  self_serve: false\n  process: >-\n    Credentials are issued by NAICS Association at account activation, after a trial request is\n    submitted through the form at https://www.naics.com/bizapi-details/. There is no developer\n    console that mints keys.\n  request_url: https://www.naics.com/bizapi-details/\n  account_url: https://www.naics.com/my-account/\n  contact: APICloudSolutions@NAICS.com\n  bound_to_layout: >-\n    The Record Layout that shapes every response is fixed to the credential at activation, not\n    chosen\
  \ per request. Changing layout means changing account configuration.\nsandbox:\n  separate_credentials: false\n  note: >-\n    \"The Sandbox requires basic authentication just like the live endpoint.\" The same secret\n    authenticates /cosearch and /cosearchtest — the path selects test mode, not the credential.\n    There is no test-mode key prefix, so a leaked credential is a production credential and\n    static analysis cannot distinguish a test key from a live one.\n  artifact: sandbox/bizapi-sandbox.yml\nfailure_modes:\n  - status: 401\n    message: Credentials are Missing or Invalid.\n  - status: 403\n    message: >-\n      Request not submitted due to lack of searches. Contact apicloudsolutions@naics.com or\n      call 973-625-5626 to purchase more searches.\n    note: >-\n      Authentication succeeded; authorization failed on the prepaid credit balance rather than\n      on scope or role.\ntransport:\n  tls_required: true\n  quote: All requests should be made over SSL.\n  observed:\
  \ TLSv1.3, HSTS max-age 31536000 (security/bizapi-domain-security.yml)\n  warning: >-\n    HTTP Basic sends a reusable long-lived secret on every request. There is no token exchange,\n    no expiry, no rotation endpoint and no revocation API documented.\ngaps:\n  - No OAuth 2.0, no OpenID Connect, no scopes — authorization is all-or-nothing per credential.\n  - No API key rotation, expiry or revocation mechanism documented.\n  - No least-privilege model; one credential grants the account's full layout and full credit balance.\n  - No separate sandbox credential.\n  - No MFA or IP allowlisting documented for API credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bizapi/refs/heads/main/authentication/bizapi-authentication.yml
summary_line: http · 1 scheme
tags:
- Business Intelligence
- Company Data
- CRM
- Firmographic Data
- NAICS
- SIC
---
