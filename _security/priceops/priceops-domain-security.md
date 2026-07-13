---
api_specs:
- filename: customer-information-and-usage-record-api
  format: yaml
  label: PriceOps API
  slug: priceops-api
  spec_type: OpenAPI
  url: https://docs.priceops.net/documentation/developers/customer-information-and-usage-record-api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: priceops.net
  spf: true
hosts:
- cert_expires: Sep 25 06:04:04 2026 GMT
  host: www.priceops.net
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 13:33:14 2026 GMT
  host: docs.priceops.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 17:45:14 2026 GMT
  host: engine.prod.priceops.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Priceops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PriceOps, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PriceOps
provider_slug: priceops
slug: priceops-domain-security
source_filename: priceops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.priceops.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:04:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: docs.priceops.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:33:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: engine.prod.priceops.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 17:45:14 2026 GMT\n  hsts: null\ndomains:\n- domain: priceops.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/priceops/refs/heads/main/security/priceops-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pricing
- Packaging
- SaaS
- Monetization
- Plans
- Entitlements
- Usage Billing
- Stripe Integration
- Price Optimization
- Revenue Analytics
---
