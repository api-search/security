---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agendapro-available-slots-api-openapi.yml
  format: yaml
  label: AgendaPro Available Slots API
  slug: agendapro-available-slots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-available-slots-api-openapi.yml
- filename: agendapro-bookings-api-openapi.yml
  format: yaml
  label: AgendaPro Bookings API
  slug: agendapro-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-bookings-api-openapi.yml
- filename: agendapro-carts-api-openapi.yml
  format: yaml
  label: AgendaPro Carts API
  slug: agendapro-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-carts-api-openapi.yml
- filename: agendapro-clients-api-openapi.yml
  format: yaml
  label: AgendaPro Clients API
  slug: agendapro-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-clients-api-openapi.yml
- filename: agendapro-custom-attributes-api-openapi.yml
  format: yaml
  label: AgendaPro Custom Attributes API
  slug: agendapro-custom-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-custom-attributes-api-openapi.yml
- filename: agendapro-locations-api-openapi.yml
  format: yaml
  label: AgendaPro Locations API
  slug: agendapro-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-locations-api-openapi.yml
- filename: agendapro-payment-requests-api-openapi.yml
  format: yaml
  label: AgendaPro Payment Requests API
  slug: agendapro-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-payment-requests-api-openapi.yml
- filename: agendapro-providers-api-openapi.yml
  format: yaml
  label: AgendaPro Providers API
  slug: agendapro-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-providers-api-openapi.yml
- filename: agendapro-sales-api-openapi.yml
  format: yaml
  label: AgendaPro Sales API
  slug: agendapro-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-sales-api-openapi.yml
- filename: agendapro-services-api-openapi.yml
  format: yaml
  label: AgendaPro Services API
  slug: agendapro-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-services-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agendapro Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgendaPro secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AgendaPro
provider_slug: agendapro
scheme_count: 1
schemes:
- applied: globally (top-level security in the OpenAPI applies BearerAuth to all 28 operations)
  description: 'API key issued per company. Pass as Authorization: Bearer <key>.'
  format: Bearer <api-key>
  header: Authorization
  key_prefix: apk_live_
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/agendapro-connect-v3-openapi.yml
  - https://developers.agendapro.com/docs/authentication
  type: http
slug: agendapro-authentication
source_filename: agendapro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://developers.agendapro.com/docs/authentication\ndocs: https://developers.agendapro.com/docs/authentication\nsummary:\n  types:\n  - http\n  model: Per-company API key presented as an HTTP Bearer token\n  oauth2: false\n  openid_connect: false\n  mtls: false\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key issued per company. Pass as Authorization: Bearer <key>.'\n  header: Authorization\n  format: Bearer <api-key>\n  key_prefix: apk_live_\n  applied: globally (top-level security in the OpenAPI applies BearerAuth to all 28 operations)\n  sources:\n  - openapi/agendapro-connect-v3-openapi.yml\n  - https://developers.agendapro.com/docs/authentication\nkey_management:\n  issued_from: Configuraciones > Integraciones in the AgendaPro web app\n  requires_plan: Pro\n  max_active_keys_per_company: 2\n  shown_once: true\n  shown_once_note: The full key is displayed only once at creation and\
  \ cannot be retrieved again.\n  revocation: permanent and immediate\n  rotation_policy: not published\n  expiry: not published (keys do not carry a documented TTL)\n  tenancy: A key is scoped to a single company; company_id is derived from the key and is never passed as a parameter.\n  source: https://developers.agendapro.com/docs/authentication\nscopes:\n  supported: true\n  model: '{resource}:{action}'\n  empty_means_full_access: true\n  catalog: scopes/agendapro-scopes.yml\ntransport:\n  https_required: true\n  http_rejected: true\n  source: https://developers.agendapro.com/docs/authentication\nfailure_modes:\n- status: 401\n  error: unauthorized\n  detail: invalid_api_key\n  meaning: Missing or invalid Bearer token.\n- status: 401\n  error: unauthorized\n  detail: api_config_inactive\n  meaning: API access is inactive for this company.\n- status: 403\n  error: forbidden\n  detail: scope_denied\n  meaning: API key lacks the required scope.\nnotes:\n- No OAuth 2.0, OpenID Connect, mTLS\
  \ or signed-request option is published. A single static per-company bearer credential\n  is the whole authentication surface.\n- Webhook deliveries are authenticated in the opposite direction with an HMAC-SHA256 signature in X-Webhook-Signature;\n  see asyncapi/agendapro-webhooks.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/authentication/agendapro-authentication.yml
summary_line: http · 1 scheme
tags:
- Appointment Scheduling
- Booking
- Salon Software
- Spa and Wellness
- Point-of-Sale
- Clinic Management
- CRM
- Payments
- Webhook
- Vertical SaaS
- Latin America
- SMB Software
- Scheduling
---
