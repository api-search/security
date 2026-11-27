---
anonymous_access: false
api_key_in: []
api_specs:
- filename: justbacked-com-applications-api-openapi.yml
  format: yaml
  label: JustBacked Applications API
  slug: justbacked-com-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justbacked-com/openapi/justbacked-com-applications-api-openapi.yml
- filename: justbacked-com-companies-api-openapi.yml
  format: yaml
  label: JustBacked Companies API
  slug: justbacked-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justbacked-com/openapi/justbacked-com-companies-api-openapi.yml
- filename: justbacked-com-jobs-api-openapi.yml
  format: yaml
  label: JustBacked Jobs API
  slug: justbacked-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justbacked-com/openapi/justbacked-com-jobs-api-openapi.yml
- filename: justbacked-com-lists-api-openapi.yml
  format: yaml
  label: JustBacked Lists API
  slug: justbacked-com-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justbacked-com/openapi/justbacked-com-lists-api-openapi.yml
- filename: justbacked-com-me-api-openapi.yml
  format: yaml
  label: JustBacked Me API
  slug: justbacked-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justbacked-com/openapi/justbacked-com-me-api-openapi.yml
- filename: justbacked-com-saved-searches-api-openapi.yml
  format: yaml
  label: JustBacked Saved Searches API
  slug: justbacked-com-saved-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justbacked-com/openapi/justbacked-com-saved-searches-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: JustBacked Authentication
name_suffix: Authentication
oauth_flows: []
overview: JustBacked secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JustBacked
provider_slug: justbacked-com
scheme_count: 1
schemes:
- description: Member API key (jb_live_...). X-Api-Key also works.
  name: bearer
  scheme: bearer
  sources:
  - openapi/justbacked-com-openapi.json
  type: http
slug: justbacked-com-authentication
source_filename: justbacked-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/justbacked-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Member API key (jb_live_...). X-Api-Key also works.\n  sources:\n  - openapi/justbacked-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/justbacked-com/authentication/justbacked-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Job
- Startups
- Hiring
- Venture
---
