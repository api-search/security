---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cuponomia.com.br
  spf: true
hosts:
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: cuponomia.com.br
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cuponomia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cuponomia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cuponomia
provider_slug: cuponomia
slug: cuponomia-domain-security
source_filename: cuponomia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cuponomia.com.br\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cuponomia.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuponomia/refs/heads/main/security/cuponomia-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Coupons
- Cashback
- Discounts
- E-commerce
- Affiliate Marketing
- Deals
- Brazil
- Consumer
---
