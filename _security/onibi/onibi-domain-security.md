---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: onibi.gg
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: true
  domain: tomoendlessblue.com
  spf: false
hosts:
- cert_expires: Nov  6 20:15:46 2026 GMT
  host: www.onibi.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 18:54:14 2026 GMT
  host: www.tomoendlessblue.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onibi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onibi, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Onibi
provider_slug: onibi
slug: onibi-domain-security
source_filename: onibi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onibi.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 20:15:46 2026 GMT\n  hsts: false\n- host: www.tomoendlessblue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 18:54:14 2026 GMT\n  hsts: false\ndomains:\n- domain: onibi.gg\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tomoendlessblue.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\nx-note: >-\n  www.tomoendlessblue.com (the product site for Tomo: Endless Blue) was probed by hand with the same\n  DNS/TLS/HTTP checks and appended, because probe-domain-security.py only reads Website/Portal/\n  humanURL/baseURL hosts from apis.yml and the Tomo site is carried as a Product pointer. Neither\n  host sends HSTS; neither domain publishes a CAA record; tomoendlessblue.com publishes no SPF or\n \
  \ DMARC record (onibi.gg publishes both, DMARC p=reject). Absence of a record is observed data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onibi/refs/heads/main/security/onibi-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Video Games
- Game Development
- Game Studio
- Sandbox MMO
- User Generated Content
- Procedural Generation
- Entertainment
- Consumer Software
---
