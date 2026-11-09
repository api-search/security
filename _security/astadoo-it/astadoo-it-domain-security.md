---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: astadoo.it
  spf: true
hosts:
- cert_expires: Jan 27 11:13:51 2027 GMT
  host: astadoo.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Astadoo It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AstaDoo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AstaDoo
provider_slug: astadoo-it
slug: astadoo-it-domain-security
source_filename: astadoo-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astadoo.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 11:13:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: astadoo.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/astadoo-it/security/astadoo-it-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Auctions
- Artificial Intelligence
- Italy
- Legal Tech
---
