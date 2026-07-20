---
api_key_in:
- header
auth_types:
- apiKey
- http
- hmac
description: ''
kind: authentication
layout: security
method: searched
name: Butterpayments Authentication
name_suffix: Authentication
oauth_flows: []
overview: Butterpayments secures its APIs with apiKey, http, and hmac across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Butterpayments
provider_slug: butterpayments
scheme_count: 5
schemes:
- applies_to: Recover Enterprise API (Butter-hosted endpoints)
  example: 'curl ''https://api.butterpayments.com/recover/payments'' --header ''x-api-key: <BUTTER_API_KEY>'''
  in: header
  name: ButterApiKey
  parameter: x-api-key
  provisioning: Butter issues API keys per environment (sandbox and production) during the integration phase.
  sources:
  - https://docs.services.butterpayments.com/authentication
  type: apiKey
- applies_to: Merchant-provided endpoints (Retry Status, Retry Results, End of Dunning)
  in: header
  name: MerchantApiKey
  notes: Merchants may secure their own inbound endpoints with an API key shared with Butter.
  parameter: x-api-key
  sources:
  - https://docs.services.butterpayments.com/authentication
  type: apiKey
- applies_to: Merchant-provided endpoints
  name: MerchantBasicAuth
  notes: HTTP Basic (base64 username:password) is a supported scheme for merchant endpoints.
  scheme: basic
  sources:
  - https://docs.services.butterpayments.com/authentication
  type: http
- applies_to: Disputes / Data Collection API (api.disputes.services.butterpayments.com Ping health check)
  name: HTTPBasic
  scheme: basic
  sources:
  - https://docs.services.butterpayments.com/ping
  type: http
- algorithm: HMAC-SHA256
  applies_to: Butter-sent webhooks (Retry Results, End of Dunning, Disputes)
  expiration_header: X-Butter-Webhook-Expiration
  name: WebhookSignature
  signature_header: X-Butter-Webhook-Signature
  signing: HMAC-SHA256 over "{json_payload}+{expiration}" using the Butter-provided signing secret as the key; compare to X-Butter-Webhook-Signature and verify X-Butter-Webhook-Expiration.
  sources:
  - https://docs.services.butterpayments.com/webhook-signature-verification
  type: hmac
slug: butterpayments-authentication
source_filename: butterpayments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.services.butterpayments.com/authentication\ndocs: https://docs.services.butterpayments.com/authentication\nsummary:\n  types: [apiKey, http, hmac]\n  api_key_in: [header]\n  api_key_header: x-api-key\n  webhook_signing: HMAC-SHA256\n  notes: >-\n    No machine-readable OpenAPI is published; this profile is captured from the\n    Recover Enterprise API authentication documentation.\nschemes:\n  - name: ButterApiKey\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    applies_to: Recover Enterprise API (Butter-hosted endpoints)\n    provisioning: Butter issues API keys per environment (sandbox and production) during the integration phase.\n    example: \"curl 'https://api.butterpayments.com/recover/payments' --header 'x-api-key: <BUTTER_API_KEY>'\"\n    sources: [https://docs.services.butterpayments.com/authentication]\n  - name: MerchantApiKey\n    type: apiKey\n    in: header\n    parameter: x-api-key\n\
  \    applies_to: Merchant-provided endpoints (Retry Status, Retry Results, End of Dunning)\n    notes: Merchants may secure their own inbound endpoints with an API key shared with Butter.\n    sources: [https://docs.services.butterpayments.com/authentication]\n  - name: MerchantBasicAuth\n    type: http\n    scheme: basic\n    applies_to: Merchant-provided endpoints\n    notes: HTTP Basic (base64 username:password) is a supported scheme for merchant endpoints.\n    sources: [https://docs.services.butterpayments.com/authentication]\n  - name: HTTPBasic\n    type: http\n    scheme: basic\n    applies_to: Disputes / Data Collection API (api.disputes.services.butterpayments.com Ping health check)\n    sources: [https://docs.services.butterpayments.com/ping]\n  - name: WebhookSignature\n    type: hmac\n    algorithm: HMAC-SHA256\n    applies_to: Butter-sent webhooks (Retry Results, End of Dunning, Disputes)\n    signature_header: X-Butter-Webhook-Signature\n    expiration_header: X-Butter-Webhook-Expiration\n\
  \    signing: >-\n      HMAC-SHA256 over \"{json_payload}+{expiration}\" using the Butter-provided signing\n      secret as the key; compare to X-Butter-Webhook-Signature and verify X-Butter-Webhook-Expiration.\n    sources: [https://docs.services.butterpayments.com/webhook-signature-verification]\nip_allowlisting:\n  supported: true\n  notes: Recover source IPs can be provided on request to allowlist inbound traffic.\nvault_keys:\n  merchant_key: Directs card element requests to a dedicated proxy and secure container.\n  source_id: Represents a specific PSP account where card payment methods are created after vaulting.\n  source: https://docs.services.butterpayments.com/api-key-provisioning\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/butterpayments/refs/heads/main/authentication/butterpayments-authentication.yml
summary_line: apiKey/http/hmac · 5 schemes
tags:
- Company
- Payments
- Payment Recovery
- Subscriptions
- Dunning
- Involuntary Churn
- Dispute Prevention
- Chargebacks
- Card Vault
- Fintech
- Machine Learning
---
