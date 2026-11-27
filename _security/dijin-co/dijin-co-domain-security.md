---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dijin.co
  spf: true
hosts:
- cert_expires: Jan 21 15:00:57 2027 GMT
  host: dijin.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dijin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dijin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dijin
provider_slug: dijin-co
slug: dijin-co-domain-security
source_filename: dijin-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dijin.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 15:00:57 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: dijin.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dijin-co/security/dijin-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Memory
- MCP
- Personal Data
- Privacy
- OAuth
---
