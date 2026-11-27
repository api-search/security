---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kwcommercial.com.au
  spf: true
hosts:
- cert_expires: Feb  8 21:56:27 2027 GMT
  host: kwcommercial.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KW Commercial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KW Commercial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KW Commercial
provider_slug: kwcommercial-com-au
slug: kwcommercial-com-au-domain-security
source_filename: kwcommercial-com-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kwcommercial.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 21:56:27 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kwcommercial.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kwcommercial-com-au/security/kwcommercial-com-au-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Kitchen
- Equipment
- Australia
- Hospitality
- Supplier
---
