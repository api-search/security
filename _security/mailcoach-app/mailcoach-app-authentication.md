---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailcoach-app-automation-mails-api-openapi.yml
  format: yaml
  label: Mailcoach Automation Mails API
  slug: mailcoach-app-automation-mails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-automation-mails-api-openapi.yml
- filename: mailcoach-app-automations-api-openapi.yml
  format: yaml
  label: Mailcoach Automations API
  slug: mailcoach-app-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-automations-api-openapi.yml
- filename: mailcoach-app-campaign-statistics-api-openapi.yml
  format: yaml
  label: Mailcoach Campaign Statistics API
  slug: mailcoach-app-campaign-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-campaign-statistics-api-openapi.yml
- filename: mailcoach-app-campaigns-api-openapi.yml
  format: yaml
  label: Mailcoach Campaigns API
  slug: mailcoach-app-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-campaigns-api-openapi.yml
- filename: mailcoach-app-links-api-openapi.yml
  format: yaml
  label: Mailcoach Links API
  slug: mailcoach-app-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-links-api-openapi.yml
- filename: mailcoach-app-lists-api-openapi.yml
  format: yaml
  label: Mailcoach Lists API
  slug: mailcoach-app-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-lists-api-openapi.yml
- filename: mailcoach-app-segments-api-openapi.yml
  format: yaml
  label: Mailcoach Segments API
  slug: mailcoach-app-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-segments-api-openapi.yml
- filename: mailcoach-app-sends-api-openapi.yml
  format: yaml
  label: Mailcoach Sends API
  slug: mailcoach-app-sends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-sends-api-openapi.yml
- filename: mailcoach-app-subscriber-imports-api-openapi.yml
  format: yaml
  label: Mailcoach Subscriber Imports API
  slug: mailcoach-app-subscriber-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-subscriber-imports-api-openapi.yml
- filename: mailcoach-app-subscribers-api-openapi.yml
  format: yaml
  label: Mailcoach Subscribers API
  slug: mailcoach-app-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-subscribers-api-openapi.yml
- filename: mailcoach-app-suppressions-api-openapi.yml
  format: yaml
  label: Mailcoach Suppressions API
  slug: mailcoach-app-suppressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-suppressions-api-openapi.yml
- filename: mailcoach-app-tags-api-openapi.yml
  format: yaml
  label: Mailcoach Tags API
  slug: mailcoach-app-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-tags-api-openapi.yml
- filename: mailcoach-app-templates-api-openapi.yml
  format: yaml
  label: Mailcoach Templates API
  slug: mailcoach-app-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-templates-api-openapi.yml
- filename: mailcoach-app-transactional-mails-api-openapi.yml
  format: yaml
  label: Mailcoach Transactional Mails API
  slug: mailcoach-app-transactional-mails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-transactional-mails-api-openapi.yml
- filename: mailcoach-app-uploads-api-openapi.yml
  format: yaml
  label: Mailcoach Uploads API
  slug: mailcoach-app-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-uploads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Mailcoach Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailcoach secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mailcoach
provider_slug: mailcoach-app
scheme_count: 1
schemes:
- description: Laravel Sanctum API token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mailcoach-app-openapi.yml
  type: http
slug: mailcoach-app-authentication
source_filename: mailcoach-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/mailcoach-app-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Laravel Sanctum API token\n  sources:\n  - openapi/mailcoach-app-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/mailcoach-app/authentication/mailcoach-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Email
- Marketing
- GDPR
---
