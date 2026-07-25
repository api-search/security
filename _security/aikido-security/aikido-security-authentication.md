---
api_key_in: []
api_specs:
- filename: aikido-security-clouds-api-openapi.yml
  format: yaml
  label: Aikido Security Clouds API
  slug: aikido-security-clouds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/openapi/aikido-security-clouds-api-openapi.yml
- filename: aikido-security-code-repositories-api-openapi.yml
  format: yaml
  label: Aikido Security Code Repositories API
  slug: aikido-security-code-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/openapi/aikido-security-code-repositories-api-openapi.yml
- filename: aikido-security-compliance-api-openapi.yml
  format: yaml
  label: Aikido Security Compliance API
  slug: aikido-security-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/openapi/aikido-security-compliance-api-openapi.yml
- filename: aikido-security-containers-api-openapi.yml
  format: yaml
  label: Aikido Security Containers API
  slug: aikido-security-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/openapi/aikido-security-containers-api-openapi.yml
- filename: aikido-security-custom-rules-api-openapi.yml
  format: yaml
  label: Aikido Security Custom Rules API
  slug: aikido-security-custom-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/openapi/aikido-security-custom-rules-api-openapi.yml
- filename: aikido-security-domains-api-openapi.yml
  format: yaml
  label: Aikido Security Domains API
  slug: aikido-security-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/openapi/aikido-security-domains-api-openapi.yml
- filename: aikido-security-issues-api-openapi.yml
  format: yaml
  label: Aikido Security Issues API
  slug: aikido-security-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/openapi/aikido-security-issues-api-openapi.yml
- filename: aikido-security-teams-api-openapi.yml
  format: yaml
  label: Aikido Security Teams API
  slug: aikido-security-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/openapi/aikido-security-teams-api-openapi.yml
- filename: aikido-security-users-api-openapi.yml
  format: yaml
  label: Aikido Security Users API
  slug: aikido-security-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/openapi/aikido-security-users-api-openapi.yml
- filename: aikido-security-webhooks-api-openapi.yml
  format: yaml
  label: Aikido Security Webhooks API
  slug: aikido-security-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/openapi/aikido-security-webhooks-api-openapi.yml
- filename: aikido-security-workspace-api-openapi.yml
  format: yaml
  label: Aikido Security Workspace API
  slug: aikido-security-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/openapi/aikido-security-workspace-api-openapi.yml
- filename: aikido-security-zen-api-openapi.yml
  format: yaml
  label: Aikido Security Zen API
  slug: aikido-security-zen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/openapi/aikido-security-zen-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aikido Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aikido Security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aikido Security
provider_slug: aikido-security
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Bearer access token obtained via POST https://app.aikido.dev/api/oauth/token

    with grant_type=client_credentials and Basic auth (client_id:client_secret).'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/aikido-security-openapi.yml
  type: http
slug: aikido-security-authentication
source_filename: aikido-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aikido-security-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Bearer access token obtained via POST https://app.aikido.dev/api/oauth/token\n    with grant_type=client_credentials and Basic auth (client_id:client_secret).\n  sources:\n  - openapi/aikido-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/authentication/aikido-security-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Pentesting
- API Security
- Application Security
- Cloud Security
- Compliance
- DAST
- Developer-First
- IaC Scanning
- SAST
- SCA
- Secret Detection
---
