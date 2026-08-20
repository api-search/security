---
api_key_in:
- header
api_specs:
- filename: creatoriq-publishers-openapi.yml
  format: yaml
  label: CreatorIQ CRM Publishers API
  slug: creatoriq-crm-publishers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-publishers-openapi.yml
- filename: creatoriq-v2-publishers-openapi.yml
  format: yaml
  label: CreatorIQ CRM Publishers API V2
  slug: creatoriq-crm-publishers-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-v2-publishers-openapi.yml
- filename: creatoriq-campaigns-openapi.yml
  format: yaml
  label: CreatorIQ Campaign APIs
  slug: creatoriq-campaign-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-campaigns-openapi.yml
- filename: creatoriq-v2-campaigns-openapi.yml
  format: yaml
  label: CreatorIQ CRM Campaigns API V2
  slug: creatoriq-crm-campaigns-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-v2-campaigns-openapi.yml
- filename: creatoriq-reports-openapi.yml
  format: yaml
  label: CreatorIQ Reporting APIs
  slug: creatoriq-reporting-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-reports-openapi.yml
- filename: creatoriq-socials-openapi.yml
  format: yaml
  label: CreatorIQ Social Account APIs
  slug: creatoriq-social-account-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-socials-openapi.yml
- filename: creatoriq-lists-openapi.yml
  format: yaml
  label: CreatorIQ CRM Lists API
  slug: creatoriq-crm-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-lists-openapi.yml
- filename: creatoriq-onesheets-openapi.yml
  format: yaml
  label: CreatorIQ CRM Onesheets API
  slug: creatoriq-crm-onesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-onesheets-openapi.yml
- filename: creatoriq-notes-openapi.yml
  format: yaml
  label: CreatorIQ CRM Notes API
  slug: creatoriq-crm-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-notes-openapi.yml
- filename: creatoriq-v1-divisions-openapi.yml
  format: yaml
  label: CreatorIQ Divisions APIs
  slug: creatoriq-divisions-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-v1-divisions-openapi.yml
- filename: creatoriq-ecommerce-openapi.yml
  format: yaml
  label: CreatorIQ Ecommerce APIs
  slug: creatoriq-ecommerce-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-ecommerce-openapi.yml
- filename: creatoriq-link-tracking-openapi.yml
  format: yaml
  label: CreatorIQ CRM LinkTracking API
  slug: creatoriq-crm-linktracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-link-tracking-openapi.yml
- filename: creatoriq-conversion-metrics-openapi.yml
  format: yaml
  label: CreatorIQ Conversion Metrics API
  slug: creatoriq-conversion-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-conversion-metrics-openapi.yml
- filename: creatoriq-brand-safety-openapi.yml
  format: yaml
  label: CreatorIQ SafeIQ Brand Safety API
  slug: creatoriq-safeiq-brand-safety-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-brand-safety-openapi.yml
- filename: creatoriq-brand-safety-draft-openapi.yml
  format: yaml
  label: CreatorIQ Brand Safety (draft)
  slug: creatoriq-brand-safety-draft
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-brand-safety-draft-openapi.yml
- filename: creatoriq-payments-openapi.yml
  format: yaml
  label: CreatorIQ Payments API
  slug: creatoriq-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-payments-openapi.yml
- filename: creatoriq-webhooks-openapi.yml
  format: yaml
  label: CreatorIQ Webhooks (pub/sub) API
  slug: creatoriq-webhooks-pubsub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/openapi/creatoriq-webhooks-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Creatoriq Authentication
name_suffix: Authentication
oauth_flows: []
overview: CreatorIQ secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CreatorIQ
provider_slug: creatoriq
scheme_count: 3
schemes:
- description: 'Format: Authorization: Bearer {api_key}'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/creatoriq-brand-safety-openapi.yml
  type: http
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/creatoriq-brand-safety-openapi.yml
  - openapi/creatoriq-campaigns-openapi.yml
  - openapi/creatoriq-conversion-metrics-openapi.yml
  - openapi/creatoriq-ecommerce-openapi.yml
  - openapi/creatoriq-lists-openapi.yml
  - openapi/creatoriq-notes-openapi.yml
  - openapi/creatoriq-onesheets-openapi.yml
  - openapi/creatoriq-publishers-openapi.yml
  - openapi/creatoriq-reports-openapi.yml
  - openapi/creatoriq-socials-openapi.yml
  - openapi/creatoriq-v1-divisions-openapi.yml
  - openapi/creatoriq-v2-campaigns-openapi.yml
  - openapi/creatoriq-v2-publishers-openapi.yml
  - openapi/creatoriq-webhooks-openapi.yml
  type: apiKey
- in: header
  name: apiKey
  parameter: X-API-KEY
  sources:
  - openapi/creatoriq-payments-openapi.yml
  type: apiKey
slug: creatoriq-authentication
source_filename: creatoriq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://apidocs.creatoriq.com/docs/ciq-api-documentation/05lf89tv60rvy-introduction-to-api-keys\n  + openapi/ (17 documents)\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Format: Authorization: Bearer {api_key}'\n  sources:\n  - openapi/creatoriq-brand-safety-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/creatoriq-brand-safety-openapi.yml\n  - openapi/creatoriq-campaigns-openapi.yml\n  - openapi/creatoriq-conversion-metrics-openapi.yml\n  - openapi/creatoriq-ecommerce-openapi.yml\n  - openapi/creatoriq-lists-openapi.yml\n  - openapi/creatoriq-notes-openapi.yml\n  - openapi/creatoriq-onesheets-openapi.yml\n  - openapi/creatoriq-publishers-openapi.yml\n  - openapi/creatoriq-reports-openapi.yml\n  - openapi/creatoriq-socials-openapi.yml\n  - openapi/creatoriq-v1-divisions-openapi.yml\n\
  \  - openapi/creatoriq-v2-campaigns-openapi.yml\n  - openapi/creatoriq-v2-publishers-openapi.yml\n  - openapi/creatoriq-webhooks-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/creatoriq-payments-openapi.yml\ndocs: https://apidocs.creatoriq.com/docs/ciq-api-documentation/05lf89tv60rvy-introduction-to-api-keys\nmodel:\n  style: static api key in a request header\n  header: x-api-key (the Payments spec declares it as X-API-KEY; HTTP header names are case-insensitive)\n  oauth2: false\n  oidc: false\n  scopes: false\n  expiry: none documented\n  refresh: none\n  issuance: 'Manual. Docs: \"reach out to your CreatorIQ contact or send an email to support@creatoriq.com\".\n    Sales issues sandbox keys; account managers issue production keys.'\n  self_serve: false\n  levels:\n  - level: partner\n    scope: The whole partner account — all divisions, all events and subscriptions.\n  - level: division\n    scope: One division. Can subscribe\
  \ and unsubscribe for that division only. A partner key can view\n      division subscriptions but cannot change them.\n  rotation: No key-rotation API. Docs recommend periodically creating new keys, deleting old ones and\n    updating applications.\n  restrictions: Docs advise adding \"API key restrictions\" but no restriction mechanism is documented or\n    exposed over the API.\n  transport: Docs instruct that calls be made server-side, not from front-end apps.\nsecondary_use: The API key doubles as the webhook signing secret — X-Signature (MD5) and X-Signature-SHA256\n  are computed over normalizedJson + timestamp + apiKey. Anything that verifies a CreatorIQ webhook therefore\n  holds a credential that can call the entire API.\ngaps:\n- No OAuth 2.0 and no scopes — a key is all-or-nothing within its partner or division.\n- No documented key expiry, no programmatic rotation, no key-management endpoints.\n- No /.well-known/openid-configuration or oauth-authorization-server on any host\
  \ (all 404/403).\n- A missing x-api-key header returns 403, not 401, which is a non-standard signal for \"unauthenticated\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creatoriq/refs/heads/main/authentication/creatoriq-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Influencer Marketing
- Creator Economy
- Social-Media
- Marketing
- Campaign Management
- creator-crm
- Social Analytics
- Brand Safety
- Affiliate Marketing
- Creator Payments
- E-Commerce
- Reporting
- Webhook
---
