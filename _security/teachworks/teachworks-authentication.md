---
api_key_in:
- header
api_specs:
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Customers API
  slug: teachworks-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Students API
  slug: teachworks-students-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Employees API
  slug: teachworks-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Lessons API
  slug: teachworks-lessons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Events and Availability API
  slug: teachworks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Services and Subjects API
  slug: teachworks-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Invoices API
  slug: teachworks-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Payments API
  slug: teachworks-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Wages API
  slug: teachworks-wages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Results and Repertoires API
  slug: teachworks-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Teachworks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teachworks secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Teachworks
provider_slug: teachworks
scheme_count: 1
schemes:
- description: 'Account API token passed in the Authorization header using the scheme "Authorization: Token token=API_TOKEN". Generate a token on the Integrations and Add-ons page in Teachworks. All requests must be over HTTPS.'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/teachworks-openapi.yml
  type: apiKey
slug: teachworks-authentication
source_filename: teachworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/teachworks-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Account API token passed in the Authorization header using the scheme \"Authorization:\n    Token token=API_TOKEN\". Generate a token on the Integrations and Add-ons page in Teachworks.\n    All requests must be over HTTPS.'\n  sources:\n  - openapi/teachworks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/authentication/teachworks-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Tutoring
- EdTech
- Scheduling
- Business Management
- CRM
- Billing
---
