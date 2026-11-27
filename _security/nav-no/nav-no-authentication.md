---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nav-no-feed-api-openapi.yml
  format: yaml
  label: NAV (Norwegian Labour and Welfare Administration) Feed API
  slug: nav-no-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nav-no/openapi/nav-no-feed-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: NAV (Norwegian Labour and Welfare Administration) Authentication
name_suffix: Authentication
oauth_flows: []
overview: NAV (Norwegian Labour and Welfare Administration) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NAV (Norwegian Labour and Welfare Administration)
provider_slug: nav-no
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nav-no-stilling-feed-openapi.yml
  type: http
slug: nav-no-authentication
source_filename: nav-no-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/nav-no-stilling-feed-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/nav-no-stilling-feed-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/nav-no/authentication/nav-no-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Government
- Employment
- Job Vacancies
- Public Sector
- Norway
- Welfare
---
