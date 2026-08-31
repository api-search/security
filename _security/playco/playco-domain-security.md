---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: play.co
  spf: true
hosts:
- cert_expires: Oct 16 11:29:33 2026 GMT
  host: www.play.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Playco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Playco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Playco
provider_slug: playco
slug: playco-domain-security
source_filename: playco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.play.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 11:29:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: play.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playco/refs/heads/main/security/playco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Games
- Instant Games
- HTML5
- Game Engine
- Mobile Games
- Social Gaming
- Developer Tools
- Open-Source
---
