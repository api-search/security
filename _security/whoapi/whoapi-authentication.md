---
api_key_in:
- query
api_specs:
- filename: whoapi-openapi.yml
  format: yaml
  label: WhoAPI Domain Intelligence API
  slug: whoapi-domain-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whoapi/refs/heads/main/openapi/whoapi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Whoapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: WhoAPI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WhoAPI
provider_slug: whoapi
scheme_count: 1
schemes:
- description: Every request must carry the account's private API key as the `apikey` query parameter, e.g. https://api.whoapi.com/?domain=whoapi.com&r=whois&apikey=YOUR_API_KEY
  in: query
  name: apiKey
  parameter: apikey
  sources:
  - openapi/whoapi-openapi.yml
  type: apiKey
slug: whoapi-authentication
source_filename: whoapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://whoapi.com/api-documentation/\ndocs: https://whoapi.com/api-documentation/\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: >-\n    Every request must carry the account's private API key as the `apikey`\n    query parameter, e.g. https://api.whoapi.com/?domain=whoapi.com&r=whois&apikey=YOUR_API_KEY\n  sources: [openapi/whoapi-openapi.yml]\nnotes:\n- IP whitelisting is available in account settings (status code 15 = \"IP not whitelisted\").\n- No OAuth2/OIDC surface; the API is single-key.\n- Both HTTP and HTTPS are accepted; HTTPS recommended.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whoapi/refs/heads/main/authentication/whoapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Domains
- WHOIS
- Domain Availability
- SSL
- Email Verification
- Blacklist
- Cybersecurity
- Domain Intelligence
- Screenshots
- Reputation
---
