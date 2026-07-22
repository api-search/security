---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: endgame.com
  spf: false
hosts:
- cert_expires: Sep 29 04:44:37 2026 GMT
  host: www.endgame.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: host answers 301 to https://www.elastic.co/security/endpoint-security for every path probed; HSTS header verified on the redirect response
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Endgame Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endgame, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Endgame
provider_slug: endgame
slug: endgame-domain-security
source_filename: endgame-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.endgame.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:44:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: host answers 301 to https://www.elastic.co/security/endpoint-security for\n    every path probed; HSTS header verified on the redirect response\ndomains:\n- domain: endgame.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endgame/refs/heads/main/security/endgame-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Cybersecurity
- Endpoint Security
- Threat Detection
- Security Operations
- Acquired
---
