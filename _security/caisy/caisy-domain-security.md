---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: caisy.io
  spf: true
hosts:
- cert_expires: Aug 16 08:09:46 2026 GMT
  host: caisy.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 19:43:50 2026 GMT
  host: cloud.caisy.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caisy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caisy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Caisy
provider_slug: caisy
slug: caisy-domain-security
source_filename: caisy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caisy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 08:09:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.caisy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 19:43:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: caisy.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caisy/refs/heads/main/security/caisy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GraphQL
- Headless CMS
- Content Management
- Content API
- Multi-site
---
