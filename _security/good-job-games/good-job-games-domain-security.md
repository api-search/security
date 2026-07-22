---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goodjobgames.com
  spf: true
hosts:
- cert_expires: Aug 22 00:23:10 2026 GMT
  host: goodjobgames.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Good Job Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Good Job Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Good Job Games
provider_slug: good-job-games
slug: good-job-games-domain-security
source_filename: good-job-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goodjobgames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 00:23:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: goodjobgames.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/good-job-games/refs/heads/main/security/good-job-games-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobile Games
- Gaming
- Mobile
- Puzzle Games
- Entertainment
- Consumer
---
