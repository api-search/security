---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: feranor-com-administration-api-openapi.yml
  format: yaml
  label: Feranor Administration API
  slug: feranor-com-administration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feranor-com/openapi/feranor-com-administration-api-openapi.yml
- filename: feranor-com-health-api-openapi.yml
  format: yaml
  label: Feranor Health API
  slug: feranor-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feranor-com/openapi/feranor-com-health-api-openapi.yml
- filename: feranor-com-keys-api-openapi.yml
  format: yaml
  label: Feranor Keys API
  slug: feranor-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feranor-com/openapi/feranor-com-keys-api-openapi.yml
- filename: feranor-com-operations-api-openapi.yml
  format: yaml
  label: Feranor Operations API
  slug: feranor-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feranor-com/openapi/feranor-com-operations-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Feranor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Feranor secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Feranor
provider_slug: feranor-com
scheme_count: 2
schemes:
- description: 'The access token of Sidecar:AccessTokenFile, on TCP: sent with every request but the health checks, in exactly one Authorization header, and compared in constant time. Any address beyond loopback needs it. On the Unix socket, the default, the socket''s file permissions decide who may call, and no token is sent.'
  name: accessToken
  scheme: bearer
  sources:
  - openapi/feranor-com-sidecar-openapi.json
  type: http
- description: The administration token of Sidecar:AdministrationTokenFile, for /v1/operations and /v1/logs only. It differs from the access token, which is sent too on TCP.
  in: header
  name: administrationToken
  parameter: Feranor-Administration-Token
  sources:
  - openapi/feranor-com-sidecar-openapi.json
  type: apiKey
slug: feranor-com-authentication
source_filename: feranor-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/feranor-com-sidecar-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: accessToken\n  type: http\n  scheme: bearer\n  description: 'The access token of Sidecar:AccessTokenFile, on TCP: sent with every request\n    but the health checks, in exactly one Authorization header, and compared in constant time.\n    Any address beyond loopback needs it. On the Unix socket, the default, the socket''s file\n    permissions decide who may call, and no token is sent.'\n  sources:\n  - openapi/feranor-com-sidecar-openapi.json\n- name: administrationToken\n  type: apiKey\n  in: header\n  parameter: Feranor-Administration-Token\n  description: The administration token of Sidecar:AdministrationTokenFile, for /v1/operations\n    and /v1/logs only. It differs from the access token, which is sent too on TCP.\n  sources:\n  - openapi/feranor-com-sidecar-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/feranor-com/authentication/feranor-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Security
- Encryption
- Post-Quantum
- Consulting
- Artificial Intelligence
---
