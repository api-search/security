---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spglobal.com
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.spglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mcgraw Hill Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for McGraw Hill Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: McGraw Hill Financial
provider_slug: mcgraw-hill-financial
slug: mcgraw-hill-financial-domain-security
source_filename: mcgraw-hill-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: spglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcgraw-hill-financial/refs/heads/main/security/mcgraw-hill-financial-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Benchmarks
- Credit Ratings
- Finance
- Financial Services
- Fortune 500
---
