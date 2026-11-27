---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cowork24.ch
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modelcontextprotocol.io
  spf: true
hosts:
- cert_expires: Jan 16 01:02:25 2027 GMT
  host: www.cowork24.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 09:23:29 2027 GMT
  host: registry.modelcontextprotocol.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 01:32:20 2026 GMT
  host: mcp.cowork24.ch
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: cowork24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cowork24, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: cowork24
provider_slug: cowork24-ch
slug: cowork24-ch-domain-security
source_filename: cowork24-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cowork24.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 01:02:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: registry.modelcontextprotocol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 09:23:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.cowork24.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 01:32:20 2026 GMT\n  hsts: null\ndomains:\n- domain: cowork24.ch\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: modelcontextprotocol.io\n  dnssec: false\n  caa: []\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cowork24-ch/security/cowork24-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Co-Working
- Workspace Booking
- Meeting Rooms
- Marketplace
- Switzerland
- MCP
---
