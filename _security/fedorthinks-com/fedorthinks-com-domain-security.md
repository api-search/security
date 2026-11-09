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
  dmarc: false
  dnssec: false
  domain: fedorthinks.com
  spf: true
hosts:
- cert_expires: Dec 10 23:36:27 2026 GMT
  host: fedorthinks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fedorthinks Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fedor Chishchin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fedor Chishchin
provider_slug: fedorthinks-com
slug: fedorthinks-com-domain-security
source_filename: fedorthinks-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fedorthinks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:36:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fedorthinks.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fedorthinks-com/security/fedorthinks-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- Engineering
- MCP
- Agents
- Software
---
