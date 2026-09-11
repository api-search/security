---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Authentication profile for the one publicly callable API surface on this record, the College Scorecard API. It is fronted by api.data.gov, the shared federal API gateway, so the authentication model is the gateway''s: a single API key, no OAuth, no scopes, no user identity. Federal Student Aid''s own partner systems (FSA Partner Connect, COD, NSLDS, SAIG) authenticate through enrolled-organization credentials that are not documented publicly and are out of scope here.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Federal Student Aid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Federal Student Aid declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Federal Student Aid
provider_slug: federal-student-aid
scheme_count: 3
schemes:
- applies_to: College Scorecard API
  description: '"To use the College Scorecard API you must have an API key... it is required for all API requests." Appended as ?api_key=YOUR_API_KEY.'
  evidence: https://collegescorecard.ed.gov/data/api-documentation/
  id: api_key_query
  in: query
  name: api_key
  required: true
  type: apiKey
- applies_to: College Scorecard API
  description: api.data.gov accepts the same key in an HTTP header instead of the query string. Preferred over the query parameter because the key does not then appear in access logs, referrers or browser history.
  evidence: https://api.data.gov/docs/developer-manual/
  id: api_key_header
  in: header
  name: X-Api-Key
  required: false
  type: apiKey
- applies_to: College Scorecard API
  description: api.data.gov also accepts the API key as the HTTP Basic Auth username with an empty password.
  evidence: https://api.data.gov/docs/developer-manual/
  id: api_key_basic
  required: false
  scheme: basic
  type: http
slug: federal-student-aid-authentication
source_filename: federal-student-aid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Federal Student Aid\nproviderId: federal-student-aid\ngenerated: '2026-09-09'\nmethod: searched\nsource: https://api.data.gov/docs/developer-manual/\ndocs: https://collegescorecard.ed.gov/data/api-documentation/\nmodified: '2026-09-09'\ndescription: >-\n  Authentication profile for the one publicly callable API surface on this record,\n  the College Scorecard API. It is fronted by api.data.gov, the shared federal API\n  gateway, so the authentication model is the gateway's: a single API key, no OAuth,\n  no scopes, no user identity. Federal Student Aid's own partner systems\n  (FSA Partner Connect, COD, NSLDS, SAIG) authenticate through enrolled-organization\n  credentials that are not documented publicly and are out of scope here.\nschemes:\n  - id: api_key_query\n    type: apiKey\n    in: query\n    name: api_key\n    applies_to: College Scorecard API\n    required: true\n    description: >-\n\
  \      \"To use the College Scorecard API you must have an API key... it is required\n      for all API requests.\" Appended as ?api_key=YOUR_API_KEY.\n    evidence: https://collegescorecard.ed.gov/data/api-documentation/\n  - id: api_key_header\n    type: apiKey\n    in: header\n    name: X-Api-Key\n    applies_to: College Scorecard API\n    required: false\n    description: >-\n      api.data.gov accepts the same key in an HTTP header instead of the query\n      string. Preferred over the query parameter because the key does not then\n      appear in access logs, referrers or browser history.\n    evidence: https://api.data.gov/docs/developer-manual/\n  - id: api_key_basic\n    type: http\n    scheme: basic\n    applies_to: College Scorecard API\n    required: false\n    description: >-\n      api.data.gov also accepts the API key as the HTTP Basic Auth username with an\n      empty password.\n    evidence: https://api.data.gov/docs/developer-manual/\noauth2: false\nopenid_connect: false\n\
  mutual_tls: false\nscopes: none\nscopes_note: >-\n  No OAuth surface exists, so there is no scope model and no scopes/ artifact.\n  A key is either valid or it is not; there is no per-resource authorization.\nkey_issuance:\n  self_service: true\n  signup_url: https://api.data.gov/signup/\n  delivery: emailed\n  approval: automatic\n  cost: free\n  note: >-\n    Registration is a form plus a security challenge; the key is emailed. No\n    contract, no billing relationship, no sales gate.\ntest_credentials:\n  demo_key: DEMO_KEY\n  demo_key_note: >-\n    api.data.gov publishes a shared DEMO_KEY for exploration, rate limited to\n    30 requests per IP per hour and 50 per IP per day. Verified live 2026-09-09\n    against /ed/collegescorecard/v1/schools (HTTP 200).\n  evidence: https://api.data.gov/docs/developer-manual/\ntransport:\n  https_required: true\n  https_error: HTTPS_REQUIRED (HTTP 400)\n  evidence: https://api.data.gov/docs/developer-manual/\nfailure_modes:\n  - code: API_KEY_MISSING\n\
  \    http_status: 403\n    observed: true\n    observed_note: >-\n      Probed 2026-09-09 — GET https://api.data.gov/ed/collegescorecard/v1/schools\n      with no key returned 403 with body {\"error\":{\"code\":\"API_KEY_MISSING\", ...}}.\n  - code: API_KEY_INVALID\n    http_status: 403\n    observed: false\n  - code: API_KEY_DISABLED\n    http_status: 403\n    observed: false\n  - code: API_KEY_UNAUTHORIZED\n    http_status: 403\n    observed: false\n  - code: API_KEY_UNVERIFIED\n    http_status: 403\n    observed: false\ngated_surfaces:\n  - name: FSA Partner Connect / SAIG\n    url: https://fsapartners.ed.gov/help-center/access-to-fsa-systems\n    model: enrolled-organization credentials\n    public_contract: false\n    note: >-\n      Schools, servicers and vendors exchange data with FSA through the Student Aid\n      Internet Gateway using enrollment-issued credentials and batch software\n      (EDconnect / TDClient). No public authentication documentation, no public\n      contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-student-aid/refs/heads/main/authentication/federal-student-aid-authentication.yml
summary_line: 3 schemes
tags:
- Education
- Federal-Government
- Financial Aid
- Grants
- Loans
- Student Aid
---
