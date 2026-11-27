---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: checklaurel.com
  spf: false
hosts:
- cert_expires: May  8 23:59:59 2027 GMT
  host: checklaurel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Laurel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laurel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Laurel
provider_slug: checklaurel-com
slug: checklaurel-com-domain-security
source_filename: checklaurel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: checklaurel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: checklaurel.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/checklaurel-com/security/checklaurel-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer Products
- E-Commerce
- Product Discovery
- Low Tox
- Sustainability
- MCP
- Shopping
---
