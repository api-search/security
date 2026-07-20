---
api_key_in:
- header
api_specs:
- filename: dnsfilter-openapi-original.json
  format: json
  label: DNSFilter API
  slug: dnsfilter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dnsfilter/refs/heads/main/openapi/dnsfilter-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dnsfilter Authentication
name_suffix: Authentication
oauth_flows: []
overview: DNSFilter secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DNSFilter
provider_slug: dnsfilter
scheme_count: 1
schemes:
- in: header
  name: header_authorization
  parameter: Authorization
  prefix: none
  sources:
  - openapi/dnsfilter-openapi-original.json
  type: apiKey
  value_format: raw-api-key
slug: dnsfilter-authentication
source_filename: dnsfilter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/dnsfilter-openapi-original.json\ndocs: https://help.dnsfilter.com/hc/en-us/articles/21169189058323-API-Tokens\nnotes: >-\n  Authentication is required for most, but not all, endpoints. It is done by\n  setting the `Authorization` request header to the API key value directly\n  (no `Bearer ` prefix), e.g. `Authorization: eyJ...`. API keys are created\n  and managed in the DNSFilter dashboard under Account Settings, and via the\n  Api Keys API (V1_Api_Keys-create / -index / -revoke). Keys carry a name,\n  expiry, last_four, and status. No OAuth2 or OpenID Connect is offered; there\n  is no scope surface.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: header_authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: raw-api-key\n  prefix: none\n  sources:\n  - openapi/dnsfilter-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dnsfilter/refs/heads/main/authentication/dnsfilter-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- DNS
- Security
- Content Filtering
- Threat Protection
- Cybersecurity
- Networking
- MSP
---
