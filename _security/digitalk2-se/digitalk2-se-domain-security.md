---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: digitalk2.se
  spf: true
hosts:
- cert_expires: Jan 19 08:58:41 2027 GMT
  host: digitalk2.se
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DigitalK2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DigitalK2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DigitalK2
provider_slug: digitalk2-se
slug: digitalk2-se-domain-security
source_filename: digitalk2-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digitalk2.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 08:58:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: digitalk2.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/digitalk2-se/security/digitalk2-se-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Accounting
- Annual Reports
- Bolagsverket
- Sweden
- SIE
- Small Business
- Tax
- MCP
---
