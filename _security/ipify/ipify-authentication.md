---
api_key_in:
- query
api_specs:
- filename: ipify-ip-api.yml
  format: yaml
  label: ipify Public IP Address API
  slug: ipify-public-ip-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipify/refs/heads/main/openapi/ipify-ip-api.yml
- filename: ipify-geolocation-api.yml
  format: yaml
  label: ipify IP Geolocation API
  slug: ipify-ip-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipify/refs/heads/main/openapi/ipify-geolocation-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ipify Authentication
name_suffix: Authentication
oauth_flows: []
overview: ipify secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ipify
provider_slug: ipify
scheme_count: 1
schemes:
- description: Personal API key issued by WhoisXML API for the ipify Geolocation product. Passed as the `apiKey` query parameter on every request.
  in: query
  name: ApiKeyQuery
  parameter: apiKey
  sources:
  - openapi/ipify-geolocation-api.yml
  type: apiKey
slug: ipify-authentication
source_filename: ipify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ipify-geolocation-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: Personal API key issued by WhoisXML API for the ipify Geolocation product. Passed\n    as the `apiKey` query parameter on every request.\n  sources:\n  - openapi/ipify-geolocation-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipify/refs/heads/main/authentication/ipify-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Development
- IP Address
- Geolocation
- IP Intelligence
- Public APIs
---
