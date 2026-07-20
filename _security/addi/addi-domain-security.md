---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: addi.com
  spf: true
hosts:
- cert_expires: Aug 20 02:48:53 2026 GMT
  host: co.addi.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 02:48:53 2026 GMT
  host: api-docs-sandbox.addi.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 02:48:53 2026 GMT
  host: api.addi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Addi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Addi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Addi
provider_slug: addi
slug: addi-domain-security
source_filename: addi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: co.addi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 02:48:53 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api-docs-sandbox.addi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 02:48:53 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.addi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 02:48:53 2026 GMT\n  hsts: null\ndomains:\n- domain: addi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/addi/refs/heads/main/security/addi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Buy Now Pay Later
- Credit
- Lending
- Checkout
- E-commerce
- Latin America
- Colombia
---
