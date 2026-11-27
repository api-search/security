---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: loppee-com-account-api-openapi.yml
  format: yaml
  label: Loppee Account API
  slug: loppee-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loppee-com/openapi/loppee-com-account-api-openapi.yml
- filename: loppee-com-agent-contract-api-openapi.yml
  format: yaml
  label: Loppee Agent Contract API
  slug: loppee-com-agent-contract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loppee-com/openapi/loppee-com-agent-contract-api-openapi.yml
- filename: loppee-com-business-owner-api-openapi.yml
  format: yaml
  label: Loppee Business Owner API
  slug: loppee-com-business-owner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loppee-com/openapi/loppee-com-business-owner-api-openapi.yml
- filename: loppee-com-customer-account-api-openapi.yml
  format: yaml
  label: Loppee Customer Account API
  slug: loppee-com-customer-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loppee-com/openapi/loppee-com-customer-account-api-openapi.yml
- filename: loppee-com-customer-jobs-api-openapi.yml
  format: yaml
  label: Loppee Customer Jobs API
  slug: loppee-com-customer-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loppee-com/openapi/loppee-com-customer-jobs-api-openapi.yml
- filename: loppee-com-destination-address-suggestions-api-openapi.yml
  format: yaml
  label: Loppee Destination Address Suggestions API
  slug: loppee-com-destination-address-suggestions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loppee-com/openapi/loppee-com-destination-address-suggestions-api-openapi.yml
- filename: loppee-com-destination-location-proofs-api-openapi.yml
  format: yaml
  label: Loppee Destination Location Proofs API
  slug: loppee-com-destination-location-proofs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loppee-com/openapi/loppee-com-destination-location-proofs-api-openapi.yml
- filename: loppee-com-discovery-api-openapi.yml
  format: yaml
  label: Loppee Discovery API
  slug: loppee-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loppee-com/openapi/loppee-com-discovery-api-openapi.yml
- filename: loppee-com-location-proofs-api-openapi.yml
  format: yaml
  label: Loppee Location Proofs API
  slug: loppee-com-location-proofs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loppee-com/openapi/loppee-com-location-proofs-api-openapi.yml
- filename: loppee-com-moderated-actions-api-openapi.yml
  format: yaml
  label: Loppee Moderated Actions API
  slug: loppee-com-moderated-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loppee-com/openapi/loppee-com-moderated-actions-api-openapi.yml
- filename: loppee-com-operations-api-openapi.yml
  format: yaml
  label: Loppee Operations API
  slug: loppee-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loppee-com/openapi/loppee-com-operations-api-openapi.yml
- filename: loppee-com-trust-cards-api-openapi.yml
  format: yaml
  label: Loppee Trust Cards API
  slug: loppee-com-trust-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loppee-com/openapi/loppee-com-trust-cards-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: derived
name: Loppee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loppee secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Loppee
provider_slug: loppee-com
scheme_count: 6
schemes:
- description: Scoped agent key. Admin-agent requests are authorized only by the key's explicit allowed_actions; admin-agent keys cannot delete users or agents.
  in: header
  name: AgentApiKey
  parameter: X-LOPPEE-API-Key
  sources:
  - openapi/loppee-com-openapi.json
  type: apiKey
- description: Bearer form of a scoped agent key for non-admin agent workflows. Admin routes deliberately require X-LOPPEE-API-Key for agent keys so Authorization remains unambiguous for human Supabase admin sessions.
  name: AgentBearer
  scheme: bearer
  sources:
  - openapi/loppee-com-openapi.json
  type: http
- description: Stripe webhook signature verified against the configured endpoint secret before any mutation.
  in: header
  name: StripeSignature
  parameter: Stripe-Signature
  sources:
  - openapi/loppee-com-openapi.json
  type: apiKey
- description: Single-intent HMAC callback authority supplied only to the private Render Workflow task.
  in: header
  name: OwnerEvidenceScanCallback
  parameter: X-Loppee-Scan-Callback-Token
  sources:
  - openapi/loppee-com-openapi.json
  type: apiKey
- description: Dedicated single-intent callback authority supplied only to the private job-resume scanner task; it is bound to the immutable scan authority and exact file fingerprint.
  in: header
  name: JobResumeScanCallback
  parameter: X-Loppee-Job-Resume-Scan-Callback-Token
  sources:
  - openapi/loppee-com-openapi.json
  type: apiKey
- description: Lowercase hexadecimal HMAC-SHA256 of '<X-Webhook-Timestamp>.<raw request body>' using the one-time endpoint signing secret. The signing secret authenticates this delivery only and grants no Loppee API authority.
  in: header
  name: ExternalAgentWebhookHmac
  parameter: X-Webhook-Signature-V2
  sources:
  - openapi/loppee-com-openapi.json
  type: apiKey
slug: loppee-com-authentication
source_filename: loppee-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/loppee-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: AgentApiKey\n  type: apiKey\n  in: header\n  parameter: X-LOPPEE-API-Key\n  description: Scoped agent key. Admin-agent requests are authorized only by the key's explicit\n    allowed_actions; admin-agent keys cannot delete users or agents.\n  sources:\n  - openapi/loppee-com-openapi.json\n- name: AgentBearer\n  type: http\n  scheme: bearer\n  description: Bearer form of a scoped agent key for non-admin agent workflows. Admin routes\n    deliberately require X-LOPPEE-API-Key for agent keys so Authorization remains unambiguous\n    for human Supabase admin sessions.\n  sources:\n  - openapi/loppee-com-openapi.json\n- name: StripeSignature\n  type: apiKey\n  in: header\n  parameter: Stripe-Signature\n  description: Stripe webhook signature verified against the configured endpoint secret before\n    any mutation.\n\
  \  sources:\n  - openapi/loppee-com-openapi.json\n- name: OwnerEvidenceScanCallback\n  type: apiKey\n  in: header\n  parameter: X-Loppee-Scan-Callback-Token\n  description: Single-intent HMAC callback authority supplied only to the private Render Workflow\n    task.\n  sources:\n  - openapi/loppee-com-openapi.json\n- name: JobResumeScanCallback\n  type: apiKey\n  in: header\n  parameter: X-Loppee-Job-Resume-Scan-Callback-Token\n  description: Dedicated single-intent callback authority supplied only to the private job-resume\n    scanner task; it is bound to the immutable scan authority and exact file fingerprint.\n  sources:\n  - openapi/loppee-com-openapi.json\n- name: ExternalAgentWebhookHmac\n  type: apiKey\n  in: header\n  parameter: X-Webhook-Signature-V2\n  description: Lowercase hexadecimal HMAC-SHA256 of '<X-Webhook-Timestamp>.<raw request body>'\n    using the one-time endpoint signing secret. The signing secret authenticates this delivery\n    only and grants no Loppee API authority.\n\
  \  sources:\n  - openapi/loppee-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/loppee-com/authentication/loppee-com-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- Business
- Artificial Intelligence
- Marketplace
- Local
- Services
---
