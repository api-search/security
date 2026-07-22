---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: instaplay.ai
  spf: false
hosts:
- cert_expires: Sep 28 20:21:00 2026 GMT
  host: instaplay.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instaplay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instaplay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Instaplay
provider_slug: instaplay
slug: instaplay-domain-security
source_filename: instaplay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instaplay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:21:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: instaplay.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instaplay/refs/heads/main/security/instaplay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Artificial Intelligence
- Gaming
- Multiplayer
- No-Code
- Game Development
- Social
- Generative AI
---
