---
anonymous_access: false
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Advancednavigation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Advanced Navigation secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Advanced Navigation
provider_slug: advancednavigation
scheme_count: 2
schemes:
- description: '"All requests done through the API are connected to an account and must be authenticated. To authenticate any request while using the API the user''s API key just needs to be included in the request." The key is issued per Kinematica account and is displayed on the account page.'
  example_form: https://hq.advancednavigation.com.au/kinematica/api/alldatasets?v=1.2&apiKey=API_KEY
  in: query
  name: apiKey
  parameter_name: apiKey
  sources:
  - https://www.advancednavigation.com/downloads/versioned/kinematica/kinematica_api_reference_manual-1.6.pdf
  type: apiKey
- description: 'Not authentication, recorded here because it is mandatory alongside the key on every call: the API version number. A request whose version is incompatible with the server is rejected with {"success":"false","message":"Incompatible API Version"}.'
  in: query
  name: v
  parameter_name: v
  sources:
  - https://www.advancednavigation.com/downloads/versioned/kinematica/kinematica_api_reference_manual-1.6.pdf
  type: apiKey
slug: advancednavigation-authentication
source_filename: advancednavigation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: https://www.advancednavigation.com/downloads/versioned/kinematica/kinematica_api_reference_manual-1.6.pdf\ndocs: https://www.advancednavigation.com/accessories/gnss-ins-post-processing/kinematica/api-reference-manual/\nnote: >-\n  Derived from the published Kinematica API Reference Manual (document v1.6, API v1.2, dated\n  06/01/2026), section 4 \"Authentication\". Advanced Navigation publishes no OpenAPI, so there are no\n  securitySchemes to read mechanically; every field below is quoted from the provider's own PDF.\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter_name: apiKey\n  description: >-\n    \"All requests done through the API are connected to an account and must be authenticated. To\n    authenticate any request while using the API the user's API key just needs to be included in the\n    request.\" The key is issued per Kinematica\
  \ account and is displayed on the account page.\n  example_form: https://hq.advancednavigation.com.au/kinematica/api/alldatasets?v=1.2&apiKey=API_KEY\n  sources: ['https://www.advancednavigation.com/downloads/versioned/kinematica/kinematica_api_reference_manual-1.6.pdf']\n- name: v\n  type: apiKey\n  in: query\n  parameter_name: v\n  description: >-\n    Not authentication, recorded here because it is mandatory alongside the key on every call: the API\n    version number. A request whose version is incompatible with the server is rejected with\n    {\"success\":\"false\",\"message\":\"Incompatible API Version\"}.\n  sources: ['https://www.advancednavigation.com/downloads/versioned/kinematica/kinematica_api_reference_manual-1.6.pdf']\nobservations:\n- >-\n  The API key travels in the query string on GET calls (and as a form field on POST calls), so it is\n  written to server access logs, browser history and proxy logs by construction. There is no header\n  form, no bearer token, no OAuth,\
  \ and no documented key rotation or scoping mechanism.\n- >-\n  Probed live 2026-09-09: GET https://hq.advancednavigation.com.au/kinematica/api/alldatasets?v=1.2\n  returns HTTP 200 with body {\"success\":\"false\",\"message\":\"Invalid API key\"} — the API answers\n  anonymously with a 200 and signals failure in the JSON body rather than with 401/403.\ngaps:\n- No OAuth 2.0 / OpenID Connect surface; no scopes; no mTLS.\n- No account-level permission or scope reference published.\n- Failed authentication is reported as HTTP 200 with success:\"false\", not an HTTP 401.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advancednavigation/refs/heads/main/authentication/advancednavigation-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Navigation
- Inertial Navigation
- GNSS
- Positioning
- Robotics
- Defense
- Subsea
- Geospatial
- Post Processing
- Hardware
---
