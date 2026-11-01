---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sendar-app-emails-api-openapi.yml
  format: yaml
  label: sendar-app Emails API
  slug: sendar-app-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendar-app/openapi/sendar-app-emails-api-openapi.yml
- filename: sendar-app-headless-api-openapi.yml
  format: yaml
  label: sendar-app Headless API
  slug: sendar-app-headless-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendar-app/openapi/sendar-app-headless-api-openapi.yml
- filename: sendar-app-inboxes-api-openapi.yml
  format: yaml
  label: sendar-app Inboxes API
  slug: sendar-app-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendar-app/openapi/sendar-app-inboxes-api-openapi.yml
- filename: sendar-app-link-checks-api-openapi.yml
  format: yaml
  label: sendar-app Link Checks API
  slug: sendar-app-link-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendar-app/openapi/sendar-app-link-checks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Sendar App Authentication
name_suffix: Authentication
oauth_flows: []
overview: sendar-app secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: sendar-app
provider_slug: sendar-app
scheme_count: 1
schemes:
- description: Explicitly scoped sndh_ management key created by the workspace owner.
  name: managementKey
  scheme: bearer
  sources:
  - openapi/sendar-app-headless-openapi.json
  - openapi/sendar-app-openapi.json
  type: http
slug: sendar-app-authentication
source_filename: sendar-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/sendar-app-headless-openapi.json, openapi/sendar-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: managementKey\n  type: http\n  scheme: bearer\n  description: Explicitly scoped sndh_ management key created by the workspace owner.\n  sources:\n  - openapi/sendar-app-headless-openapi.json\n  - openapi/sendar-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/sendar-app/authentication/sendar-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Logistics
- Delivery
- API
- Automation
---
