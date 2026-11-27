---
anonymous_access: false
api_key_in: []
api_specs:
- filename: panembrivdienu-lv-calendar-api-openapi.yml
  format: yaml
  label: Paņem brīvdienu Calendar API
  slug: panembrivdienu-lv-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/panembrivdienu-lv/openapi/panembrivdienu-lv-calendar-api-openapi.yml
- filename: panembrivdienu-lv-entitlement-api-openapi.yml
  format: yaml
  label: Paņem brīvdienu Entitlement API
  slug: panembrivdienu-lv-entitlement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/panembrivdienu-lv/openapi/panembrivdienu-lv-entitlement-api-openapi.yml
- filename: panembrivdienu-lv-health-api-openapi.yml
  format: yaml
  label: Paņem brīvdienu Health API
  slug: panembrivdienu-lv-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/panembrivdienu-lv/openapi/panembrivdienu-lv-health-api-openapi.yml
- filename: panembrivdienu-lv-optimize-api-openapi.yml
  format: yaml
  label: Paņem brīvdienu Optimize API
  slug: panembrivdienu-lv-optimize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/panembrivdienu-lv/openapi/panembrivdienu-lv-optimize-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Paņem brīvdienu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paņem brīvdienu secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paņem brīvdienu
provider_slug: panembrivdienu-lv
scheme_count: 1
schemes:
- description: Optional. Raises the rate limit; a supplied but unknown key returns 401.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/panembrivdienu-lv-openapi.yml
  type: http
slug: panembrivdienu-lv-authentication
source_filename: panembrivdienu-lv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/panembrivdienu-lv-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: Optional. Raises the rate limit; a supplied but unknown key returns 401.\n  sources:\n  - openapi/panembrivdienu-lv-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/panembrivdienu-lv/authentication/panembrivdienu-lv-authentication.yml
summary_line: http · 1 scheme
tags:
- Calendar
- Latvia
- Holidays
- Workdays
- Planner
---
