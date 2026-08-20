---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cast Corporation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cast Corporation secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cast Corporation
provider_slug: cast-corporation
scheme_count: 2
schemes:
- applies_to:
  - https://cast.app/designer/{org_slug}/api
  description: 'The Cast Analytics API takes the raw API key as the value of the Authorization header, with no "Bearer" prefix. Documented example - "Authorization: your_api_key".'
  in: header
  issuance: Requested by emailing support@cast.app. Not self-serve.
  name: analytics-api-key
  parameter_name: Authorization
  scheme_format: raw-key
  source: https://school.cast.app/cast-api/
  type: apiKey
- applies_to:
  - https://cast.app/designer/api/v1
  description: 'The In-app Delivery permalink endpoint takes a bearer token - "Authorization: Bearer <api_key>".'
  exposure: Cast documents this key as safe to expose in client-side embed code - it can only resolve a permalink for a contact in a published campaign. It is still a credential; the analytics key is not client-safe.
  in: header
  issuance: Self-serve. Generated (and regenerated) from Campaigns & Analytics -> In-app Delivery in the Cast Designer. Regeneration immediately invalidates the prior key.
  name: inapp-delivery-bearer
  parameter_name: Authorization
  scheme: bearer
  source: https://school.cast.app/projects/campaigns-and-analytics/in-app-delivery/
  type: http
slug: cast-corporation-authentication
source_filename: cast-corporation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://school.cast.app/cast-api/\ndocs:\n- https://school.cast.app/cast-api/\n- https://school.cast.app/projects/campaigns-and-analytics/in-app-delivery/\n- https://school.cast.app/sso-setup-guide/\nnote: >-\n  Cast publishes no OpenAPI, so this profile is transcribed from the two published API\n  reference pages rather than derived from securitySchemes. Two distinct API keys exist\n  and they are NOT interchangeable: the Analytics API key is issued by Cast support on\n  request, the In-app Delivery key is self-serve from the Cast Designer UI.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mtls: false\nschemes:\n- name: analytics-api-key\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  scheme_format: raw-key\n  description: >-\n    The Cast Analytics API takes the raw API key as the value of the Authorization\n    header, with no\
  \ \"Bearer\" prefix. Documented example - \"Authorization: your_api_key\".\n  issuance: >-\n    Requested by emailing support@cast.app. Not self-serve.\n  applies_to:\n  - https://cast.app/designer/{org_slug}/api\n  source: https://school.cast.app/cast-api/\n- name: inapp-delivery-bearer\n  type: http\n  scheme: bearer\n  in: header\n  parameter_name: Authorization\n  description: >-\n    The In-app Delivery permalink endpoint takes a bearer token -\n    \"Authorization: Bearer <api_key>\".\n  issuance: >-\n    Self-serve. Generated (and regenerated) from Campaigns & Analytics -> In-app\n    Delivery in the Cast Designer. Regeneration immediately invalidates the prior key.\n  exposure: >-\n    Cast documents this key as safe to expose in client-side embed code - it can only\n    resolve a permalink for a contact in a published campaign. It is still a credential;\n    the analytics key is not client-safe.\n  applies_to:\n  - https://cast.app/designer/api/v1\n  source: https://school.cast.app/projects/campaigns-and-analytics/in-app-delivery/\n\
  tenancy:\n  org_slug_required: true\n  note: >-\n    The Analytics API path embeds the tenant - https://cast.app/designer/{org_slug}/api -\n    so the key is scoped to one organization. org_slug, cast_id (project) and\n    generation_id (campaign) are read off the Designer URL, not from a discovery endpoint.\nplatform_sso:\n  protocol: SAML 2.0\n  scope: Cast Designer console sign-in (not API authentication)\n  identity_providers:\n  - Okta\n  - Microsoft Entra ID\n  - Google Workspace\n  docs: https://school.cast.app/sso-setup-guide/\nx-evidence:\n  fetched: '2026-08-13'\n  checks:\n  - url: https://cast.app/designer/api/v1/permalink\n    method: POST\n    unauthenticated_status: 401\n    finding: >-\n      Endpoint is live and rejects unauthenticated requests, confirming the documented\n      bearer scheme is enforced.\n  - url: https://school.cast.app/llms-full.txt\n    status: 200\n    finding: Full documentation text, including both API reference pages, is machine-readable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cast-corporation/refs/heads/main/authentication/cast-corporation-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Customer Success
- Artificial Intelligence
- AI Agents
- Revenue Operations
- Software-as-a-Service
- Automation
- Post-Sales
- Analytics
- Webhook
- Embeddable
---
