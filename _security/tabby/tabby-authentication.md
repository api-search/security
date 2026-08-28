---
api_key_in: []
api_specs:
- filename: tabby-checkout-api-openapi.yml
  format: yaml
  label: Tabby Checkout API
  slug: tabby-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-checkout-api-openapi.yml
- filename: tabby-disputes-api-openapi.yml
  format: yaml
  label: Tabby Disputes API
  slug: tabby-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-disputes-api-openapi.yml
- filename: tabby-payments-api-openapi.yml
  format: yaml
  label: Tabby Payments API
  slug: tabby-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-payments-api-openapi.yml
- filename: tabby-webhooks-api-openapi.yml
  format: yaml
  label: Tabby Webhooks API
  slug: tabby-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Tabby Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tabby declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Tabby
provider_slug: tabby
scheme_count: 1
schemes:
- applies_to: all 19 operations
  description: Bearer authentication header of the form `Bearer <secret_key>`, where `<secret_key>` is your secret_key.
  format: Bearer <secret_key>
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_original/tabby-api-openapi.yml
  - https://docs.tabby.ai/introduction/technical-requirements#authentication
  type: http
slug: tabby-authentication
source_filename: tabby-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://docs.tabby.ai/introduction/technical-requirements#authentication\ndocs: https://docs.tabby.ai/introduction/technical-requirements#authentication\nderived_from: openapi/_original/tabby-api-openapi.yml\nprovider: Tabby\nproviderId: tabby\nsummary: >-\n  A single static bearer credential. Tabby issues two keys per merchant account — a secret key used\n  server-side for every Checkout, Payments, Webhooks and Disputes call, and a public key used only\n  in the browser for promo snippets. The key prefix, not the host, selects test or live. There is no\n  OAuth, no OIDC, no scopes and no key rotation surface documented.\nsummary_types:\n  types:\n    - http\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer <secret_key>'\n    description: >-\n      Bearer authentication header of the form `Bearer <secret_key>`, where `<secret_key>` is your\n \
  \     secret_key.\n    applies_to: all 19 operations\n    sources:\n      - openapi/_original/tabby-api-openapi.yml\n      - https://docs.tabby.ai/introduction/technical-requirements#authentication\ncredentials:\n  - name: Secret Key\n    role: server-to-server authorization\n    prefix_live: sk_\n    prefix_test: sk_test_\n    transport: Authorization header on every request\n    scope: >-\n      Bound to a merchant account. Also determines which environment a webhook registration\n      subscribes to.\n    exposure_rule: Never send to the browser or commit to version control.\n  - name: Public Key\n    role: client-side promo snippets, plans and customization\n    prefix_live: pk_\n    prefix_test: pk_test_\n    transport: Passed to TabbyPromo / TabbyCard constructors in page JavaScript\n    scope: Display only. Cannot authorize a payment operation.\nenvironment_selection:\n  mechanism: key-prefix\n  hosts_shared: true\n  note: >-\n    api.tabby.ai and api.tabby.sa each serve both test\
  \ and live. Tabby identifies the environment\n    from the key, so a test key against the production host is the normal test path.\nissuance:\n  - path: Merchant Dashboard (merchant.tabby.ai / merchant.tabby.sa)\n    for: Self-hosted plugin integrations\n  - path: Tabby account manager, after Tabby-side QA testing is complete\n    for: Custom (Direct API) integrations\nrotation:\n  documented: false\n  note: No key rotation, expiry or revocation procedure is published.\nmtls: false\noauth2: false\noidc: false\nscopes:\n  present: false\n  note: >-\n    No scope or permission model exists — a secret key can call every operation the merchant account\n    is entitled to. scopes/ is intentionally absent for this provider.\nregional_note: >-\n  Keys are region-bound in practice: a key issued for a KSA merchant is used against api.tabby.sa,\n  and currency validation will reject a mismatched market (the checkout error\n  \"only AED is supported, but got SAR\" is exactly this).\nfailure_modes:\n\
  \  - status: 401\n    errorType: not_authorized\n    messages:\n      - authorization\n      - missing Bearer scheme\n      - invalid secret key\n      - \"auth: provided key doesn't exist\"\n      - merchant is null\n    detail: errors/tabby-problem-types.yml\n  - status: 403\n    errorType: no_permission\n    meaning: Authenticated, but the resource does not belong to this merchant.\ntransport_requirements:\n  tls_minimum: TLSv1.2\n  cipher_suites: Restricted for PCI DSS compliance; enumerated at the docs source above.\n  detail: security/tabby-domain-security.yml\nwebhook_authentication:\n  inbound_to_merchant: >-\n    Optional caller-defined auth header set at webhook registration and echoed on every delivery.\n    No HMAC signature, no timestamp, no rotation. Combine with the published source-IP allowlist.\n  detail: asyncapi/tabby-webhooks.yml\ndiscovery:\n  well_known_openid_configuration: 404 on all hosts\n  well_known_oauth_authorization_server: 404 on all hosts\n  detail: well-known/tabby-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/authentication/tabby-authentication.yml
summary_line: 1 scheme
tags:
- BNPL
- Buy Now Pay Later
- Consumer Finance
- E-Commerce
- Fintech
- Installments
- MENA
- Payments
- Saudi Arabia
- UAE
---
