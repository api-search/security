---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: anar.biz
  spf: false
hosts:
- cert_expires: Aug 25 06:09:04 2026 GMT
  host: anar.biz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Anar
provider_slug: anar
slug: anar-domain-security
source_filename: anar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anar.biz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 06:09:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: anar.biz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anar/refs/heads/main/security/anar-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Mobile
- Marketplace
- B2B
- E-Commerce
- India
- SMB
- Defunct
---
