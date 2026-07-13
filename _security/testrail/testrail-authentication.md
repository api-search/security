---
api_key_in: []
api_specs:
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Test Runs API
  slug: testrail-test-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Test Results API
  slug: testrail-test-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Test Cases API
  slug: testrail-test-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Tests API
  slug: testrail-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Test Plans API
  slug: testrail-test-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Projects API
  slug: testrail-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Test Suites API
  slug: testrail-test-suites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Sections API
  slug: testrail-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Milestones API
  slug: testrail-milestones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Configurations API
  slug: testrail-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Users API
  slug: testrail-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Testrail Authentication
name_suffix: Authentication
oauth_flows: []
overview: TestRail secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TestRail
provider_slug: testrail
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication. The username is your TestRail email address; the password is either your account password or an API key generated under My Settings. Sent as `Authorization: Basic base64(email:api_key)`, for example `curl -u "user@example.com:APIkey"`. All requests and responses are JSON (`Content-Type: application/json`). The API must be enabled by an administrator under Administration > Site Settings > API ("Enable API"). API keys can be revoked at any time under My Settings.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/testrail-openapi.yml
  - https://support.testrail.com/hc/en-us/articles/7077039051284-Accessing-the-TestRail-API
  type: http
slug: testrail-authentication
source_filename: testrail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/testrail-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication. The username is your TestRail email address; the\n    password is either your account password or an API key generated under My\n    Settings. Sent as `Authorization: Basic base64(email:api_key)`, for example\n    `curl -u \"user@example.com:APIkey\"`. All requests and responses are JSON\n    (`Content-Type: application/json`). The API must be enabled by an\n    administrator under Administration > Site Settings > API (\"Enable API\").\n    API keys can be revoked at any time under My Settings.\n  sources:\n  - openapi/testrail-openapi.yml\n  - https://support.testrail.com/hc/en-us/articles/7077039051284-Accessing-the-TestRail-API\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/authentication/testrail-authentication.yml
summary_line: http · 1 scheme
tags:
- Test Runs
- Test Management
- QA
- Test Cases
- Test Results
- Test Plans
- Testing
- Test Automation
---
