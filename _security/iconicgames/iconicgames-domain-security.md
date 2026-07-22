---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iconicgames.io
  spf: true
hosts:
- cert_expires: Sep  5 20:39:26 2026 GMT
  host: iconicgames.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iconicgames Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iconicgames, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Iconicgames
provider_slug: iconicgames
slug: iconicgames-domain-security
source_filename: iconicgames-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iconicgames.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:39:26 2026 GMT\n  hsts: false\ndomains:\n- domain: iconicgames.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iconicgames/refs/heads/main/security/iconicgames-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Games
- Gaming
- Game Development
- Artificial Intelligence
- Interactive Storytelling
- Real-time AI
---
