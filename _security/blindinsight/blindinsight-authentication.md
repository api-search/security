---
api_key_in:
- cookie
api_specs:
- filename: blindinsight-accounts-api-openapi.yml
  format: yaml
  label: BlindInsight accounts API
  slug: blindinsight-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-accounts-api-openapi.yml
- filename: blindinsight-blindllm-api-openapi.yml
  format: yaml
  label: BlindInsight blindllm API
  slug: blindinsight-blindllm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-blindllm-api-openapi.yml
- filename: blindinsight-blindllm-queries-api-openapi.yml
  format: yaml
  label: BlindInsight blindllm-queries API
  slug: blindinsight-blindllm-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-blindllm-queries-api-openapi.yml
- filename: blindinsight-csrf-api-openapi.yml
  format: yaml
  label: BlindInsight csrf API
  slug: blindinsight-csrf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-csrf-api-openapi.yml
- filename: blindinsight-datasets-api-openapi.yml
  format: yaml
  label: BlindInsight datasets API
  slug: blindinsight-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-datasets-api-openapi.yml
- filename: blindinsight-delete-jobs-api-openapi.yml
  format: yaml
  label: BlindInsight delete-jobs API
  slug: blindinsight-delete-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-delete-jobs-api-openapi.yml
- filename: blindinsight-files-api-openapi.yml
  format: yaml
  label: BlindInsight files API
  slug: blindinsight-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-files-api-openapi.yml
- filename: blindinsight-grants-api-openapi.yml
  format: yaml
  label: BlindInsight grants API
  slug: blindinsight-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-grants-api-openapi.yml
- filename: blindinsight-identities-api-openapi.yml
  format: yaml
  label: BlindInsight identities API
  slug: blindinsight-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-identities-api-openapi.yml
- filename: blindinsight-jobs-api-openapi.yml
  format: yaml
  label: BlindInsight jobs API
  slug: blindinsight-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-jobs-api-openapi.yml
- filename: blindinsight-materials-api-openapi.yml
  format: yaml
  label: BlindInsight materials API
  slug: blindinsight-materials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-materials-api-openapi.yml
- filename: blindinsight-organizations-api-openapi.yml
  format: yaml
  label: BlindInsight organizations API
  slug: blindinsight-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-organizations-api-openapi.yml
- filename: blindinsight-records-api-openapi.yml
  format: yaml
  label: BlindInsight records API
  slug: blindinsight-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-records-api-openapi.yml
- filename: blindinsight-requests-api-openapi.yml
  format: yaml
  label: BlindInsight requests API
  slug: blindinsight-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-requests-api-openapi.yml
- filename: blindinsight-schemas-api-openapi.yml
  format: yaml
  label: BlindInsight schemas API
  slug: blindinsight-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-schemas-api-openapi.yml
- filename: blindinsight-status-api-openapi.yml
  format: yaml
  label: BlindInsight status API
  slug: blindinsight-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-status-api-openapi.yml
- filename: blindinsight-token-api-openapi.yml
  format: yaml
  label: BlindInsight token API
  slug: blindinsight-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-token-api-openapi.yml
- filename: blindinsight-users-api-openapi.yml
  format: yaml
  label: BlindInsight users API
  slug: blindinsight-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-users-api-openapi.yml
- filename: blindinsight-ws-api-openapi.yml
  format: yaml
  label: BlindInsight ws API
  slug: blindinsight-ws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-ws-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Blindinsight Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlindInsight secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BlindInsight
provider_slug: blindinsight
scheme_count: 3
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/blindinsight-openapi-original.yml
  type: http
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/blindinsight-openapi-original.yml
  type: apiKey
- bearerFormat: JWT
  name: jwtAuth
  scheme: bearer
  sources:
  - openapi/blindinsight-openapi-original.yml
  type: http
slug: blindinsight-authentication
source_filename: blindinsight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/blindinsight-openapi-original.yml\ndocs: https://docs.blindinsight.io/api-reference/authentication/\nnotes: >-\n  Three authentication methods are documented. JWT Bearer is recommended for\n  production: obtain a token pair via POST /api/token/, send the access token as\n  `Authorization: Bearer <access_token>`, and refresh via POST /api/token/refresh/.\n  HTTP Basic sends `Authorization: Basic <base64(email:password)>` on every request\n  and is the default used by the local Blind Proxy and the blind-ml library.\n  Session/cookie auth uses a `sessionid` cookie after POST /api/accounts/login/,\n  with a CSRF token from GET /api/csrf/. All endpoints require credentials on every\n  request except the public GET /api/status/ health check.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/blindinsight-openapi-original.yml\n\
  - name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/blindinsight-openapi-original.yml\n- name: jwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/blindinsight-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/authentication/blindinsight-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Security
- Encryption
- Privacy
- Confidential Computing
- Data
- Machine Learning
- Compliance
- Cryptography
---
