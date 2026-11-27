---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mcpdirectory.fyi
  spf: true
hosts:
- cert_expires: Jan 27 21:09:32 2027 GMT
  host: mcpdirectory.fyi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MCPDirectory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCPDirectory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MCPDirectory
provider_slug: mcpdirectory-fyi
slug: mcpdirectory-fyi-domain-security
source_filename: mcpdirectory-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpdirectory.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 21:09:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mcpdirectory.fyi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mcpdirectory-fyi/security/mcpdirectory-fyi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Directory
- MCP
- Open Data
- Tools
---
