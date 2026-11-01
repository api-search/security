---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pushcut-automation-server-api-openapi.yml
  format: yaml
  label: Pushcut Automation Server API
  slug: pushcut-automation-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pushcut/openapi/pushcut-automation-server-api-openapi.yml
- filename: pushcut-notifications-api-openapi.yml
  format: yaml
  label: Pushcut Notifications API
  slug: pushcut-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pushcut/openapi/pushcut-notifications-api-openapi.yml
- filename: pushcut-subscriptions-api-openapi.yml
  format: yaml
  label: Pushcut Subscriptions API
  slug: pushcut-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pushcut/openapi/pushcut-subscriptions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Pushcut Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pushcut declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Pushcut
provider_slug: pushcut
scheme_count: 1
schemes:
- description: API-Keys can be managed in the Account view of the Pushcut app.
  in: header
  name: API-Key
  type: apiKey
slug: pushcut-authentication
source_filename: pushcut-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: https://api.pushcut.io/openapi.yaml\nschemes:\n  - type: apiKey\n    name: API-Key\n    in: header\n    description: API-Keys can be managed in the Account view of the Pushcut app.\n"
source_yaml_url: https://artifacts.apis.io/pushcut/authentication/pushcut-authentication.yml
summary_line: 1 scheme
tags:
- Company
- automation
- iOS
- shortcuts
- webhooks
- integration
---
