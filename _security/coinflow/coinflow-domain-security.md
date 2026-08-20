---
api_specs:
- filename: coinflow-authentication-api-openapi.yml
  format: yaml
  label: Coinflow authentication API
  slug: coinflow-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-authentication-api-openapi.yml
- filename: coinflow-cardtokenization-api-openapi.yml
  format: yaml
  label: Coinflow cardTokenization API
  slug: coinflow-cardtokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-cardtokenization-api-openapi.yml
- filename: coinflow-checkout-api-openapi.yml
  format: yaml
  label: Coinflow checkout API
  slug: coinflow-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-checkout-api-openapi.yml
- filename: coinflow-customers-api-openapi.yml
  format: yaml
  label: Coinflow customers API
  slug: coinflow-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-customers-api-openapi.yml
- filename: coinflow-events-api-openapi.yml
  format: yaml
  label: Coinflow events API
  slug: coinflow-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-events-api-openapi.yml
- filename: coinflow-marketplace-api-openapi.yml
  format: yaml
  label: Coinflow marketplace API
  slug: coinflow-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-marketplace-api-openapi.yml
- filename: coinflow-merchant-api-openapi.yml
  format: yaml
  label: Coinflow merchant API
  slug: coinflow-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-merchant-api-openapi.yml
- filename: coinflow-merchantsubscription-api-openapi.yml
  format: yaml
  label: Coinflow merchantSubscription API
  slug: coinflow-merchantsubscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-merchantsubscription-api-openapi.yml
- filename: coinflow-redeem-api-openapi.yml
  format: yaml
  label: Coinflow redeem API
  slug: coinflow-redeem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-redeem-api-openapi.yml
- filename: coinflow-refund-api-openapi.yml
  format: yaml
  label: Coinflow refund API
  slug: coinflow-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-refund-api-openapi.yml
- filename: coinflow-submerchant-api-openapi.yml
  format: yaml
  label: Coinflow subMerchant API
  slug: coinflow-submerchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-submerchant-api-openapi.yml
- filename: coinflow-subscription-api-openapi.yml
  format: yaml
  label: Coinflow subscription API
  slug: coinflow-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-subscription-api-openapi.yml
- filename: coinflow-utilities-api-openapi.yml
  format: yaml
  label: Coinflow utilities API
  slug: coinflow-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-utilities-api-openapi.yml
- filename: coinflow-withdraw-api-openapi.yml
  format: yaml
  label: Coinflow withdraw API
  slug: coinflow-withdraw-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/openapi/coinflow-withdraw-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coinflow.cash
  spf: true
hosts:
- cert_expires: Oct  1 14:31:00 2026 GMT
  host: coinflow.cash
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 14:32:10 2026 GMT
  host: api-sandbox.coinflow.cash
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinflow, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coinflow
provider_slug: coinflow
slug: coinflow-domain-security
source_filename: coinflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinflow.cash\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:31:00 2026 GMT\n  hsts: false\n- host: api-sandbox.coinflow.cash\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 14:32:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coinflow.cash\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinflow/refs/heads/main/security/coinflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Payments
- Stablecoins
- USDC
- Checkout
- Payouts
- Marketplace
- Web3
- Fintech
---
