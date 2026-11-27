---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: estroni.com.au
  spf: true
hosts:
- cert_expires: Dec 24 21:29:02 2026 GMT
  host: estroni.com.au
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Estroni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Estroni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Estroni
provider_slug: estroni-com-au
slug: estroni-com-au-domain-security
source_filename: estroni-com-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: estroni.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 21:29:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: estroni.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/estroni-com-au/security/estroni-com-au-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Activewear
- Merino
- Sustainable
- Australia
---
