---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mcp4mail.online
  spf: false
hosts:
- cert_expires: Dec 16 09:30:32 2026 GMT
  host: mcp4mail.online
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mcp4mail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mcp4mail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: mcp4mail
provider_slug: mcp4mail-online
slug: mcp4mail-online-domain-security
source_filename: mcp4mail-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcp4mail.online\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 16 09:30:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mcp4mail.online\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mcp4mail-online/security/mcp4mail-online-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Email
- Artificial Intelligence
- Open Source
- MailConnect
- MCP
---
