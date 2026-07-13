---
api_key_in: []
api_specs:
- filename: sauce.json
  format: json
  label: Sauce Labs Jobs API
  slug: jobs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/sauce.json
- filename: rdc.json
  format: json
  label: Sauce Labs Real Device API
  slug: real-devices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/rdc.json
- filename: real-device-access-api-spec.yaml
  format: yaml
  label: Sauce Labs Real Device Access API
  slug: real-device-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/real-device-access-api-spec.yaml
- filename: accounts.yml
  format: yaml
  label: Sauce Labs Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/accounts.yml
- filename: buildsv2.json
  format: json
  label: Sauce Labs Builds API
  slug: builds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/buildsv2.json
- filename: test-authoring-api.json
  format: json
  label: Sauce Labs Test Authoring API
  slug: test-authoring
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/test-authoring-api.json
- filename: performance.json
  format: json
  label: Sauce Labs Performance API
  slug: performance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/performance.json
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
