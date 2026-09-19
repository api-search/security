---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commsharbor-apis-json-api-openapi.yml
  format: yaml
  label: CommsHarbor Apis.json API
  slug: commsharbor-apis-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-apis-json-api-openapi.yml
- filename: commsharbor-auth-api-openapi.yml
  format: yaml
  label: CommsHarbor Auth API
  slug: commsharbor-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-auth-api-openapi.yml
- filename: commsharbor-aws-api-openapi.yml
  format: yaml
  label: CommsHarbor Aws API
  slug: commsharbor-aws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-aws-api-openapi.yml
- filename: commsharbor-billing-api-openapi.yml
  format: yaml
  label: CommsHarbor Billing API
  slug: commsharbor-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-billing-api-openapi.yml
- filename: commsharbor-commsharbor-api-openapi.yml
  format: yaml
  label: CommsHarbor Comms Harbor API
  slug: commsharbor-commsharbor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-commsharbor-api-openapi.yml
- filename: commsharbor-context-api-openapi.yml
  format: yaml
  label: CommsHarbor Context API
  slug: commsharbor-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-context-api-openapi.yml
- filename: commsharbor-credito-api-openapi.yml
  format: yaml
  label: CommsHarbor Credito API
  slug: commsharbor-credito-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-credito-api-openapi.yml
- filename: commsharbor-health-api-openapi.yml
  format: yaml
  label: CommsHarbor Health API
  slug: commsharbor-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-health-api-openapi.yml
- filename: commsharbor-invitations-api-openapi.yml
  format: yaml
  label: CommsHarbor Invitations API
  slug: commsharbor-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-invitations-api-openapi.yml
- filename: commsharbor-mcp-api-openapi.yml
  format: yaml
  label: CommsHarbor MCP API
  slug: commsharbor-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-mcp-api-openapi.yml
- filename: commsharbor-me-api-openapi.yml
  format: yaml
  label: CommsHarbor Me API
  slug: commsharbor-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-me-api-openapi.yml
- filename: commsharbor-messages-api-openapi.yml
  format: yaml
  label: CommsHarbor Messages API
  slug: commsharbor-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-messages-api-openapi.yml
- filename: commsharbor-metrics-api-openapi.yml
  format: yaml
  label: CommsHarbor Metrics API
  slug: commsharbor-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-metrics-api-openapi.yml
- filename: commsharbor-okf-api-openapi.yml
  format: yaml
  label: CommsHarbor Okf API
  slug: commsharbor-okf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-okf-api-openapi.yml
- filename: commsharbor-organizations-api-openapi.yml
  format: yaml
  label: CommsHarbor Organizations API
  slug: commsharbor-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-organizations-api-openapi.yml
- filename: commsharbor-platform-api-openapi.yml
  format: yaml
  label: CommsHarbor Platform API
  slug: commsharbor-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-platform-api-openapi.yml
- filename: commsharbor-preferences-api-openapi.yml
  format: yaml
  label: CommsHarbor Preferences API
  slug: commsharbor-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-preferences-api-openapi.yml
- filename: commsharbor-well-known-api-openapi.yml
  format: yaml
  label: CommsHarbor .well Known API
  slug: commsharbor-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/openapi/commsharbor-well-known-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Commsharbor Authentication
name_suffix: Authentication
oauth_flows: []
overview: CommsHarbor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CommsHarbor
provider_slug: commsharbor
scheme_count: 1
schemes:
- description: Human session or scoped organization API key. Organization identity remains explicit.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/commsharbor-openapi.json
  type: http
slug: commsharbor-authentication
source_filename: commsharbor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/commsharbor-openapi.json\ndocs: https://commsharbor.com/api/\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Human session or scoped organization API key. Organization identity remains explicit.\n  sources:\n  - openapi/commsharbor-openapi.json\nauth_modes:\n  note: >-\n    The machine-readable API index (GET /api/, 200) documents eleven per-endpoint auth modes beyond\n    the single bearer scheme the OpenAPI declares. API keys are organization-scoped with named\n    permissions; keys cannot manage credentials or membership, and platform access is a separate\n    explicit grant never implied by tenant ownership. Keys and webhook secrets are revealed exactly\n    once at creation; revocation is immediate.\n  modes:\n    - name: none\n      detail: Public endpoint. No tenant data is returned.\n    - name: session\n      detail: Bearer session or secure session\
  \ cookie. No organization is implied.\n    - name: organization\n      detail: Session plus X-Organization-Id membership, or a scoped API key that determines the organization (and rejects a conflicting header).\n    - name: organization_template_write\n      detail: Active organization identity with template:write permission.\n    - name: organization_messages_send\n      detail: Active organization identity with messages:send permission. Idempotency-Key is mandatory.\n    - name: organization_campaign_write\n      detail: Active organization identity with campaign:write permission. Campaign launches require Idempotency-Key.\n    - name: organization_admin\n      detail: Human organization member with the required role; API keys cannot manage credentials or membership.\n    - name: platform_admin\n      detail: Session with an explicit platform_roles grant. Tenant ownership does not grant platform access.\n    - name: aws_sns\n      detail: Amazon SNS signature, regional certificate URL\
  \ and the exact configured TopicArn. Never accepts a user credential.\n    - name: preference_capability\n      detail: Signed, expiring capability scoped to one organization and contact. No login required; no email address embedded in the token.\n    - name: credito\n      detail: 'Prepaid credit token in Authorization: Bearer cred_... (or the X-Credito header). Not an account: a bearer of balance.'\n  permissions:\n    - messages:send\n    - template:write\n    - campaign:write\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commsharbor/refs/heads/main/authentication/commsharbor-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Transactional Email
- Email Marketing
- Communications
- Messaging
- Deliverability
- CRM
- Multi-tenant SaaS
- agent-native
- MCP
- Web3 payments
- x402
---
