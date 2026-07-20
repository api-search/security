---
api_key_in:
- header
api_specs:
- filename: athenian-openapi-original.yml
  format: yaml
  label: Athenian API
  slug: athenian-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-openapi-original.yml
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
