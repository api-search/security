---
api_specs:
- filename: uzum-checkout-openapi.yaml
  format: yaml
  label: Uzum Checkout
  slug: uzum-checkout
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-checkout-openapi.yaml
- filename: uzum-crossborder-openapi.yaml
  format: yaml
  label: Uzum CrossBorder Transfer
  slug: uzum-crossborder-transfer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-crossborder-openapi.yaml
- filename: uzum-remitcore-openapi.yaml
  format: yaml
  label: Remit Core
  slug: uzum-remit-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-remitcore-openapi.yaml
- filename: uzum-nasiya-openapi.yaml
  format: yaml
  label: Uzum Nasiya Partner API
  slug: uzum-nasiya-partner
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-nasiya-openapi.yaml
- filename: uzum-fiscalization-openapi.yaml
  format: yaml
  label: Uzum Fiscalization
  slug: uzum-fiscalization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-fiscalization-openapi.yaml
- filename: uzum-fastpay-openapi.yaml
  format: yaml
  label: Uzum Fast Pay
  slug: uzum-fast-pay
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-fastpay-openapi.yaml
- filename: uzum-dynamicqr-openapi.yaml
  format: yaml
  label: Uzum Dynamic QR
  slug: uzum-dynamic-qr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-dynamicqr-openapi.yaml
- filename: uzum-merchant-openapi.yaml
  format: yaml
  label: Uzum Merchant API
  slug: uzum-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-merchant-openapi.yaml
- filename: uzum-ratekeeper-openapi.yaml
  format: yaml
  label: Uzum RateKeeper
  slug: uzum-ratekeeper
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/openapi/uzum-ratekeeper-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uzum.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uzumbank.uz
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: uzum.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: developer.uzumbank.uz
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: crossborder.transfer.uz
  https: false
kind: domain-security
layout: security
method: probed
name: Uzum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uzum, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Uzum
provider_slug: uzum
slug: uzum-domain-security
source_filename: uzum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uzum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\n- host: developer.uzumbank.uz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: crossborder.transfer.uz\n  https: false\ndomains:\n- domain: uzum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: uzumbank.uz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uzum/refs/heads/main/security/uzum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Banking
- Financial Services
- E-Commerce
- Marketplace
- Money Transfer
- Remittances
- BNPL
- Acquiring
- QR Payments
- Fiscalization
- Banking as a Service
- Uzbekistan
- Central Asia
---
