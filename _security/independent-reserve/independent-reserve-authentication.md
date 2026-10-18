---
anonymous_access: true
api_key_in: []
api_specs:
- filename: independent-reserve-private-api-openapi.yml
  format: yaml
  label: Independent Reserve Private API
  slug: independent-reserve-private-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independent-reserve/refs/heads/main/openapi/independent-reserve-private-api-openapi.yml
- filename: independent-reserve-public-api-openapi.yml
  format: yaml
  label: Independent Reserve Public API
  slug: independent-reserve-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independent-reserve/refs/heads/main/openapi/independent-reserve-public-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Independent Reserve Authentication
name_suffix: Authentication
oauth_flows: []
overview: Independent Reserve declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Independent Reserve
provider_slug: independent-reserve
scheme_count: 2
schemes:
- applies_to: /Private/* and /rfq/*
  in: body
  key_management:
  - Keys are generated under Settings > API Keys with a selectable access level
  - IP whitelisting strongly recommended; non-whitelisted IPs are rejected
  - Keys created without IP whitelisting are disabled after 6 months unused
  name: IR API key + HMAC-SHA256 signature
  parameters:
  - apiKey
  - nonce
  - expiry
  - signature
  signature:
    algorithm: HMAC-SHA256
    encoding: hex
    message: method URL, then parameterName=parameterValue pairs, comma-separated, in documented order
  type: apiKey
- applies_to: /Public/*
  name: none
  type: none
slug: independent-reserve-authentication
source_filename: independent-reserve-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: searched\nsource: https://www.independentreserve.com/features/api#authentication-api-key\ndocs: https://www.independentreserve.com/features/api#authentication-api-key\nsummary: 'Public methods need no authentication. Private methods are POSTs carrying apiKey, a nonce OR an expiry (one, not both), and a signature: a hex HMAC-SHA256 over a comma-separated string of the method URL and every parameter as parameterName=parameterValue, keyed with the API secret.'\nschemes:\n- name: IR API key + HMAC-SHA256 signature\n  type: apiKey\n  in: body\n  parameters:\n  - apiKey\n  - nonce\n  - expiry\n  - signature\n  signature:\n    algorithm: HMAC-SHA256\n    encoding: hex\n    message: method URL, then parameterName=parameterValue pairs, comma-separated, in documented order\n  key_management:\n  - Keys are generated under Settings > API Keys with a selectable access level\n  - IP whitelisting strongly recommended; non-whitelisted IPs are rejected\n  -\
  \ Keys created without IP whitelisting are disabled after 6 months unused\n  applies_to: /Private/* and /rfq/*\n- name: none\n  type: none\n  applies_to: /Public/*\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/independent-reserve/refs/heads/main/authentication/independent-reserve-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Bitcoin
- Financial Services
---
