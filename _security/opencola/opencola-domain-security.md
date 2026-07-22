---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opencola.io
  spf: true
hosts:
- cert_expires: Aug 27 20:36:18 2026 GMT
  host: opencola.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opencola Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenCola, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenCola
provider_slug: opencola
slug: opencola-domain-security
source_filename: opencola-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opencola.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:36:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: opencola.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opencola/refs/heads/main/security/opencola-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Open Source
- Decentralization
- Local-First
- Personal Data
- Privacy
- Social Software
- Non-Profit
---
