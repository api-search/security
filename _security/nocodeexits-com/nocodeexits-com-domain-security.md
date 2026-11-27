---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nocodeexits.com
  spf: true
hosts:
- cert_expires: Dec 19 23:06:51 2026 GMT
  host: nocodeexits.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI and No-Code Exits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI and No-Code Exits, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AI and No-Code Exits
provider_slug: nocodeexits-com
slug: nocodeexits-com-domain-security
source_filename: nocodeexits-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nocodeexits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:06:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nocodeexits.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nocodeexits-com/security/nocodeexits-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- No-Code
- Micro-Startups
- Builder Community
- Playbooks
- Exit Strategies
- Challenge
---
