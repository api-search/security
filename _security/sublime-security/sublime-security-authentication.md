---
api_key_in: []
api_specs:
- filename: sublime-security-binexplode-api-openapi.yml
  format: yaml
  label: Sublime Security BinExplode API
  slug: sublime-security-binexplode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-binexplode-api-openapi.yml
- filename: sublime-security-email-bombs-api-openapi.yml
  format: yaml
  label: Sublime Security Email Bombs API
  slug: sublime-security-email-bombs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-email-bombs-api-openapi.yml
- filename: sublime-security-enrichment-api-openapi.yml
  format: yaml
  label: Sublime Security Enrichment API
  slug: sublime-security-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-enrichment-api-openapi.yml
- filename: sublime-security-events-in-the-audit-log-api-openapi.yml
  format: yaml
  label: Sublime Security Events in the audit log API
  slug: sublime-security-events-in-the-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-events-in-the-audit-log-api-openapi.yml
- filename: sublime-security-hunt-jobs-api-openapi.yml
  format: yaml
  label: Sublime Security Hunt Jobs API
  slug: sublime-security-hunt-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-hunt-jobs-api-openapi.yml
- filename: sublime-security-lists-api-openapi.yml
  format: yaml
  label: Sublime Security Lists API
  slug: sublime-security-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-lists-api-openapi.yml
- filename: sublime-security-live-flow-api-openapi.yml
  format: yaml
  label: Sublime Security Live flow API
  slug: sublime-security-live-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-live-flow-api-openapi.yml
- filename: sublime-security-mailboxes-api-openapi.yml
  format: yaml
  label: Sublime Security Mailboxes API
  slug: sublime-security-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-mailboxes-api-openapi.yml
- filename: sublime-security-message-groups-api-openapi.yml
  format: yaml
  label: Sublime Security Message Groups API
  slug: sublime-security-message-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-message-groups-api-openapi.yml
- filename: sublime-security-messages-api-openapi.yml
  format: yaml
  label: Sublime Security Messages API
  slug: sublime-security-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-messages-api-openapi.yml
- filename: sublime-security-organizations-api-openapi.yml
  format: yaml
  label: Sublime Security Organizations API
  slug: sublime-security-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-organizations-api-openapi.yml
- filename: sublime-security-roles-api-openapi.yml
  format: yaml
  label: Sublime Security Roles API
  slug: sublime-security-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-roles-api-openapi.yml
- filename: sublime-security-rules-api-openapi.yml
  format: yaml
  label: Sublime Security Rules API
  slug: sublime-security-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-rules-api-openapi.yml
- filename: sublime-security-scim-api-openapi.yml
  format: yaml
  label: Sublime Security SCIM API
  slug: sublime-security-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-scim-api-openapi.yml
- filename: sublime-security-tasks-api-openapi.yml
  format: yaml
  label: Sublime Security Tasks API
  slug: sublime-security-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-tasks-api-openapi.yml
- filename: sublime-security-user-reports-api-openapi.yml
  format: yaml
  label: Sublime Security User Reports API
  slug: sublime-security-user-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-user-reports-api-openapi.yml
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
