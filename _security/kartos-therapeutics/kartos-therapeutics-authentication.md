---
api_key_in: []
api_specs:
- filename: kartos-therapeutics-content-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics Content API
  slug: kartos-therapeutics-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-content-api-openapi.yml
- filename: kartos-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics Discovery API
  slug: kartos-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-discovery-api-openapi.yml
- filename: kartos-therapeutics-media-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics Media API
  slug: kartos-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-media-api-openapi.yml
- filename: kartos-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics Oembed API
  slug: kartos-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-oembed-api-openapi.yml
- filename: kartos-therapeutics-people-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics People API
  slug: kartos-therapeutics-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-people-api-openapi.yml
- filename: kartos-therapeutics-science-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics Science API
  slug: kartos-therapeutics-science-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-science-api-openapi.yml
- filename: kartos-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics Taxonomy API
  slug: kartos-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-taxonomy-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kartos Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kartos Therapeutics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kartos Therapeutics
provider_slug: kartos-therapeutics
scheme_count: 1
schemes:
- description: WordPress application passwords, advertised by the site's own route index at `/wp-json/` (`authentication.application-passwords.endpoints.authorization` → https://kartosthera.com/wp-admin/authorize-application.php). Application passwords are issued to existing WordPress accounts only; there is no public sign-up, no developer registration and no self-service credential issuance. Every operation mod
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/kartos-therapeutics-content-openapi.yml
  type: http
slug: kartos-therapeutics-authentication
source_filename: kartos-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: openapi/kartos-therapeutics-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application passwords, advertised by the site's own route index at\n    `/wp-json/` (`authentication.application-passwords.endpoints.authorization` → https://kartosthera.com/wp-admin/authorize-application.php).\n    Application passwords are issued to existing WordPress accounts only; there is no public\n    sign-up, no developer registration and no self-service credential issuance. Every operation\n    mod\n  sources:\n  - openapi/kartos-therapeutics-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/authentication/kartos-therapeutics-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- biotechnology
- pharmaceuticals
- oncology
- hematology
- rare-disease
- precision-medicine
- clinical-trials
- life-sciences
- content-api
---
