---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: swap-commerce.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: api-swap-os.com
  spf: false
hosts:
- cert_expires: Sep 14 16:56:12 2026 GMT
  host: www.swap-commerce.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 19:19:48 2026 GMT
  host: docs.api-swap-os.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 19:19:48 2026 GMT
  host: prod-ws-gateway.api-swap-os.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swap, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Swap
provider_slug: swap
slug: swap-domain-security
source_filename: swap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swap-commerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 16:56:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.api-swap-os.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 19:19:48 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: prod-ws-gateway.api-swap-os.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 19:19:48 2026 GMT\n  hsts: null\ndomains:\n- domain: swap-commerce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: api-swap-os.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swap/refs/heads/main/security/swap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Cross-Border
- Customs
- Shipping
- Returns
- Tax
- Duties
- Agentic Commerce
- Checkout
- Package Protection
- Landed Cost
---
