---
api_key_in: []
api_specs:
- filename: kobiton-openapi.yml
  format: yaml
  label: Kobiton Devices API
  slug: kobiton-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kobiton/refs/heads/main/openapi/kobiton-openapi.yml
- filename: kobiton-openapi.yml
  format: yaml
  label: Kobiton Sessions API
  slug: kobiton-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kobiton/refs/heads/main/openapi/kobiton-openapi.yml
- filename: kobiton-openapi.yml
  format: yaml
  label: Kobiton Scriptless Automation API
  slug: kobiton-scriptless-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kobiton/refs/heads/main/openapi/kobiton-openapi.yml
- filename: kobiton-openapi.yml
  format: yaml
  label: Kobiton Apps Repository API
  slug: kobiton-apps-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kobiton/refs/heads/main/openapi/kobiton-openapi.yml
- filename: kobiton-openapi.yml
  format: yaml
  label: Kobiton Data-Driven Testing API
  slug: kobiton-data-driven-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kobiton/refs/heads/main/openapi/kobiton-openapi.yml
- filename: kobiton-openapi.yml
  format: yaml
  label: Kobiton Organization API
  slug: kobiton-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kobiton/refs/heads/main/openapi/kobiton-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kobiton Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kobiton secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kobiton
provider_slug: kobiton
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication over HTTPS. Use your Kobiton username (or email) as the username and your Kobiton API key as the password. The pair is base64-encoded and sent in the `Authorization: Basic <encoded>` header (for example, `curl -u <USERNAME>:<API_KEY>`). API keys are created and managed in the Kobiton portal under API Keys settings. The Appium/WebDriver hub at https://api.kobiton.com/wd/hub instead takes the username and API key via Kobiton desired capabilities.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/kobiton-openapi.yml
  - https://api.kobiton.com/docs
  - https://github.com/kobiton/samples/tree/master/kobiton-rest-api/get-devices-info
  type: http
slug: kobiton-authentication
source_filename: kobiton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kobiton-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication over HTTPS. Use your Kobiton username (or email)\n    as the username and your Kobiton API key as the password. The pair is\n    base64-encoded and sent in the `Authorization: Basic <encoded>` header (for\n    example, `curl -u <USERNAME>:<API_KEY>`). API keys are created and managed\n    in the Kobiton portal under API Keys settings. The Appium/WebDriver hub at\n    https://api.kobiton.com/wd/hub instead takes the username and API key via\n    Kobiton desired capabilities.\n  sources:\n  - openapi/kobiton-openapi.yml\n  - https://api.kobiton.com/docs\n  - https://github.com/kobiton/samples/tree/master/kobiton-rest-api/get-devices-info\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kobiton/refs/heads/main/authentication/kobiton-authentication.yml
summary_line: http · 1 scheme
tags:
- Mobile Testing
- Test Runs
- Device Cloud
- Real Devices
- Appium
- Automation Testing
- Visual Testing
- QA
- Mobile
---
