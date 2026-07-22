---
api_specs:
- filename: neon-commerce-account-openapi.yml
  format: yaml
  label: Neon Account API
  slug: neon-commerce-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-account-openapi.yml
- filename: neon-commerce-assets-openapi.yml
  format: yaml
  label: Neon Assets API
  slug: neon-commerce-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-assets-openapi.yml
- filename: neon-commerce-auth-openapi.yml
  format: yaml
  label: Neon Auth API
  slug: neon-commerce-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-auth-openapi.yml
- filename: neon-commerce-checkout-openapi.yml
  format: yaml
  label: Neon Checkout API
  slug: neon-commerce-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-checkout-openapi.yml
- filename: neon-commerce-payout-openapi.yml
  format: yaml
  label: Neon Payout API
  slug: neon-commerce-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-payout-openapi.yml
- filename: neon-commerce-purchase-openapi.yml
  format: yaml
  label: Neon Purchase API
  slug: neon-commerce-purchase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-purchase-openapi.yml
- filename: neon-commerce-reports-openapi.yml
  format: yaml
  label: Neon Reports API
  slug: neon-commerce-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-reports-openapi.yml
- filename: neon-commerce-status-openapi.yml
  format: yaml
  label: Neon Status API
  slug: neon-commerce-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-status-openapi.yml
- filename: neon-commerce-storefront-openapi.yml
  format: yaml
  label: Neon Storefront API
  slug: neon-commerce-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-storefront-openapi.yml
- filename: neon-commerce-subscriptions-openapi.yml
  format: yaml
  label: Neon Subscriptions API
  slug: neon-commerce-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/openapi/neon-commerce-subscriptions-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: neonpay.com
  spf: true
hosts:
- cert_expires: Oct  1 02:38:59 2026 GMT
  host: www.neonpay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 22:25:26 2026 GMT
  host: docs.neonpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: api.neonpay.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Neon Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neon Commerce, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Neon Commerce
provider_slug: neon-commerce
slug: neon-commerce-domain-security
source_filename: neon-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neonpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 02:38:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.neonpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 22:25:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.neonpay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: neonpay.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neon-commerce/refs/heads/main/security/neon-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Commerce
- Payments
- Gaming
- Checkout
- Storefront
- Direct-to-Consumer
- Subscriptions
- Merchant of Record
- Game Monetization
- Company
---
