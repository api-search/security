---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: playsome.fi
  spf: true
hosts:
- cert_expires: Aug 26 09:54:33 2026 GMT
  host: www.playsome.fi
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Playsome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Playsome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Playsome
provider_slug: playsome
slug: playsome-domain-security
source_filename: playsome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.playsome.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 09:54:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: playsome.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playsome/refs/heads/main/security/playsome-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Mobile Gaming
- Games
- Game Studio
- Free-to-Play
- Finland
- Consumer
- MCP
---
