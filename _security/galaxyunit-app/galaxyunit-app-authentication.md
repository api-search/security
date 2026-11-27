---
anonymous_access: false
api_key_in: []
api_specs:
- filename: galaxyunit-app-actions-api-openapi.yml
  format: yaml
  label: Galaxy Unit Actions API
  slug: galaxyunit-app-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-actions-api-openapi.yml
- filename: galaxyunit-app-business-api-openapi.yml
  format: yaml
  label: Galaxy Unit Business API
  slug: galaxyunit-app-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-business-api-openapi.yml
- filename: galaxyunit-app-contacts-api-openapi.yml
  format: yaml
  label: Galaxy Unit Contacts API
  slug: galaxyunit-app-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-contacts-api-openapi.yml
- filename: galaxyunit-app-estimate-api-openapi.yml
  format: yaml
  label: Galaxy Unit Estimate API
  slug: galaxyunit-app-estimate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-estimate-api-openapi.yml
- filename: galaxyunit-app-events-api-openapi.yml
  format: yaml
  label: Galaxy Unit Events API
  slug: galaxyunit-app-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-events-api-openapi.yml
- filename: galaxyunit-app-expenses-api-openapi.yml
  format: yaml
  label: Galaxy Unit Expenses API
  slug: galaxyunit-app-expenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-expenses-api-openapi.yml
- filename: galaxyunit-app-invoices-api-openapi.yml
  format: yaml
  label: Galaxy Unit Invoices API
  slug: galaxyunit-app-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-invoices-api-openapi.yml
- filename: galaxyunit-app-jobs-api-openapi.yml
  format: yaml
  label: Galaxy Unit Jobs API
  slug: galaxyunit-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-jobs-api-openapi.yml
- filename: galaxyunit-app-me-api-openapi.yml
  format: yaml
  label: Galaxy Unit Me API
  slug: galaxyunit-app-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-me-api-openapi.yml
- filename: galaxyunit-app-quotes-api-openapi.yml
  format: yaml
  label: Galaxy Unit Quotes API
  slug: galaxyunit-app-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/galaxyunit-app/openapi/galaxyunit-app-quotes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Galaxy Unit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Galaxy Unit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Galaxy Unit
provider_slug: galaxyunit-app
scheme_count: 1
schemes:
- description: 'Authorization: Bearer gu_live_… — issued in Settings → Integrations by an owner or admin.'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/galaxyunit-app-openapi.json
  type: http
slug: galaxyunit-app-authentication
source_filename: galaxyunit-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/galaxyunit-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer gu_live_… — issued in Settings → Integrations by an owner\n    or admin.'\n  sources:\n  - openapi/galaxyunit-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/galaxyunit-app/authentication/galaxyunit-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Business
- Software-as-a-Service
- ServiceIndustry
- Artificial Intelligence
---
