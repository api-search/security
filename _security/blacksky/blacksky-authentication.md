---
anonymous_access: false
api_key_in: []
api_specs:
- filename: blacksky-budgets-api-openapi.yml
  format: yaml
  label: BlackSky Budgets API
  slug: blacksky-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-budgets-api-openapi.yml
- filename: blacksky-catalog-api-openapi.yml
  format: yaml
  label: BlackSky Catalog API
  slug: blacksky-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-catalog-api-openapi.yml
- filename: blacksky-data-management-api-openapi.yml
  format: yaml
  label: BlackSky Data management API
  slug: blacksky-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-data-management-api-openapi.yml
- filename: blacksky-eulas-api-openapi.yml
  format: yaml
  label: BlackSky EULAs API
  slug: blacksky-eulas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-eulas-api-openapi.yml
- filename: blacksky-geometries-api-openapi.yml
  format: yaml
  label: BlackSky Geometries API
  slug: blacksky-geometries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-geometries-api-openapi.yml
- filename: blacksky-glossary-api-openapi.yml
  format: yaml
  label: BlackSky Glossary API
  slug: blacksky-glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-glossary-api-openapi.yml
- filename: blacksky-orders-api-openapi.yml
  format: yaml
  label: BlackSky Orders API
  slug: blacksky-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-orders-api-openapi.yml
- filename: blacksky-processing-api-openapi.yml
  format: yaml
  label: BlackSky Processing API
  slug: blacksky-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-processing-api-openapi.yml
- filename: blacksky-tasking-api-openapi.yml
  format: yaml
  label: BlackSky Tasking API
  slug: blacksky-tasking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-tasking-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Blacksky Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: BlackSky secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: BlackSky
provider_slug: blacksky
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: httpBearer
  scheme: bearer
  sources:
  - openapi/blacksky-up42-api-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://auth.up42.com/realms/public/protocol/openid-connect/token
  - authorizationUrl: https://auth.up42.com/realms/public/protocol/openid-connect/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://auth.up42.com/realms/public/protocol/openid-connect/token
  name: oauth2Profiles
  sources:
  - openapi/blacksky-up42-api-openapi.yml
  type: oauth2
slug: blacksky-authentication
source_filename: blacksky-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/blacksky-up42-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: httpBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/blacksky-up42-api-openapi.yml\n- name: oauth2Profiles\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.up42.com/realms/public/protocol/openid-connect/token\n    scopes: 2\n  - flow: authorizationCode\n    authorizationUrl: https://auth.up42.com/realms/public/protocol/openid-connect/auth\n    tokenUrl: https://auth.up42.com/realms/public/protocol/openid-connect/token\n    scopes: 2\n  sources:\n  - openapi/blacksky-up42-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/authentication/blacksky-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Earth Observation
- Satellite Imagery
- Remote Sensing
- Geospatial Intelligence
- Space
- ISR
- Intelligence Surveillance Reconnaissance
- Tasking
- AI Analytics
- Object Detection
- Defense
- Monitoring
- Spectra
- Gen-3
- NYSE BKSY
---
