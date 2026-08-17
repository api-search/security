---
api_key_in:
- header
- body
api_specs:
- filename: smtp2go-email-api-openapi.yml
  format: yaml
  label: SMTP2GO Email API
  slug: smtp2go-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-email-api-openapi.yml
- filename: smtp2go-activity-api-openapi.yml
  format: yaml
  label: SMTP2GO Activity API
  slug: smtp2go-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-activity-api-openapi.yml
- filename: smtp2go-api-keys-api-openapi.yml
  format: yaml
  label: SMTP2GO API Keys API
  slug: smtp2go-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-api-keys-api-openapi.yml
- filename: smtp2go-domains-api-openapi.yml
  format: yaml
  label: SMTP2GO Domains API
  slug: smtp2go-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-domains-api-openapi.yml
- filename: smtp2go-sms-api-openapi.yml
  format: yaml
  label: SMTP2GO SMS API
  slug: smtp2go-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-sms-api-openapi.yml
- filename: smtp2go-smtp-users-api-openapi.yml
  format: yaml
  label: SMTP2GO SMTP Users API
  slug: smtp2go-smtp-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-smtp-users-api-openapi.yml
- filename: smtp2go-stats-api-openapi.yml
  format: yaml
  label: SMTP2GO Stats API
  slug: smtp2go-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-stats-api-openapi.yml
- filename: smtp2go-subaccounts-api-openapi.yml
  format: yaml
  label: SMTP2GO Subaccounts API
  slug: smtp2go-subaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-subaccounts-api-openapi.yml
- filename: smtp2go-suppressions-api-openapi.yml
  format: yaml
  label: SMTP2GO Suppressions API
  slug: smtp2go-suppressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-suppressions-api-openapi.yml
- filename: smtp2go-templates-api-openapi.yml
  format: yaml
  label: SMTP2GO Templates API
  slug: smtp2go-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-templates-api-openapi.yml
- filename: smtp2go-webhooks-api-openapi.yml
  format: yaml
  label: SMTP2GO Webhooks API
  slug: smtp2go-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Smtp2Go Authentication
name_suffix: Authentication
oauth_flows: []
overview: SMTP2GO secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SMTP2GO
provider_slug: smtp2go
scheme_count: 2
schemes:
- applied_to_operations: 73
  description: The provider's own contract declares exactly one security scheme, applied globally to all 73 operations. The docs show a ${SMTP2GO_API_KEY} environment-variable default.
  in: header
  name: sec0
  parameter: X-Smtp2go-Api-Key
  sources:
  - openapi/_original/smtp2go-openapi-original.yml
  type: apiKey
- description: 'Documented alternate: the same key may be supplied as an api_key field inside the JSON request body instead of the header. Not declared as a securityScheme in the OpenAPI — only the header form is machine-readable.'
  in: body
  name: ApiKeyBody
  parameter: api_key
  sources:
  - https://developers.smtp2go.com/reference/authentication
  type: apiKey
slug: smtp2go-authentication
source_filename: smtp2go-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/smtp2go-openapi-original.yml\ndocs: https://developers.smtp2go.com/reference/authentication\ndocs_secondary: https://developers.smtp2go.com/docs/getting-started\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - body\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: X-Smtp2go-Api-Key\n  description: >-\n    The provider's own contract declares exactly one security scheme, applied\n    globally to all 73 operations. The docs show a ${SMTP2GO_API_KEY}\n    environment-variable default.\n  sources:\n  - openapi/_original/smtp2go-openapi-original.yml\n  applied_to_operations: 73\n- name: ApiKeyBody\n  type: apiKey\n  in: body\n  parameter: api_key\n  description: >-\n    Documented alternate: the same key may be supplied as an api_key field\n    inside the JSON request body instead of the header. Not declared as a\n\
  \    securityScheme in the OpenAPI — only the header form is machine-readable.\n  sources:\n  - https://developers.smtp2go.com/reference/authentication\nkey:\n  format: '\"api-\" prefix followed by 32 generated characters'\n  management_url: https://app.smtp2go.com/sending/apikeys/\n  console_path: Sending > API Keys\n  rotation: 'Keys are added, edited, patched and removed over the API itself (/api_keys/*); the value is masked on edit/view responses since 2026-06-22.'\n  per_key_settings:\n    - Description / friendly identifier\n    - Rate limit (defaults to unlimited)\n    - Endpoint permission list — which endpoints this key may call\n    - Unsubscribe footer toggle\n    - Open tracking toggle\n    - Click tracking toggle\n    - Disable, or set to Sandbox Mode\n    - Email archiving toggle\n    - BCC address for email auditing\n    - Bounce notifications toggle\nauthorization:\n  model: per-key endpoint permissions\n  introspection:\n    operation: view-api-key-permissions\n    path:\
  \ /api_keys/permissions\n    note: Returns the endpoint list the calling key may use; callable by every key.\n  failure:\n    http_status: 400\n    error_code: E_ApiResponseCodes.ENDPOINT_PERMISSION_DENIED\n    note: A permission failure is a 400 carrying an error_code, not a 403.\n  escalation_rule: >-\n    Since 2026-05-29, adding or removing endpoints on a key without the\n    appropriate permissions on the authenticating key, or beyond the target\n    key's existing permission set, is refused.\n  scopes: null\n  scopes_note: >-\n    There is no OAuth scope surface. Authorization is an explicit per-key list of\n    API endpoints, so scopes/ is intentionally not emitted for this provider.\nmissing_auth:\n  http_status: 401\n  note: 'Failure to supply a key, or supplying an invalid or disabled key, returns 401 Unauthorized.'\nother_credentials:\n  - {kind: SMTP user, note: 'Username/password for the SMTP relay, managed via /users/smtp/*. Separate from API keys.'}\n  - {kind: IP authentication,\
  \ note: 'Send without a credential from an authenticated IP, managed via /ip_auth/*.'}\n  - {kind: IP allow list, note: 'Account-level restriction of where SMTP or API traffic may originate, managed via /ip_allow_list/*; a type parameter selects the SMTP or API list.'}\noauth:\n  supported: false\n  evidence:\n    - {url: 'https://api.smtp2go.com/.well-known/oauth-authorization-server', status: 404}\n    - {url: 'https://developers.smtp2go.com/.well-known/oauth-authorization-server', status: 404}\n    - {url: 'https://api.smtp2go.com/.well-known/openid-configuration', status: 404}\nmcp_authentication:\n  endpoint: https://developers.smtp2go.com/mcp\n  scheme: 'Same X-Smtp2go-Api-Key header; no OAuth challenge, no /.well-known/oauth-protected-resource.'\n  anonymous_surface: 'Documentation discovery tools (list-endpoints, search-endpoints, get-endpoint, get-server-variables) answer without a key; execute-request requires one.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/authentication/smtp2go-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Email
- Email Delivery
- Transactional Email
- SMTP
- SMS
- Email API
- Deliverability
- Webhooks
- Messaging
- Communications
- MCP
- Agent Skills
---
