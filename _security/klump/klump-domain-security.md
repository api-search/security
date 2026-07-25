---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: useklump.com
  spf: true
hosts:
- cert_expires: Sep 19 12:12:17 2026 GMT
  host: useklump.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 12:12:17 2026 GMT
  host: docs.useklump.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 12:12:17 2026 GMT
  host: api.useklump.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klump Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klump, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Klump
provider_slug: klump
slug: klump-domain-security
source_filename: klump-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: useklump.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 12:12:17 2026 GMT\n  hsts: false\n- host: docs.useklump.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 12:12:17 2026 GMT\n  hsts: false\n- host: api.useklump.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 12:12:17 2026 GMT\n  hsts: null\ndomains:\n- domain: useklump.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klump/refs/heads/main/security/klump-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Buy Now Pay Later
- BNPL
- Fintech
- Lending
- Checkout
- E-Commerce
- Nigeria
- Africa
- Instalments
- Consumer Credit
---
