---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: triumpharcade.com
  spf: true
hosts:
- cert_expires: Oct  4 14:03:17 2026 GMT
  host: triumpharcade.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Triumph Arcade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Triumph Arcade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Triumph Arcade
provider_slug: triumph-arcade
slug: triumph-arcade-domain-security
source_filename: triumph-arcade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: triumpharcade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:03:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: triumpharcade.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triumph-arcade/refs/heads/main/security/triumph-arcade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Gaming
- Mobile Apps
- Entertainment
- Skill Games
---
