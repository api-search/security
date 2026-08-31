---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: op.gg
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: op.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opgg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OPGG, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OPGG
provider_slug: opgg
slug: opgg-domain-security
source_filename: opgg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: op.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: op.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opgg/refs/heads/main/security/opgg-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Esports
- Game Data
- Analytics
- League of Legends
- Valorant
- Statistics
- MCP
---
