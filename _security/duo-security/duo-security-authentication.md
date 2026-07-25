---
api_key_in: []
api_specs:
- filename: duo-security-bulk-api-openapi.yml
  format: yaml
  label: Duo Security Bulk API
  slug: duo-security-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duo-security/refs/heads/main/openapi/duo-security-bulk-api-openapi.yml
- filename: duo-security-bypass-codes-api-openapi.yml
  format: yaml
  label: Duo Security Bypass Codes API
  slug: duo-security-bypass-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duo-security/refs/heads/main/openapi/duo-security-bypass-codes-api-openapi.yml
- filename: duo-security-groups-api-openapi.yml
  format: yaml
  label: Duo Security Groups API
  slug: duo-security-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duo-security/refs/heads/main/openapi/duo-security-groups-api-openapi.yml
- filename: duo-security-phones-api-openapi.yml
  format: yaml
  label: Duo Security Phones API
  slug: duo-security-phones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duo-security/refs/heads/main/openapi/duo-security-phones-api-openapi.yml
- filename: duo-security-tokens-api-openapi.yml
  format: yaml
  label: Duo Security Tokens API
  slug: duo-security-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duo-security/refs/heads/main/openapi/duo-security-tokens-api-openapi.yml
- filename: duo-security-users-api-openapi.yml
  format: yaml
  label: Duo Security Users API
  slug: duo-security-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duo-security/refs/heads/main/openapi/duo-security-users-api-openapi.yml
- filename: duo-security-webauthn-api-openapi.yml
  format: yaml
  label: Duo Security WebAuthn API
  slug: duo-security-webauthn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duo-security/refs/heads/main/openapi/duo-security-webauthn-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Duo Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Duo Security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Duo Security
provider_slug: duo-security
scheme_count: 1
schemes:
- description: HTTP Basic with HMAC-SHA1 signed credentials (integration key as user, signed signature as password).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/duo-admin-api-openapi.yml
  type: http
slug: duo-security-authentication
source_filename: duo-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/duo-admin-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with HMAC-SHA1 signed credentials (integration key as user, signed\n    signature as password).\n  sources:\n  - openapi/duo-admin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duo-security/refs/heads/main/authentication/duo-security-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- MFA
- Zero Trust
- Identity
---
