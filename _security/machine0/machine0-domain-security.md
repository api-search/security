---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: machine0.io
  spf: true
hosts:
- cert_expires: Oct 17 02:47:41 2026 GMT
  host: machine0.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 04:16:31 2026 GMT
  host: docs.machine0.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 02:47:41 2026 GMT
  host: app.machine0.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Machine0 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Machine0, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Machine0
provider_slug: machine0
slug: machine0-domain-security
source_filename: machine0-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: machine0.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 02:47:41 2026 GMT\n  hsts: false\n- host: docs.machine0.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 04:16:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.machine0.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 02:47:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: machine0.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/machine0/refs/heads/main/security/machine0-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Cloud
- Infrastructure
- Virtual Machines
- AI Agents
- Developer Tools
- CLI
- MCP
---
