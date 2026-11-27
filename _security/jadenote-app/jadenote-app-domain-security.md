---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jadenote.app
  spf: true
hosts:
- cert_expires: Jan 29 06:21:47 2027 GMT
  host: jadenote.app
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jade Note Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jade Note, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jade Note
provider_slug: jadenote-app
slug: jadenote-app-domain-security
source_filename: jadenote-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jadenote.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 06:21:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: jadenote.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jadenote-app/security/jadenote-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Note Taking
- Collaboration
- MCP
- Productivity
- Company
---
