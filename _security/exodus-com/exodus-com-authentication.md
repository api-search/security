---
anonymous_access: false
api_key_in: []
api_specs:
- filename: exodus-com-checkouts-api-openapi.yml
  format: yaml
  label: Exodus Checkouts API
  slug: exodus-com-checkouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-checkouts-api-openapi.yml
- filename: exodus-com-payments-api-openapi.yml
  format: yaml
  label: Exodus Payments API
  slug: exodus-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-payments-api-openapi.yml
- filename: exodus-com-reports-api-openapi.yml
  format: yaml
  label: Exodus Reports API
  slug: exodus-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-reports-api-openapi.yml
- filename: exodus-com-settings-api-openapi.yml
  format: yaml
  label: Exodus Settings API
  slug: exodus-com-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-settings-api-openapi.yml
- filename: exodus-com-subscription-checkouts-api-openapi.yml
  format: yaml
  label: Exodus Subscription checkouts API
  slug: exodus-com-subscription-checkouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-subscription-checkouts-api-openapi.yml
- filename: exodus-com-subscriptions-api-openapi.yml
  format: yaml
  label: Exodus Subscriptions API
  slug: exodus-com-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-subscriptions-api-openapi.yml
- filename: exodus-com-webhook-events-api-openapi.yml
  format: yaml
  label: Exodus Webhook events API
  slug: exodus-com-webhook-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exodus-com/openapi/exodus-com-webhook-events-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Exodus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exodus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Exodus
provider_slug: exodus-com
scheme_count: 1
schemes:
- description: 'Merchant secret API key. Send as `Authorization: Bearer sk_...`. Keys can be restricted to scopes: `read` (all GET endpoints), `checkouts_write` (create/cancel checkouts and quotes), `payments_write` (capture, refund, rescue, recover, subscription charge/cancel), `settings_write` (webhook, settlement, and signer configuration — highest privilege). Calls outside a key’s scopes fail with 403 `permis'
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/exodus-com-openapi.json
  type: http
slug: exodus-com-authentication
source_filename: exodus-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/exodus-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  description: 'Merchant secret API key. Send as `Authorization: Bearer sk_...`. Keys can be\n    restricted to scopes: `read` (all GET endpoints), `checkouts_write` (create/cancel checkouts\n    and quotes), `payments_write` (capture, refund, rescue, recover, subscription charge/cancel),\n    `settings_write` (webhook, settlement, and signer configuration — highest privilege). Calls\n    outside a key’s scopes fail with 403 `permis'\n  sources:\n  - openapi/exodus-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/exodus-com/authentication/exodus-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cryptocurrency
- Wallets
- Finance
- Payments
- Security
---
