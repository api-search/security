---
api_key_in:
- header
api_specs:
- filename: travis-ci-builds-api-openapi.yml
  format: yaml
  label: Travis CI Builds API
  slug: travis-ci-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travis-ci/refs/heads/main/openapi/travis-ci-builds-api-openapi.yml
- filename: travis-ci-jobs-api-openapi.yml
  format: yaml
  label: Travis CI Jobs API
  slug: travis-ci-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travis-ci/refs/heads/main/openapi/travis-ci-jobs-api-openapi.yml
- filename: travis-ci-logs-api-openapi.yml
  format: yaml
  label: Travis CI Logs API
  slug: travis-ci-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travis-ci/refs/heads/main/openapi/travis-ci-logs-api-openapi.yml
- filename: travis-ci-organizations-api-openapi.yml
  format: yaml
  label: Travis CI Organizations API
  slug: travis-ci-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travis-ci/refs/heads/main/openapi/travis-ci-organizations-api-openapi.yml
- filename: travis-ci-repositories-api-openapi.yml
  format: yaml
  label: Travis CI Repositories API
  slug: travis-ci-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travis-ci/refs/heads/main/openapi/travis-ci-repositories-api-openapi.yml
- filename: travis-ci-users-api-openapi.yml
  format: yaml
  label: Travis CI Users API
  slug: travis-ci-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travis-ci/refs/heads/main/openapi/travis-ci-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Travis Ci Authentication
name_suffix: Authentication
oauth_flows: []
overview: Travis CI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Travis CI
provider_slug: travis-ci
scheme_count: 1
schemes:
- description: 'Token-based authentication. Header format: `Authorization: token <TOKEN>`

    with `Travis-API-Version: 3`. Tokens for travis-ci.com, travis-ci.org,

    and Enterprise installations are not interchangeable.'
  in: header
  name: TravisToken
  parameter: Authorization
  sources:
  - openapi/travis-ci-openapi.yml
  type: apiKey
slug: travis-ci-authentication
source_filename: travis-ci-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/travis-ci-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TravisToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Token-based authentication. Header format: `Authorization: token <TOKEN>`\n    with `Travis-API-Version: 3`. Tokens for travis-ci.com, travis-ci.org,\n    and Enterprise installations are not interchangeable.\n  sources:\n  - openapi/travis-ci-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travis-ci/refs/heads/main/authentication/travis-ci-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DevOps
- CI/CD
- Builds
- Open-Source
- Hosted
- GitHub
---
