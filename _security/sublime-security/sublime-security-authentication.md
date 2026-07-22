---
api_key_in: []
api_specs:
- filename: sublime-security-platform-openapi.json
  format: json
  label: Sublime Platform API
  slug: sublime-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-platform-openapi.json
- filename: sublime-security-multitenancy-openapi.json
  format: json
  label: Sublime Multi-Tenancy API (Beta)
  slug: sublime-multi-tenancy-api-beta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-multitenancy-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sublime Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sublime Security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sublime Security
provider_slug: sublime-security
scheme_count: 1
schemes:
- format: Bearer <API key>
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sublime-security-multitenancy-openapi.json
  - openapi/sublime-security-platform-openapi.json
  type: http
slug: sublime-security-authentication
source_filename: sublime-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sublime-security-multitenancy-openapi.json, openapi/sublime-security-platform-openapi.json\ndocs: https://docs.sublime.security/reference/authentication.md\nsummary:\n  types:\n  - http\n  scheme: api-key-bearer\n  detail: >-\n    Static API keys generated under Automate > API on the Sublime dashboard and sent as\n    an HTTP Bearer token (`Authorization: Bearer <API key>`). The key is displayed only\n    once at creation. No OAuth2 flows or scopes; RBAC governs what each key can do.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <API key>'\n  sources:\n  - openapi/sublime-security-multitenancy-openapi.json\n  - openapi/sublime-security-platform-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/authentication/sublime-security-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Email Security
- Phishing
- Detection as Code
- Threat Detection
- Cloud Email Security
- SCIM
---
