---
api_key_in: []
api_specs:
- filename: cloudwalk-checkout-links-api-openapi.yml
  format: yaml
  label: CloudWalk Checkout Links API
  slug: cloudwalk-checkout-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwalk/refs/heads/main/openapi/cloudwalk-checkout-links-api-openapi.yml
- filename: cloudwalk-infinitepay-checkout-api-api-openapi.yml
  format: yaml
  label: CloudWalk InfinitePay Checkout API
  slug: cloudwalk-infinitepay-checkout-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwalk/refs/heads/main/openapi/cloudwalk-infinitepay-checkout-api-api-openapi.yml
- filename: cloudwalk-payments-api-openapi.yml
  format: yaml
  label: CloudWalk Payments API
  slug: cloudwalk-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwalk/refs/heads/main/openapi/cloudwalk-payments-api-openapi.yml
auth_types: []
description: CloudWalk's public InfinitePay Checkout API has NO transport-level authentication. The mechanical derivation from the captured OpenAPI produced no security schemes because there are none to derive — the provider genuinely publishes an unauthenticated write endpoint. The merchant is identified by its InfiniteTag `handle` in the JSON request body, and the InfiniteTap FAQ states outright that no API key is needed to integrate. This is recorded as a finding, not a gap in our harvest.
kind: authentication
layout: security
method: searched
name: Cloudwalk Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudWalk declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: CloudWalk
provider_slug: cloudwalk
scheme_count: 0
schemes: []
slug: cloudwalk-authentication
source_filename: cloudwalk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: >-\n  https://www.infinitepay.io/checkout-documentacao and\n  https://www.infinitepay.io/checkout-tap, plus live probes on 2026-08-01.\ndocs: https://www.infinitepay.io/checkout-documentacao\ndescription: >-\n  CloudWalk's public InfinitePay Checkout API has NO transport-level authentication. The\n  mechanical derivation from the captured OpenAPI produced no security schemes because there\n  are none to derive — the provider genuinely publishes an unauthenticated write endpoint.\n  The merchant is identified by its InfiniteTag `handle` in the JSON request body, and the\n  InfiniteTap FAQ states outright that no API key is needed to integrate. This is recorded as\n  a finding, not a gap in our harvest.\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  transport_auth: none\n  identification: request-body field (`handle`, the merchant's InfiniteTag)\nschemes: []\nmodel:\n  merchant_identifier:\n    field: handle\n\
  \    location: request body (JSON)\n    description: >-\n      The merchant's InfiniteTag — the public username in the InfinitePay app — sent without\n      its leading \"$\". Required on both POST /links and POST /payment_check.\n    secrecy: >-\n      Not a secret. An InfiniteTag is a public handle used for consumer payment links, so it\n      confers no authentication value.\n  provisioning: >-\n    None. There is no developer registration, no credential issuance, no dashboard key\n    management and no client_id in the published contract. Partner integration questions go\n    to parcerias@cloudwalk.io.\n  authorization: >-\n    None published. There are no scopes, roles or permissions; the two operations are the\n    entire surface.\n  payment_check_binding: >-\n    payment_check requires handle + order_nsu + transaction_nsu + slug together, so reading a\n    payment status requires possession of identifiers only the paying flow produces. That\n    quadruple acts as a weak capability\
  \ check in place of authentication.\nobserved_but_undocumented:\n- host: https://authorizer.infinitepay.io\n  path: /v2/cards/tokenize\n  method: POST\n  probe:\n    http_status: 400\n    date: '2026-08-01'\n  note: >-\n    A card-tokenization endpoint exists and responds. Search-engine snippets of the\n    now-offline docs.infinitepay.io referenced authenticating with a `card_tokenization`\n    scope before calling it, implying an OAuth-style scoped credential on a\n    partner-only surface. docs.infinitepay.io does not resolve in DNS (NXDOMAIN on\n    1.1.1.1 and 8.8.8.8) and has no Wayback snapshot, so nothing about that scheme could be\n    verified. Recorded as an observed endpoint only — no scopes artifact was written,\n    because there is no live published scope reference to capture.\nwebhook_authentication:\n  signing: none published\n  shared_secret: none published\n  note: >-\n    Incoming webhooks carry no signature and no authentication. The provider's own guidance\n    is\
  \ to validate that `order_nsu` matches a real order, then confirm via payment_check.\n    Integrators should treat the webhook as an untrusted hint and verify out of band.\ntransport_security:\n  https_required: true\n  tls: TLSv1.3 observed on api.checkout.infinitepay.io\n  hsts: true\n  detail: security/cloudwalk-domain-security.yml\ngaps:\n- No API keys, tokens, OAuth or mTLS on the public checkout API.\n- Link creation is an unauthenticated write bound only to a public merchant handle.\n- No webhook signing.\n- No published credential rotation, revocation or least-privilege model.\nx-evidence:\n  fetched: '2026-08-01'\n  derive_script: 'python3 all/0-working/derive-authentication.py cloudwalk → 0 auth profiles (no securitySchemes in spec, correctly reflecting the API)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudwalk/refs/heads/main/authentication/cloudwalk-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Payments
- Financial-Services
- Fintech
- Checkout
- Point-of-Sale
- Acquiring
- Pix
- Brazil
- Banking
- Webhook
- Tap to Pay
---
