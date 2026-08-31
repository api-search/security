---
api_key_in:
- header
api_specs:
- filename: ownlocal-ads-api-openapi.yml
  format: yaml
  label: OwnLocal Ads API
  slug: ownlocal-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownlocal/refs/heads/main/openapi/ownlocal-ads-api-openapi.yml
- filename: ownlocal-businesses-api-openapi.yml
  format: yaml
  label: OwnLocal Businesses API
  slug: ownlocal-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownlocal/refs/heads/main/openapi/ownlocal-businesses-api-openapi.yml
- filename: ownlocal-categories-api-openapi.yml
  format: yaml
  label: OwnLocal Categories API
  slug: ownlocal-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownlocal/refs/heads/main/openapi/ownlocal-categories-api-openapi.yml
- filename: ownlocal-reports-data-api-api-openapi.yml
  format: yaml
  label: OwnLocal Reports Data API
  slug: ownlocal-reports-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ownlocal/refs/heads/main/openapi/ownlocal-reports-data-api-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ownlocal Authentication
name_suffix: Authentication
oauth_flows: []
overview: OwnLocal secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OwnLocal
provider_slug: ownlocal
scheme_count: 1
schemes:
- description: Organization API key sent raw (no scheme prefix) in the Authorization header. Keys are issued by OwnLocal support; there is no self-serve key provisioning.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/ownlocal-ads-openapi.yml
  - openapi/ownlocal-businesses-openapi.yml
  - openapi/ownlocal-categories-openapi.yml
  - openapi/ownlocal-reports-data-api-openapi.yml
  type: apiKey
slug: ownlocal-authentication
source_filename: ownlocal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/ownlocal-ads-openapi.yml, openapi/ownlocal-businesses-openapi.yml, openapi/ownlocal-categories-openapi.yml,\n  openapi/ownlocal-reports-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Organization API key sent raw (no scheme prefix) in the Authorization header.\n    Keys are issued by OwnLocal support; there is no self-serve key provisioning.\n  sources:\n  - openapi/ownlocal-ads-openapi.yml\n  - openapi/ownlocal-businesses-openapi.yml\n  - openapi/ownlocal-categories-openapi.yml\n  - openapi/ownlocal-reports-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ownlocal/refs/heads/main/authentication/ownlocal-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Advertising
- Local Media
- Digital Advertising
- Marketing
- Newspapers
- AdTech
- Print to Digital
- Business Listings
- Local Business Data
- Ad Reporting
- Publishers
---
