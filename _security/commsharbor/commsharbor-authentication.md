---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: CommsHarbor API
  slug: commsharbor-api
  spec_type: OpenAPI
  url: https://commsharbor.com/openapi.json
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
- Agent-native
- MCP
- Web3 payments
- x402
---
