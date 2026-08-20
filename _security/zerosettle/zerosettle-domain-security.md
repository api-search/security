---
api_specs:
- filename: zerosettle-cancel-flow-api-openapi.yml
  format: yaml
  label: ZeroSettle Cancel Flow API
  slug: zerosettle-cancel-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-cancel-flow-api-openapi.yml
- filename: zerosettle-checkout-api-openapi.yml
  format: yaml
  label: ZeroSettle Checkout API
  slug: zerosettle-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-checkout-api-openapi.yml
- filename: zerosettle-entitlements-api-openapi.yml
  format: yaml
  label: ZeroSettle Entitlements API
  slug: zerosettle-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-entitlements-api-openapi.yml
- filename: zerosettle-events-api-openapi.yml
  format: yaml
  label: ZeroSettle Events API
  slug: zerosettle-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-events-api-openapi.yml
- filename: zerosettle-migration-api-openapi.yml
  format: yaml
  label: ZeroSettle Migration API
  slug: zerosettle-migration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-migration-api-openapi.yml
- filename: zerosettle-products-api-openapi.yml
  format: yaml
  label: ZeroSettle Products API
  slug: zerosettle-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-products-api-openapi.yml
- filename: zerosettle-restore-api-openapi.yml
  format: yaml
  label: ZeroSettle Restore API
  slug: zerosettle-restore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-restore-api-openapi.yml
- filename: zerosettle-storekit-api-openapi.yml
  format: yaml
  label: ZeroSettle StoreKit API
  slug: zerosettle-storekit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-storekit-api-openapi.yml
- filename: zerosettle-subscriptions-api-openapi.yml
  format: yaml
  label: ZeroSettle Subscriptions API
  slug: zerosettle-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-subscriptions-api-openapi.yml
- filename: zerosettle-transactions-api-openapi.yml
  format: yaml
  label: ZeroSettle Transactions API
  slug: zerosettle-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-transactions-api-openapi.yml
- filename: zerosettle-upgrade-offers-api-openapi.yml
  format: yaml
  label: ZeroSettle Upgrade Offers API
  slug: zerosettle-upgrade-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-upgrade-offers-api-openapi.yml
- filename: zerosettle-user-offer-api-openapi.yml
  format: yaml
  label: ZeroSettle User Offer API
  slug: zerosettle-user-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-user-offer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zerosettle.io
  spf: true
hosts:
- cert_expires: Oct 17 04:26:06 2026 GMT
  host: api.zerosettle.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zerosettle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZeroSettle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ZeroSettle
provider_slug: zerosettle
slug: zerosettle-domain-security
source_filename: zerosettle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.zerosettle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 04:26:06 2026 GMT\n  hsts: null\ndomains:\n- domain: zerosettle.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/security/zerosettle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- In-App Purchase
- Subscription
- Merchant of Record
- Billing
- Mobile
- Developer Tools
---
