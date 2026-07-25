---
api_key_in: []
api_specs:
- filename: sauce-labs-devices-api-openapi.yml
  format: yaml
  label: Sauce Labs Devices API
  slug: sauce-labs-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/openapi/sauce-labs-devices-api-openapi.yml
- filename: sauce-labs-job-assets-api-openapi.yml
  format: yaml
  label: Sauce Labs Job Assets API
  slug: sauce-labs-job-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/openapi/sauce-labs-job-assets-api-openapi.yml
- filename: sauce-labs-jobs-api-openapi.yml
  format: yaml
  label: Sauce Labs Jobs API
  slug: sauce-labs-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/openapi/sauce-labs-jobs-api-openapi.yml
- filename: sauce-labs-platform-api-openapi.yml
  format: yaml
  label: Sauce Labs Platform API
  slug: sauce-labs-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/openapi/sauce-labs-platform-api-openapi.yml
- filename: sauce-labs-sessions-api-openapi.yml
  format: yaml
  label: Sauce Labs Sessions API
  slug: sauce-labs-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/openapi/sauce-labs-sessions-api-openapi.yml
- filename: sauce-labs-users-api-openapi.yml
  format: yaml
  label: Sauce Labs Users API
  slug: sauce-labs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/openapi/sauce-labs-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sauce Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sauce Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sauce Labs
provider_slug: sauce-labs
scheme_count: 1
schemes:
- description: Use your Sauce Labs username and access key as the HTTP Basic Authentication credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/sauce-labs-jobs-openapi.yml
  - openapi/sauce-labs-real-device-access-openapi.yml
  type: http
slug: sauce-labs-authentication
source_filename: sauce-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sauce-labs-jobs-openapi.yml, openapi/sauce-labs-real-device-access-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Use your Sauce Labs username and access key as the HTTP Basic Authentication\n    credentials.\n  sources:\n  - openapi/sauce-labs-jobs-openapi.yml\n  - openapi/sauce-labs-real-device-access-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/authentication/sauce-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Testing
- Cross-Browser Testing
- Mobile Testing
- Real Devices
- Automation
- CI/CD
- Quality Assurance
---
