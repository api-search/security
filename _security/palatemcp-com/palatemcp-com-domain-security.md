---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: palatemcp.com
  spf: true
hosts:
- cert_expires: Jan  6 17:56:40 2027 GMT
  host: palatemcp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Palate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Palate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Palate
provider_slug: palatemcp-com
slug: palatemcp-com-domain-security
source_filename: palatemcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: palatemcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 17:56:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: palatemcp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/palatemcp-com/security/palatemcp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Design
- Website Builder
- MCP
- Design Tokens
---
