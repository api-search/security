---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meowwolf.com
  spf: true
hosts:
- cert_expires: Nov  3 01:18:38 2026 GMT
  host: meowwolf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meow Wolf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meow Wolf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Meow Wolf
provider_slug: meow-wolf
slug: meow-wolf-domain-security
source_filename: meow-wolf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meowwolf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 01:18:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: meowwolf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meow-wolf/refs/heads/main/security/meow-wolf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Art
- Entertainment
- Immersive Experiences
- Events
- Ticketing
- Museums
- Tourism
- Retail
- Mobile Apps
---
