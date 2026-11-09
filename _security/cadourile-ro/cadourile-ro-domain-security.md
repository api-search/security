---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cadourile.ro
  spf: false
hosts:
- cert_expires: Jan 13 17:51:16 2027 GMT
  host: cadourile.ro
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cadourile Ro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cadourile.ro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Cadourile.ro
provider_slug: cadourile-ro
slug: cadourile-ro-domain-security
source_filename: cadourile-ro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cadourile.ro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 17:51:16 2027 GMT\n  hsts: false\ndomains:\n- domain: cadourile.ro\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cadourile-ro/security/cadourile-ro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Gifts
- Event
- Wishlist
- Romania
- Free
---
