---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chia-health-catalog-api-openapi.yml
  format: yaml
  label: Chia Health Catalog API
  slug: chia-health-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chia-health/openapi/chia-health-catalog-api-openapi.yml
- filename: chia-health-handoff-sessions-api-openapi.yml
  format: yaml
  label: Chia Health Handoff sessions API
  slug: chia-health-handoff-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chia-health/openapi/chia-health-handoff-sessions-api-openapi.yml
- filename: chia-health-settlements-api-openapi.yml
  format: yaml
  label: Chia Health Settlements API
  slug: chia-health-settlements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chia-health/openapi/chia-health-settlements-api-openapi.yml
- filename: chia-health-webhook-tests-api-openapi.yml
  format: yaml
  label: Chia Health Webhook tests API
  slug: chia-health-webhook-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chia-health/openapi/chia-health-webhook-tests-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Chia Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chia Health secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Chia Health
provider_slug: chia-health
scheme_count: 2
schemes:
- bearerFormat: chia_test_… / chia_test_finance_… / chia_live_… / chia_live_finance_…
  description: 'Every request sends `Authorization: Bearer ${CHIA_RUNTIME_KEY}` or `Authorization: Bearer ${CHIA_FINANCE_KEY}` from confidential server workloads only. Credentials are environment-, tenant- and role-bound; tenant identity is derived from the credential, never from a caller-supplied header. No self-service issuance: six values (sandbox/production x runtime/finance/webhook) are delivered via signed onboarding through an approved secret channel.'
  key_prefixes:
    production_finance: chia_live_finance_…
    production_runtime: chia_live_…
    production_webhook_secret: whsec_live_…
    sandbox_finance: chia_test_finance_…
    sandbox_runtime: chia_test_…
    sandbox_webhook_secret: whsec_test_…
  name: bearerAuth
  roles:
  - allowed:
    - catalog:read
    - handoffs:create
    - authenticated asset GET
    - webhooks:test
    role: runtime catalog/handoff service; ephemeral test job
    secret: runtime key
  - allowed:
    - verify inbound Chia events
    role: webhook receiver
    secret: current signing secret; optionally one retiring secret
  - allowed:
    - settlements:read
    role: finance worker
    secret: finance key
  - allowed:
    - partner-projected cards and OS-browser navigation
    role: mobile app
    secret: none
  rotation: Provision and validate the replacement key, switch the workload, then revoke the old key; webhook secrets overlap with at most two signing secrets during rotation.
  scheme: bearer
  sources:
  - openapi/chia-health-openapi.yml
  - https://partners.chia.health/docs/environments/
  type: http
- api: Chia affiliate read API (/api/affiliate/v1, limited pilot)
  bearerFormat: chia_aff_live_<12 lowercase hex>_<43 URL-safe characters> / chia_aff_test_…
  description: Separate credential issued by the named Chia affiliate integration owner; no self-service issuance. Every authentication and authorisation failure returns one identical opaque 401.
  name: affiliateBearer
  scheme: bearer
  sources:
  - https://partners.chia.health/docs/affiliate-read-api/
  type: http
slug: chia-health-authentication
source_filename: chia-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://partners.chia.health/docs/environments/\ndocs: https://partners.chia.health/docs/environments/\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: chia_test_… / chia_test_finance_… / chia_live_… / chia_live_finance_…\n  description: 'Every request sends `Authorization: Bearer ${CHIA_RUNTIME_KEY}` or `Authorization: Bearer\n    ${CHIA_FINANCE_KEY}` from confidential server workloads only. Credentials are environment-, tenant-\n    and role-bound; tenant identity is derived from the credential, never from a caller-supplied header.\n    No self-service issuance: six values (sandbox/production x runtime/finance/webhook) are delivered\n    via signed onboarding through an approved secret channel.'\n  sources:\n  - openapi/chia-health-openapi.yml\n  - https://partners.chia.health/docs/environments/\n  key_prefixes:\n    sandbox_runtime: chia_test_…\n    sandbox_finance:\
  \ chia_test_finance_…\n    production_runtime: chia_live_…\n    production_finance: chia_live_finance_…\n    sandbox_webhook_secret: whsec_test_…\n    production_webhook_secret: whsec_live_…\n  roles:\n  - role: runtime catalog/handoff service; ephemeral test job\n    secret: runtime key\n    allowed: [catalog:read, handoffs:create, authenticated asset GET, webhooks:test]\n  - role: webhook receiver\n    secret: current signing secret; optionally one retiring secret\n    allowed: [verify inbound Chia events]\n  - role: finance worker\n    secret: finance key\n    allowed: [settlements:read]\n  - role: mobile app\n    secret: none\n    allowed: [partner-projected cards and OS-browser navigation]\n  rotation: Provision and validate the replacement key, switch the workload, then revoke the old key;\n    webhook secrets overlap with at most two signing secrets during rotation.\n- name: affiliateBearer\n  type: http\n  scheme: bearer\n  api: Chia affiliate read API (/api/affiliate/v1, limited\
  \ pilot)\n  bearerFormat: chia_aff_live_<12 lowercase hex>_<43 URL-safe characters> / chia_aff_test_…\n  description: Separate credential issued by the named Chia affiliate integration owner; no self-service\n    issuance. Every authentication and authorisation failure returns one identical opaque 401.\n  sources:\n  - https://partners.chia.health/docs/affiliate-read-api/\nwebhook_signing:\n  scheme: HMAC over the exact raw body, single `v1` signature, 300-second timestamp tolerance\n  docs: https://partners.chia.health/docs/webhooks/\n"
source_yaml_url: https://artifacts.apis.io/chia-health/authentication/chia-health-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Telehealth
- Healthcare
- Peptides
- GLP-1
- Weight Loss
- Partner API
- MCP
---
