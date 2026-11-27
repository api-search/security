---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nibiashara-biz-africa-fx-data-api-openapi.yml
  format: yaml
  label: Ni Biashara Africa FX data API
  slug: nibiashara-biz-africa-fx-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibiashara-biz/openapi/nibiashara-biz-africa-fx-data-api-openapi.yml
- filename: nibiashara-biz-agent-identity-api-openapi.yml
  format: yaml
  label: Ni Biashara Agent identity API
  slug: nibiashara-biz-agent-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibiashara-biz/openapi/nibiashara-biz-agent-identity-api-openapi.yml
- filename: nibiashara-biz-discovery-api-openapi.yml
  format: yaml
  label: Ni Biashara Discovery API
  slug: nibiashara-biz-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibiashara-biz/openapi/nibiashara-biz-discovery-api-openapi.yml
- filename: nibiashara-biz-free-tools-api-openapi.yml
  format: yaml
  label: Ni Biashara Free tools API
  slug: nibiashara-biz-free-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibiashara-biz/openapi/nibiashara-biz-free-tools-api-openapi.yml
- filename: nibiashara-biz-services-api-openapi.yml
  format: yaml
  label: Ni Biashara Services API
  slug: nibiashara-biz-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibiashara-biz/openapi/nibiashara-biz-services-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ni Biashara Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ni Biashara secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ni Biashara
provider_slug: nibiashara-biz
scheme_count: 1
schemes:
- description: 'Shelves agent access token (nbat_). Get one: https://agents.nibiashara.biz/auth.md. Authorization server: https://agents.nibiashara.biz/.well-known/oauth-authorization-server.'
  name: agentBearer
  scheme: bearer
  sources:
  - openapi/agents.nibiashara.biz-openapi.json
  type: http
slug: nibiashara-biz-authentication
source_filename: nibiashara-biz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/agents.nibiashara.biz-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: agentBearer\n  type: http\n  scheme: bearer\n  description: 'Shelves agent access token (nbat_). Get one: https://agents.nibiashara.biz/auth.md.\n    Authorization server: https://agents.nibiashara.biz/.well-known/oauth-authorization-server.'\n  sources:\n  - openapi/agents.nibiashara.biz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nibiashara-biz/authentication/nibiashara-biz-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Automation
- Small Business
- Software-as-a-Service
- Africa
---
