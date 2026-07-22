---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: makespace.com
  spf: true
hosts:
- cert_expires: Sep  6 21:38:40 2026 GMT
  host: makespace.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Makespace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for makespace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: makespace
provider_slug: makespace
slug: makespace-domain-security
source_filename: makespace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: makespace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 21:38:40 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: makespace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makespace/refs/heads/main/security/makespace-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Storage
- Consumer
- Logistics
- Moving
- Warehousing
---
