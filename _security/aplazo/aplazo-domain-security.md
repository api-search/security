---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aplazo.mx
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: aplazo.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: api.aplazo.mx
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Aplazo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aplazo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aplazo
provider_slug: aplazo
slug: aplazo-domain-security
source_filename: aplazo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aplazo.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\n- host: api.aplazo.mx\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: aplazo.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aplazo/refs/heads/main/security/aplazo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- BNPL
- Buy Now Pay Later
- Installments
- Fintech
- Lending
- Mexico
- Checkout
- E-commerce
---
