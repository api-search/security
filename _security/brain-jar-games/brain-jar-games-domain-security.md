---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brainjar.games
  spf: true
hosts:
- cert_expires: Sep 26 11:44:49 2026 GMT
  host: brainjar.games
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brain Jar Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brain Jar Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Brain Jar Games
provider_slug: brain-jar-games
slug: brain-jar-games-domain-security
source_filename: brain-jar-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brainjar.games\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 11:44:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brainjar.games\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brain-jar-games/refs/heads/main/security/brain-jar-games-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Video Games
- Gaming
- Game Studio
- Entertainment
- Interactive Media
---
