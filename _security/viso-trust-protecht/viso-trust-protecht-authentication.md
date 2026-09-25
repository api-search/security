---
anonymous_access: false
api_key_in: []
api_specs:
- filename: viso-trust-protecht-client-api-assessment-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust (Protecht) client-api-assessment-rest-resource API
  slug: viso-trust-protecht-client-api-assessment-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust-protecht/refs/heads/main/openapi/viso-trust-protecht-client-api-assessment-rest-resource-api-openapi.yml
- filename: viso-trust-protecht-client-api-audit-log-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust (Protecht) client-api-audit-log-rest-resource API
  slug: viso-trust-protecht-client-api-audit-log-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust-protecht/refs/heads/main/openapi/viso-trust-protecht-client-api-audit-log-rest-resource-api-openapi.yml
- filename: viso-trust-protecht-client-api-chat-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust (Protecht) Client API Chat Rest Resource API
  slug: viso-trust-protecht-client-api-chat-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust-protecht/refs/heads/main/openapi/viso-trust-protecht-client-api-chat-rest-resource-api-openapi.yml
- filename: viso-trust-protecht-client-api-context-type-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust (Protecht) Client API Context Type Rest Resource API
  slug: viso-trust-protecht-client-api-context-type-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust-protecht/refs/heads/main/openapi/viso-trust-protecht-client-api-context-type-rest-resource-api-openapi.yml
- filename: viso-trust-protecht-client-api-data-type-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust (Protecht) Client API Data Type Rest Resource API
  slug: viso-trust-protecht-client-api-data-type-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust-protecht/refs/heads/main/openapi/viso-trust-protecht-client-api-data-type-rest-resource-api-openapi.yml
- filename: viso-trust-protecht-client-api-external-intelligence-report-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust (Protecht) Client API External Intelligence Report Rest Resource API
  slug: viso-trust-protecht-client-api-external-intelligence-report-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust-protecht/refs/heads/main/openapi/viso-trust-protecht-client-api-external-intelligence-report-rest-resource-api-openapi.yml
- filename: viso-trust-protecht-client-api-questionnaire-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust (Protecht) Client API Questionnaire Rest Resource API
  slug: viso-trust-protecht-client-api-questionnaire-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust-protecht/refs/heads/main/openapi/viso-trust-protecht-client-api-questionnaire-rest-resource-api-openapi.yml
- filename: viso-trust-protecht-client-api-relationship-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust (Protecht) Client API Relationship Rest Resource API
  slug: viso-trust-protecht-client-api-relationship-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust-protecht/refs/heads/main/openapi/viso-trust-protecht-client-api-relationship-rest-resource-api-openapi.yml
- filename: viso-trust-protecht-client-api-user-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust (Protecht) Client API User Rest Resource API
  slug: viso-trust-protecht-client-api-user-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust-protecht/refs/heads/main/openapi/viso-trust-protecht-client-api-user-rest-resource-api-openapi.yml
- filename: viso-trust-protecht-client-api-vendor-directory-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust (Protecht) Client API Vendor Directory Rest Resource API
  slug: viso-trust-protecht-client-api-vendor-directory-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust-protecht/refs/heads/main/openapi/viso-trust-protecht-client-api-vendor-directory-rest-resource-api-openapi.yml
- filename: viso-trust-protecht-client-api-vendor-risk-summary-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust (Protecht) Client API Vendor Risk Summary Rest Resource API
  slug: viso-trust-protecht-client-api-vendor-risk-summary-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust-protecht/refs/heads/main/openapi/viso-trust-protecht-client-api-vendor-risk-summary-rest-resource-api-openapi.yml
- filename: viso-trust-protecht-client-api-webhook-rest-resource-api-openapi.yml
  format: yaml
  label: VISO Trust (Protecht) Client API Webhook Rest Resource API
  slug: viso-trust-protecht-client-api-webhook-rest-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust-protecht/refs/heads/main/openapi/viso-trust-protecht-client-api-webhook-rest-resource-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Viso Trust Protecht Authentication
name_suffix: Authentication
oauth_flows: []
overview: VISO Trust (Protecht) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VISO Trust (Protecht)
provider_slug: viso-trust-protecht
scheme_count: 1
schemes:
- description: API token generated from your VISO TRUST user profile. Send it in the `Authorization` header as `Bearer <token>`. The same token authenticates the hosted MCP server at https://mcp.visotrust.com/sse.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/viso-trust-protecht-openapi-original.json
  type: http
slug: viso-trust-protecht-authentication
source_filename: viso-trust-protecht-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/viso-trust-protecht-openapi-original.json\ndocs: https://docs.visotrust.com/api-reference/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\nbase_url: https://app.visotrust.com\ntoken_model:\n  source: Generated once from an Admin or Program Manager user profile, or a dedicated service account.\n  storage: Shown only at generation; store in a secrets manager (not retrievable later).\n  permissions: Program-level access required; Contributor/Viewer tokens are rejected.\n  same_token_for_mcp: true\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    API token generated from your VISO TRUST user profile. Send it in the\n    `Authorization` header as `Bearer <token>`. The same token authenticates the\n    hosted MCP server at https://mcp.visotrust.com/sse.\n  sources:\n  - openapi/viso-trust-protecht-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viso-trust-protecht/refs/heads/main/authentication/viso-trust-protecht-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Third-Party Risk Management
- GRC
- Cybersecurity
- Compliance
- Artificial Intelligence
---
