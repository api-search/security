---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kahvetabela-com-agent-api-openapi.yml
  format: yaml
  label: Kahve Tabela Agent API
  slug: kahvetabela-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kahvetabela-com/openapi/kahvetabela-com-agent-api-openapi.yml
- filename: kahvetabela-com-locations-api-openapi.yml
  format: yaml
  label: Kahve Tabela Locations API
  slug: kahvetabela-com-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kahvetabela-com/openapi/kahvetabela-com-locations-api-openapi.yml
- filename: kahvetabela-com-nearby-api-openapi.yml
  format: yaml
  label: Kahve Tabela Nearby API
  slug: kahvetabela-com-nearby-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kahvetabela-com/openapi/kahvetabela-com-nearby-api-openapi.yml
- filename: kahvetabela-com-partners-api-openapi.yml
  format: yaml
  label: Kahve Tabela Partners API
  slug: kahvetabela-com-partners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kahvetabela-com/openapi/kahvetabela-com-partners-api-openapi.yml
- filename: kahvetabela-com-place-audio-api-openapi.yml
  format: yaml
  label: Kahve Tabela Place Audio API
  slug: kahvetabela-com-place-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kahvetabela-com/openapi/kahvetabela-com-place-audio-api-openapi.yml
- filename: kahvetabela-com-place-media-api-openapi.yml
  format: yaml
  label: Kahve Tabela Place Media API
  slug: kahvetabela-com-place-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kahvetabela-com/openapi/kahvetabela-com-place-media-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Kahve Tabela Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kahve Tabela secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kahve Tabela
provider_slug: kahvetabela-com
scheme_count: 1
schemes:
- description: 'Partner API key (`Authorization: Bearer <key>`), provisioned out-of-band by Kahve Tabela. Keys are metered monthly and can be revoked.'
  name: partnerBearer
  scheme: bearer
  sources:
  - openapi/kahvetabela-com-openapi.json
  type: http
slug: kahvetabela-com-authentication
source_filename: kahvetabela-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/kahvetabela-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: partnerBearer\n  type: http\n  scheme: bearer\n  description: 'Partner API key (`Authorization: Bearer <key>`), provisioned out-of-band by\n    Kahve Tabela. Keys are metered monthly and can be revoked.'\n  sources:\n  - openapi/kahvetabela-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kahvetabela-com/authentication/kahvetabela-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Cultural Heritage
- Mapping
- Open Data
- Turkey
- Travel
---
