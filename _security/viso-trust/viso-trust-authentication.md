---
api_key_in: []
api_specs:
- filename: viso-trust-client-api-assessment-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust client-api-assessment-rest-resource API
  slug: viso-trust-client-api-assessment-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/openapi/viso-trust-client-api-assessment-rest-resource-api-openapi.yml
- filename: viso-trust-client-api-audit-log-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust client-api-audit-log-rest-resource API
  slug: viso-trust-client-api-audit-log-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/openapi/viso-trust-client-api-audit-log-rest-resource-api-openapi.yml
- filename: viso-trust-client-api-chat-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust client-api-chat-rest-resource API
  slug: viso-trust-client-api-chat-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/openapi/viso-trust-client-api-chat-rest-resource-api-openapi.yml
- filename: viso-trust-client-api-context-type-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust client-api-context-type-rest-resource API
  slug: viso-trust-client-api-context-type-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/openapi/viso-trust-client-api-context-type-rest-resource-api-openapi.yml
- filename: viso-trust-client-api-data-type-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust client-api-data-type-rest-resource API
  slug: viso-trust-client-api-data-type-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/openapi/viso-trust-client-api-data-type-rest-resource-api-openapi.yml
- filename: viso-trust-client-api-external-intelligence-report-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust client-api-external-intelligence-report-rest-resource API
  slug: viso-trust-client-api-external-intelligence-report-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/openapi/viso-trust-client-api-external-intelligence-report-rest-resource-api-openapi.yml
- filename: viso-trust-client-api-questionnaire-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust client-api-questionnaire-rest-resource API
  slug: viso-trust-client-api-questionnaire-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/openapi/viso-trust-client-api-questionnaire-rest-resource-api-openapi.yml
- filename: viso-trust-client-api-relationship-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust client-api-relationship-rest-resource API
  slug: viso-trust-client-api-relationship-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/openapi/viso-trust-client-api-relationship-rest-resource-api-openapi.yml
- filename: viso-trust-client-api-user-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust client-api-user-rest-resource API
  slug: viso-trust-client-api-user-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/openapi/viso-trust-client-api-user-rest-resource-api-openapi.yml
- filename: viso-trust-client-api-vendor-directory-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust client-api-vendor-directory-rest-resource API
  slug: viso-trust-client-api-vendor-directory-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/openapi/viso-trust-client-api-vendor-directory-rest-resource-api-openapi.yml
- filename: viso-trust-client-api-vendor-risk-summary-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust client-api-vendor-risk-summary-rest-resource API
  slug: viso-trust-client-api-vendor-risk-summary-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/openapi/viso-trust-client-api-vendor-risk-summary-rest-resource-api-openapi.yml
- filename: viso-trust-client-api-webhook-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust client-api-webhook-rest-resource API
  slug: viso-trust-client-api-webhook-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/openapi/viso-trust-client-api-webhook-rest-resource-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Viso Trust Authentication
name_suffix: Authentication
oauth_flows: []
overview: VISO Trust secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VISO Trust
provider_slug: viso-trust
scheme_count: 1
schemes:
- description: API token generated from your VISO TRUST user profile. Send it in the `Authorization` header as `Bearer <token>`.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/viso-trust-openapi-original.json
  type: http
slug: viso-trust-authentication
source_filename: viso-trust-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/viso-trust-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API token generated from your VISO TRUST user profile. Send it in the `Authorization`\n    header as `Bearer <token>`.\n  sources:\n  - openapi/viso-trust-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/authentication/viso-trust-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Third Party Risk Management
- TPRM
- Vendor Risk
- Risk Management
- Compliance
- Cybersecurity
- Artificial Intelligence
---
