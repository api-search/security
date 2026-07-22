---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: avantarte.com
  spf: true
hosts:
- cert_expires: Sep 13 21:32:15 2026 GMT
  host: avantarte.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avant Arte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avant Arte, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Avant Arte
provider_slug: avant-arte
slug: avant-arte-domain-security
source_filename: avant-arte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avantarte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 21:32:15 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: avantarte.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avant-arte/refs/heads/main/security/avant-arte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Marketplaces
- Art
- E-commerce
- Collectibles
- Contemporary Art
- Prints
---
