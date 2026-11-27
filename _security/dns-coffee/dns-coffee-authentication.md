---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dns-coffee-auth-api-openapi.yml
  format: yaml
  label: DNS Coffee Auth API
  slug: dns-coffee-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-auth-api-openapi.yml
- filename: dns-coffee-dnssec-api-openapi.yml
  format: yaml
  label: DNS Coffee Dnssec API
  slug: dns-coffee-dnssec-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-dnssec-api-openapi.yml
- filename: dns-coffee-domains-api-openapi.yml
  format: yaml
  label: DNS Coffee Domains API
  slug: dns-coffee-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-domains-api-openapi.yml
- filename: dns-coffee-feeds-api-openapi.yml
  format: yaml
  label: DNS Coffee Feeds API
  slug: dns-coffee-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-feeds-api-openapi.yml
- filename: dns-coffee-ips-api-openapi.yml
  format: yaml
  label: DNS Coffee Ips API
  slug: dns-coffee-ips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-ips-api-openapi.yml
- filename: dns-coffee-nameservers-api-openapi.yml
  format: yaml
  label: DNS Coffee Nameservers API
  slug: dns-coffee-nameservers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-nameservers-api-openapi.yml
- filename: dns-coffee-records-api-openapi.yml
  format: yaml
  label: DNS Coffee Records API
  slug: dns-coffee-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-records-api-openapi.yml
- filename: dns-coffee-search-api-openapi.yml
  format: yaml
  label: DNS Coffee Search API
  slug: dns-coffee-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-search-api-openapi.yml
- filename: dns-coffee-stats-api-openapi.yml
  format: yaml
  label: DNS Coffee Stats API
  slug: dns-coffee-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-stats-api-openapi.yml
- filename: dns-coffee-trends-api-openapi.yml
  format: yaml
  label: DNS Coffee Trends API
  slug: dns-coffee-trends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-trends-api-openapi.yml
- filename: dns-coffee-zones-api-openapi.yml
  format: yaml
  label: DNS Coffee Zones API
  slug: dns-coffee-zones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dns-coffee/openapi/dns-coffee-zones-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: DNS Coffee Authentication
name_suffix: Authentication
oauth_flows: []
overview: DNS Coffee secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DNS Coffee
provider_slug: dns-coffee
scheme_count: 1
schemes:
- description: API key issued by DNS Coffee.
  in: header
  name: api_key
  parameter: X-API-Key
  sources:
  - openapi/dns-coffee-openapi.yml
  type: apiKey
slug: dns-coffee-authentication
source_filename: dns-coffee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/dns-coffee-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key issued by DNS Coffee.\n  sources:\n  - openapi/dns-coffee-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/dns-coffee/authentication/dns-coffee-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DNS
- Domain Names
- Domains
- Zone Files
- Nameservers
- Research
---
