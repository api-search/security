---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bugbug-io-components-api-openapi.yml
  format: yaml
  label: BugBug Components API
  slug: bugbug-io-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-components-api-openapi.yml
- filename: bugbug-io-config-api-openapi.yml
  format: yaml
  label: BugBug Config API
  slug: bugbug-io-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-config-api-openapi.yml
- filename: bugbug-io-folders-api-openapi.yml
  format: yaml
  label: BugBug Folders API
  slug: bugbug-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-folders-api-openapi.yml
- filename: bugbug-io-groups-api-openapi.yml
  format: yaml
  label: BugBug Groups API
  slug: bugbug-io-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-groups-api-openapi.yml
- filename: bugbug-io-import-export-api-openapi.yml
  format: yaml
  label: BugBug Import / Export API
  slug: bugbug-io-import-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-import-export-api-openapi.yml
- filename: bugbug-io-organizations-api-openapi.yml
  format: yaml
  label: BugBug Organizations API
  slug: bugbug-io-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-organizations-api-openapi.yml
- filename: bugbug-io-profiles-api-openapi.yml
  format: yaml
  label: BugBug Profiles API
  slug: bugbug-io-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-profiles-api-openapi.yml
- filename: bugbug-io-projects-api-openapi.yml
  format: yaml
  label: BugBug Projects API
  slug: bugbug-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-projects-api-openapi.yml
- filename: bugbug-io-settings-api-openapi.yml
  format: yaml
  label: BugBug Settings API
  slug: bugbug-io-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-settings-api-openapi.yml
- filename: bugbug-io-step-runs-api-openapi.yml
  format: yaml
  label: BugBug Step runs API
  slug: bugbug-io-step-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-step-runs-api-openapi.yml
- filename: bugbug-io-steps-api-openapi.yml
  format: yaml
  label: BugBug Steps API
  slug: bugbug-io-steps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-steps-api-openapi.yml
- filename: bugbug-io-suite-runs-api-openapi.yml
  format: yaml
  label: BugBug Suite runs API
  slug: bugbug-io-suite-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-suite-runs-api-openapi.yml
- filename: bugbug-io-suites-api-openapi.yml
  format: yaml
  label: BugBug Suites API
  slug: bugbug-io-suites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-suites-api-openapi.yml
- filename: bugbug-io-tags-api-openapi.yml
  format: yaml
  label: BugBug Tags API
  slug: bugbug-io-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-tags-api-openapi.yml
- filename: bugbug-io-test-runs-api-openapi.yml
  format: yaml
  label: BugBug Test runs API
  slug: bugbug-io-test-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-test-runs-api-openapi.yml
- filename: bugbug-io-tests-api-openapi.yml
  format: yaml
  label: BugBug Tests API
  slug: bugbug-io-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-tests-api-openapi.yml
- filename: bugbug-io-variables-api-openapi.yml
  format: yaml
  label: BugBug Variables API
  slug: bugbug-io-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-variables-api-openapi.yml
- filename: bugbug-io-visual-regression-api-openapi.yml
  format: yaml
  label: BugBug Visual regression API
  slug: bugbug-io-visual-regression-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-visual-regression-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bugbug Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: BugBug secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BugBug
provider_slug: bugbug-io
scheme_count: 1
schemes:
- description: Token-based authentication with required prefix "Token"
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/bugbug-io-openapi.json
  type: apiKey
slug: bugbug-io-authentication
source_filename: bugbug-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/bugbug-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication with required prefix \"Token\"\n  sources:\n  - openapi/bugbug-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/bugbug-io/authentication/bugbug-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Testing
- Automation
- Software-as-a-Service
- Low-Code
- No-Code
---
