---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gread.dev
  spf: false
hosts:
- cert_expires: Jan 30 16:07:36 2027 GMT
  host: gread.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gread Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gread, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Gread
provider_slug: gread-dev
slug: gread-dev-domain-security
source_filename: gread-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gread.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 16:07:36 2027 GMT\n  hsts: false\ndomains:\n- domain: gread.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gread-dev/security/gread-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Source Code Access
- Open Source
- AI Agents
- MCP
- Coding Tools
---
