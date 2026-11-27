---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inkfe.com
  spf: true
hosts:
- cert_expires: Jan 11 14:45:14 2027 GMT
  host: inkfe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: InkFE Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InkFE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: InkFE
provider_slug: inkfe-com
slug: inkfe-com-domain-security
source_filename: inkfe-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inkfe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 14:45:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: inkfe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/inkfe-com/security/inkfe-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Printing
- E-Commerce
- Custom Design
- Marketing Materials
- United States
---
