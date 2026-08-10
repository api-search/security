---
api_key_in: []
api_specs:
- filename: abnormal-ai-security-mailbox-formerly-known-as-abuse-mailbox-api-openapi.yml
  format: yaml
  label: Abnormal AI AI Security Mailbox (formerly known as Abuse Mailbox) API
  slug: abnormal-ai-security-mailbox-formerly-known-as-abuse-mailbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-ai-security-mailbox-formerly-known-as-abuse-mailbox-api-openapi.yml
- filename: abnormal-audit-logs-api-openapi.yml
  format: yaml
  label: Abnormal AI Audit Logs API
  slug: abnormal-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-audit-logs-api-openapi.yml
- filename: abnormal-cases-api-openapi.yml
  format: yaml
  label: Abnormal AI Cases API
  slug: abnormal-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-cases-api-openapi.yml
- filename: abnormal-dashboard-aggregations-api-openapi.yml
  format: yaml
  label: Abnormal AI Dashboard Aggregations API
  slug: abnormal-dashboard-aggregations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-dashboard-aggregations-api-openapi.yml
- filename: abnormal-detection360-api-openapi.yml
  format: yaml
  label: Abnormal AI Detection360 API
  slug: abnormal-detection360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-detection360-api-openapi.yml
- filename: abnormal-employee-insights-api-openapi.yml
  format: yaml
  label: Abnormal AI Employee Insights API
  slug: abnormal-employee-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-employee-insights-api-openapi.yml
- filename: abnormal-messages-api-openapi.yml
  format: yaml
  label: Abnormal AI Messages API
  slug: abnormal-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-messages-api-openapi.yml
- filename: abnormal-resources-api-openapi.yml
  format: yaml
  label: Abnormal AI Resources API
  slug: abnormal-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-resources-api-openapi.yml
- filename: abnormal-roles-api-openapi.yml
  format: yaml
  label: Abnormal AI Roles API
  slug: abnormal-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-roles-api-openapi.yml
- filename: abnormal-search-and-respond-api-openapi.yml
  format: yaml
  label: Abnormal AI Search and Respond API
  slug: abnormal-search-and-respond-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-search-and-respond-api-openapi.yml
- filename: abnormal-security-settings-api-openapi.yml
  format: yaml
  label: Abnormal AI Security Settings API
  slug: abnormal-security-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-security-settings-api-openapi.yml
- filename: abnormal-spm-api-openapi.yml
  format: yaml
  label: Abnormal AI SPM API
  slug: abnormal-spm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-spm-api-openapi.yml
- filename: abnormal-threats-api-openapi.yml
  format: yaml
  label: Abnormal AI Threats API
  slug: abnormal-threats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-threats-api-openapi.yml
- filename: abnormal-tokens-api-openapi.yml
  format: yaml
  label: Abnormal AI Tokens API
  slug: abnormal-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-tokens-api-openapi.yml
- filename: abnormal-url-rewrite-api-openapi.yml
  format: yaml
  label: Abnormal AI URL Rewrite API
  slug: abnormal-url-rewrite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-url-rewrite-api-openapi.yml
- filename: abnormal-users-api-openapi.yml
  format: yaml
  label: Abnormal AI Users API
  slug: abnormal-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-users-api-openapi.yml
- filename: abnormal-vendors-api-openapi.yml
  format: yaml
  label: Abnormal AI Vendors API
  slug: abnormal-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-vendors-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Abnormal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Abnormal AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Abnormal AI
provider_slug: abnormal
scheme_count: 1
schemes:
- applied: global (root-level security requirement)
  description: A long-lived organization API token generated in the Abnormal Portal under Settings > Integrations > Abnormal REST API. The token grants access to the calling organization's threat, case and posture data; Abnormal instructs customers to store it in an encrypted vault and to contact their account manager if it is compromised.
  format: 'Authorization: Bearer <ACCESS_TOKEN>'
  header: Authorization
  in: header
  name: BearerAuth
  operations_protected: 67
  scheme: bearer
  scopes: []
  sources:
  - openapi/abnormal-client-api-openapi-original.yml
  type: http
slug: abnormal-authentication
source_filename: abnormal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/abnormal-client-api-openapi-original.yml\ndocs: https://abnormalsecurity.my.site.com/knowledgebase/s/article/Abnormal-REST-API-Integration\ntoken_issuance: https://portal.abnormalsecurity.com/home/settings/integrations\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  scopes: none\n  note: >-\n    Single global security requirement — every one of the 67 operations is protected by the\n    same bearer scheme. There is no OAuth, no OIDC, no API-key-in-query, no mutual TLS and no\n    scope model, so scopes/ is intentionally absent for this provider.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <ACCESS_TOKEN>'\n  description: >-\n    A long-lived organization API token generated in the Abnormal Portal under\n    Settings > Integrations > Abnormal REST API. The token grants access to\
  \ the calling\n    organization's threat, case and posture data; Abnormal instructs customers to store it in\n    an encrypted vault and to contact their account manager if it is compromised.\n  scopes: []\n  sources:\n  - openapi/abnormal-client-api-openapi-original.yml\n  applied: global (root-level security requirement)\n  operations_protected: 67\nadditional_controls:\n- name: source IP allowlist\n  required: false\n  configured_at: https://portal.abnormalsecurity.com/home/settings/integrations\n  accepts: [IPv4 address, IPv6 address, CIDR block]\n  failure_mode: >-\n    HTTP 403 (ForbiddenError — \"Access to the resource is forbidden (e.g. IP not in\n    allowlist)\") even when the bearer token is valid. This is the most common cause of 403 on\n    this API and should not be mistaken for a credential problem.\n  description: >-\n    Abnormal presents allowlisting as the second layer of API security, so that a compromised\n    token alone cannot reach the tenant's SOAR data from an\
  \ unauthorized network.\ntoken_management:\n  rotation: manual, in the Abnormal Portal\n  expiry: not published\n  introspection_api: v1_soar_tokens_retrieve (GET /soar/tokens)\n  note: >-\n    The API can enumerate the tenant's SOAR API tokens, but issuance and revocation are\n    Portal-only operations — there is no programmatic token mint or revoke.\nregions:\n  note: >-\n    The token is bound to the tenant's region. US tenants authenticate against\n    https://api.abnormalplatform.com/v1; EU tenants must use\n    https://eu.rest.abnormalsecurity.com/v1.\nverification:\n  test_call: 'curl -H \"Authorization: Bearer <ACCESS_TOKEN>\" https://api.abnormalplatform.com/v1/threats'\n  mock_call: 'curl -H \"Authorization: Bearer <ACCESS_TOKEN>\" -H \"Mock-Data: True\" https://api.abnormalplatform.com/v1/threats'\nfailure_codes:\n  '401': Access token is missing or invalid (UnauthorizedError) — declared on all 67 operations.\n  '403': Token valid but request forbidden, typically source IP\
  \ not allowlisted (ForbiddenError) — declared on 66 operations.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/authentication/abnormal-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Email Security
- Cybersecurity
- Threat Intelligence
- Artificial Intelligence
- SOAR
- Identity
- Compliance
---
