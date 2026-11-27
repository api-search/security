---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dreamtap.xyz
  spf: true
hosts:
- cert_expires: Dec 12 23:00:23 2026 GMT
  host: dreamtap.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dreamtap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dreamtap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dreamtap
provider_slug: dreamtap-xyz
slug: dreamtap-xyz-domain-security
source_filename: dreamtap-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dreamtap.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:00:23 2026 GMT\n  hsts: false\ndomains:\n- domain: dreamtap.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dreamtap-xyz/security/dreamtap-xyz-domain-security.yml
summary_line: TLSv1.3
tags:
- Creative AI
- MCP
- Inspiration tool
---
