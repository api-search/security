---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Numverify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Numverify API declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Numverify API
provider_slug: numverify
scheme_count: 2
schemes:
- base: https://apilayer.net/api
  evidence: Probed 2026-09-16; missing key -> code 101 missing_access_key
  example: https://apilayer.net/api/validate?access_key=YOUR_KEY&number=14158586273
  id: access_key_query
  in: query
  name: access_key
  type: apiKey
- base: https://api.apilayer.com/number_verification
  evidence: Probed 2026-09-16; missing header -> HTTP 401 {"message":"No API key found in request"}
  example: 'curl ''https://api.apilayer.com/number_verification/validate?number=14158586273'' --header ''apikey: YOUR_KEY'''
  id: apikey_header
  in: header
  name: apikey
  type: apiKey
slug: numverify-authentication
source_filename: numverify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: searched\nsource: >-\n  numverify.com homepage example and the APILayer marketplace page for\n  number_verification. No OpenAPI is published (docs gated), so this profile is\n  hand-derived from the public request examples and confirmed against live\n  probes.\nsummary: >-\n  Single API-key credential, no OAuth. The key is obtained from a free APILayer\n  account. Two transports depending on base URL.\nschemes:\n- id: access_key_query\n  type: apiKey\n  in: query\n  name: access_key\n  base: https://apilayer.net/api\n  example: 'https://apilayer.net/api/validate?access_key=YOUR_KEY&number=14158586273'\n  evidence: 'Probed 2026-09-16; missing key -> code 101 missing_access_key'\n- id: apikey_header\n  type: apiKey\n  in: header\n  name: apikey\n  base: https://api.apilayer.com/number_verification\n  example: \"curl 'https://api.apilayer.com/number_verification/validate?number=14158586273' --header 'apikey: YOUR_KEY'\"\n  evidence: 'Probed 2026-09-16;\
  \ missing header -> HTTP 401 {\"message\":\"No API key found in request\"}'\noauth2: false\nmutual_tls: false\nnotes: >-\n  Key acquisition is self-serve at https://numverify.com/signup (free tier, 100\n  requests/month). The same APILayer account key works across the APILayer\n  marketplace suite on the api.apilayer.com host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numverify/refs/heads/main/authentication/numverify-authentication.yml
summary_line: 2 schemes
tags:
- Phone Validation
- Phone Numbers
- Telecommunications
- Data
- Validation
- Carrier Lookup
- Phone Number Lookup
---
