---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: f1ow.com
  spf: false
hosts:
- cert_expires: Dec 26 16:50:16 2026 GMT
  host: f1ow.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: f1ow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for f1ow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: f1ow
provider_slug: f1ow-com
slug: f1ow-com-domain-security
source_filename: f1ow-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: f1ow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 16:50:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: f1ow.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/f1ow-com/security/f1ow-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cryptocurrency
- Market Data
- Finance
- MCP
---
