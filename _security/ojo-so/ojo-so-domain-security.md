---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ojo.so
  spf: true
hosts:
- cert_expires: Jan  8 13:35:37 2027 GMT
  host: ojo.so
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ojo So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ojo-so, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ojo-so
provider_slug: ojo-so
slug: ojo-so-domain-security
source_filename: ojo-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ojo.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 13:35:37 2027 GMT\n  hsts: false\ndomains:\n- domain: ojo.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ojo-so/security/ojo-so-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Templates
- API
- Document-Generation
- MCP
---
