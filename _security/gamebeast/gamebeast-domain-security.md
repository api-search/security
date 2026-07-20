---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gamebeast.gg
  spf: true
hosts:
- cert_expires: Sep 12 23:35:11 2026 GMT
  host: docs.gamebeast.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 15:40:42 2026 GMT
  host: api.gamebeast.gg
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gamebeast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gamebeast, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gamebeast
provider_slug: gamebeast
slug: gamebeast-domain-security
source_filename: gamebeast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.gamebeast.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:35:11 2026 GMT\n  hsts: false\n- host: api.gamebeast.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:40:42 2026 GMT\n  hsts: null\ndomains:\n- domain: gamebeast.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamebeast/refs/heads/main/security/gamebeast-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Analytics
- Gaming
- Game Development
- LiveOps
- Experiments
- A/B Testing
- Roblox
- Unity
- Player Analytics
- Attribution
---
