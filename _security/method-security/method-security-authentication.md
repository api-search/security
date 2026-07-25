---
api_key_in: []
api_specs:
- filename: method-security-audit-api-openapi.yml
  format: yaml
  label: Method Security audit API
  slug: method-security-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-audit-api-openapi.yml
- filename: method-security-auth-api-openapi.yml
  format: yaml
  label: Method Security auth API
  slug: method-security-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-auth-api-openapi.yml
- filename: method-security-blueprints-api-openapi.yml
  format: yaml
  label: Method Security blueprints API
  slug: method-security-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-blueprints-api-openapi.yml
- filename: method-security-environments-api-openapi.yml
  format: yaml
  label: Method Security environments API
  slug: method-security-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-environments-api-openapi.yml
- filename: method-security-issues-api-openapi.yml
  format: yaml
  label: Method Security issues API
  slug: method-security-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-issues-api-openapi.yml
- filename: method-security-reports-api-openapi.yml
  format: yaml
  label: Method Security reports API
  slug: method-security-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-reports-api-openapi.yml
- filename: method-security-signals-api-openapi.yml
  format: yaml
  label: Method Security signals API
  slug: method-security-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-signals-api-openapi.yml
- filename: method-security-skills-api-openapi.yml
  format: yaml
  label: Method Security skills API
  slug: method-security-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-skills-api-openapi.yml
- filename: method-security-system-api-openapi.yml
  format: yaml
  label: Method Security system API
  slug: method-security-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-system-api-openapi.yml
- filename: method-security-targets-api-openapi.yml
  format: yaml
  label: Method Security targets API
  slug: method-security-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-targets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Method Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Method Security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Method Security
provider_slug: method-security
scheme_count: 1
schemes:
- name: client-credentials
  scheme: bearer
  sources:
  - openapi/method-security-openapi-original.yml
  type: http
slug: method-security-authentication
source_filename: method-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/method-security-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: client-credentials\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/method-security-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/authentication/method-security-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Offensive Security
- Exposure Management
- Attack Surface Management
- Vulnerability Management
- Red Team
- AI Agents
- Government
---
