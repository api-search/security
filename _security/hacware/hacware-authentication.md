---
api_key_in: []
api_specs:
- filename: hacware-admin-api-openapi.yml
  format: yaml
  label: Hacware Admin API
  slug: hacware-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-admin-api-openapi.yml
- filename: hacware-compliance-api-openapi.yml
  format: yaml
  label: Hacware Compliance API
  slug: hacware-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-compliance-api-openapi.yml
- filename: hacware-compliance-tenant-api-openapi.yml
  format: yaml
  label: Hacware Compliance-Tenant API
  slug: hacware-compliance-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-compliance-tenant-api-openapi.yml
- filename: hacware-customer-api-openapi.yml
  format: yaml
  label: Hacware Customer API
  slug: hacware-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-customer-api-openapi.yml
- filename: hacware-email-tenant-api-openapi.yml
  format: yaml
  label: Hacware Email-Tenant API
  slug: hacware-email-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-email-tenant-api-openapi.yml
- filename: hacware-group-api-openapi.yml
  format: yaml
  label: Hacware Group API
  slug: hacware-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-group-api-openapi.yml
- filename: hacware-multi-tenant-api-openapi.yml
  format: yaml
  label: Hacware Multi-Tenant API
  slug: hacware-multi-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-multi-tenant-api-openapi.yml
- filename: hacware-phishing-api-openapi.yml
  format: yaml
  label: Hacware Phishing API
  slug: hacware-phishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-phishing-api-openapi.yml
- filename: hacware-report-api-openapi.yml
  format: yaml
  label: Hacware Report API
  slug: hacware-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-report-api-openapi.yml
- filename: hacware-training-api-openapi.yml
  format: yaml
  label: Hacware Training API
  slug: hacware-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-training-api-openapi.yml
- filename: hacware-user-api-openapi.yml
  format: yaml
  label: Hacware User API
  slug: hacware-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hacware Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hacware secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hacware
provider_slug: hacware
scheme_count: 1
schemes:
- description: Bearer access token obtained from POST /api/v1/auth/ (exchange appid + secret key). Tokens expire ~1 hour after issue; use the refresh token to renew.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hacware-openapi.yml
  type: http
slug: hacware-authentication
source_filename: hacware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hacware-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer access token obtained from POST /api/v1/auth/ (exchange appid + secret\n    key). Tokens expire ~1 hour after issue; use the refresh token to renew.\n  sources:\n  - openapi/hacware-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/authentication/hacware-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Security Awareness
- Phishing
- Training
- Compliance
- Email Security
- Artificial Intelligence
---
