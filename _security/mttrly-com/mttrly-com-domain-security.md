---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mttrly.com
  spf: true
hosts:
- cert_expires: Jan 11 16:29:47 2027 GMT
  host: mttrly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mttrly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mttrly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mttrly
provider_slug: mttrly-com
slug: mttrly-com-domain-security
source_filename: mttrly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mttrly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 16:29:47 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mttrly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mttrly-com/security/mttrly-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Incident Response
- Artificial Intelligence
- Server Management
- DevOps
- Small Business
---
