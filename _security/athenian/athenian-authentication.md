---
api_key_in:
- header
api_specs:
- filename: athenian-align-api-openapi.yml
  format: yaml
  label: Athenian align API
  slug: athenian-align-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-align-api-openapi.yml
- filename: athenian-events-api-openapi.yml
  format: yaml
  label: Athenian events API
  slug: athenian-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-events-api-openapi.yml
- filename: athenian-filter-api-openapi.yml
  format: yaml
  label: Athenian filter API
  slug: athenian-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-filter-api-openapi.yml
- filename: athenian-get-api-openapi.yml
  format: yaml
  label: Athenian get API
  slug: athenian-get-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-get-api-openapi.yml
- filename: athenian-histograms-api-openapi.yml
  format: yaml
  label: Athenian histograms API
  slug: athenian-histograms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-histograms-api-openapi.yml
- filename: athenian-integrations-api-openapi.yml
  format: yaml
  label: Athenian integrations API
  slug: athenian-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-integrations-api-openapi.yml
- filename: athenian-metrics-api-openapi.yml
  format: yaml
  label: Athenian metrics API
  slug: athenian-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-metrics-api-openapi.yml
- filename: athenian-pagination-api-openapi.yml
  format: yaml
  label: Athenian pagination API
  slug: athenian-pagination-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-pagination-api-openapi.yml
- filename: athenian-registration-api-openapi.yml
  format: yaml
  label: Athenian registration API
  slug: athenian-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-registration-api-openapi.yml
- filename: athenian-reposet-api-openapi.yml
  format: yaml
  label: Athenian reposet API
  slug: athenian-reposet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-reposet-api-openapi.yml
- filename: athenian-security-api-openapi.yml
  format: yaml
  label: Athenian security API
  slug: athenian-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-security-api-openapi.yml
- filename: athenian-settings-api-openapi.yml
  format: yaml
  label: Athenian settings API
  slug: athenian-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-settings-api-openapi.yml
- filename: athenian-team-api-openapi.yml
  format: yaml
  label: Athenian team API
  slug: athenian-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-team-api-openapi.yml
- filename: athenian-user-api-openapi.yml
  format: yaml
  label: Athenian user API
  slug: athenian-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-user-api-openapi.yml
- filename: athenian-version-api-openapi.yml
  format: yaml
  label: Athenian version API
  slug: athenian-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-version-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Athenian Authentication
name_suffix: Authentication
oauth_flows: []
overview: Athenian secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Athenian
provider_slug: athenian
scheme_count: 2
schemes:
- description: 'Authorization by the value of `X-API-Key` header aka API token.

    The tokens are user- and account-specific. Create them by calling `/token/create`.

    The server automatically inserts `account` in the request''s body if it was not

    supplied by the user.'
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/athenian-openapi-original.yml
  type: apiKey
- bearerFormat: JWT
  description: 'Regular JSON Web Token authorization powered by Auth0.

    The server expects an `Authorization: Bearer <token>` header and checks `<token>` by

    sending it to Auth0. Visit [{{ server_url | replace("api", "app") }}/bearer]({{ server_url | replace("api", "app") }}/bearer)

    to copy your current JWT that will expire within 24 hours.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/athenian-openapi-original.yml
  type: http
slug: athenian-authentication
source_filename: athenian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/athenian-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: |-\n    Authorization by the value of `X-API-Key` header aka API token.\n    The tokens are user- and account-specific. Create them by calling `/token/create`.\n    The server automatically inserts `account` in the request's body if it was not\n    supplied by the user.\n  sources:\n  - openapi/athenian-openapi-original.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Regular JSON Web Token authorization powered by Auth0.\n    The server expects an `Authorization: Bearer <token>` header and checks `<token>` by\n    sending it to Auth0. Visit [{{ server_url | replace(\"api\", \"app\") }}/bearer]({{ server_url | replace(\"api\", \"app\") }}/bearer)\n    to copy your current\
  \ JWT that will expire within 24 hours.\n  sources:\n  - openapi/athenian-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/authentication/athenian-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Engineering Intelligence
- Software Development Analytics
- Developer Productivity
- DevOps
- Metrics
- Git
- JIRA
- CI/CD
- Analytics
---
