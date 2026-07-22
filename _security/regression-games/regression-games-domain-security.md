---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: regression.gg
  spf: false
hosts:
- cert_expires: Oct 11 17:16:06 2026 GMT
  host: regression.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Regression Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regression Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Regression Games
provider_slug: regression-games
slug: regression-games-domain-security
source_filename: regression-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: regression.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 17:16:06 2026 GMT\n  hsts: false\ndomains:\n- domain: regression.gg\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regression-games/refs/heads/main/security/regression-games-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Gaming
- Game Development
- Testing
- Quality Assurance
- Unity
- Bots
- Agents
- SDK
---
