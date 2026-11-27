---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: indiacos-com-account-api-openapi.yml
  format: yaml
  label: IndiaCos Account API
  slug: indiacos-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-account-api-openapi.yml
- filename: indiacos-com-categories-api-openapi.yml
  format: yaml
  label: IndiaCos Categories API
  slug: indiacos-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-categories-api-openapi.yml
- filename: indiacos-com-companies-api-openapi.yml
  format: yaml
  label: IndiaCos Companies API
  slug: indiacos-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-companies-api-openapi.yml
- filename: indiacos-com-company-api-openapi.yml
  format: yaml
  label: IndiaCos Company API
  slug: indiacos-com-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-company-api-openapi.yml
- filename: indiacos-com-copyright-api-openapi.yml
  format: yaml
  label: IndiaCos Copyright API
  slug: indiacos-com-copyright-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-copyright-api-openapi.yml
- filename: indiacos-com-defaulter-api-openapi.yml
  format: yaml
  label: IndiaCos Defaulter API
  slug: indiacos-com-defaulter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-defaulter-api-openapi.yml
- filename: indiacos-com-design-api-openapi.yml
  format: yaml
  label: IndiaCos Design API
  slug: indiacos-com-design-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-design-api-openapi.yml
- filename: indiacos-com-director-api-openapi.yml
  format: yaml
  label: IndiaCos Director API
  slug: indiacos-com-director-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-director-api-openapi.yml
- filename: indiacos-com-doctor-api-openapi.yml
  format: yaml
  label: IndiaCos Doctor API
  slug: indiacos-com-doctor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-doctor-api-openapi.yml
- filename: indiacos-com-find-api-openapi.yml
  format: yaml
  label: IndiaCos Find API
  slug: indiacos-com-find-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-find-api-openapi.yml
- filename: indiacos-com-gst-api-openapi.yml
  format: yaml
  label: IndiaCos Gst API
  slug: indiacos-com-gst-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-gst-api-openapi.yml
- filename: indiacos-com-gst-registrations-api-openapi.yml
  format: yaml
  label: IndiaCos Gst Registrations API
  slug: indiacos-com-gst-registrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-gst-registrations-api-openapi.yml
- filename: indiacos-com-msme-api-openapi.yml
  format: yaml
  label: IndiaCos Msme API
  slug: indiacos-com-msme-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-msme-api-openapi.yml
- filename: indiacos-com-office-api-openapi.yml
  format: yaml
  label: IndiaCos Office API
  slug: indiacos-com-office-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-office-api-openapi.yml
- filename: indiacos-com-pan-api-openapi.yml
  format: yaml
  label: IndiaCos Pan API
  slug: indiacos-com-pan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-pan-api-openapi.yml
- filename: indiacos-com-patent-api-openapi.yml
  format: yaml
  label: IndiaCos Patent API
  slug: indiacos-com-patent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-patent-api-openapi.yml
- filename: indiacos-com-person-api-openapi.yml
  format: yaml
  label: IndiaCos Person API
  slug: indiacos-com-person-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-person-api-openapi.yml
- filename: indiacos-com-search-api-openapi.yml
  format: yaml
  label: IndiaCos Search API
  slug: indiacos-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-search-api-openapi.yml
- filename: indiacos-com-stats-api-openapi.yml
  format: yaml
  label: IndiaCos Stats API
  slug: indiacos-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-stats-api-openapi.yml
- filename: indiacos-com-trademark-api-openapi.yml
  format: yaml
  label: IndiaCos Trademark API
  slug: indiacos-com-trademark-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indiacos-com/openapi/indiacos-com-trademark-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: IndiaCos Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: IndiaCos secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: IndiaCos
provider_slug: indiacos-com
scheme_count: 3
schemes:
- description: API key of your IndiaCos account (https://indiacos.com/signup)
  name: bearer
  scheme: bearer
  sources:
  - openapi/indiacos-com-openapi.json
  type: http
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/indiacos-com-openapi.json
  type: apiKey
- flows:
  - authorizationUrl: https://indiacos.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://indiacos.com/oauth/token
  name: oauth
  sources:
  - openapi/indiacos-com-openapi.json
  type: oauth2
slug: indiacos-com-authentication
source_filename: indiacos-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/indiacos-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: API key of your IndiaCos account (https://indiacos.com/signup)\n  sources:\n  - openapi/indiacos-com-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/indiacos-com-openapi.json\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://indiacos.com/oauth/authorize\n    tokenUrl: https://indiacos.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/indiacos-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/indiacos-com/authentication/indiacos-com-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Data
- Compliance
- India
- Business
- Public Records
---
