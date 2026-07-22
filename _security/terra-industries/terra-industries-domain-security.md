---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: terraindustries.co
  spf: false
hosts:
- cert_expires: Oct 16 05:19:16 2026 GMT
  host: terraindustries.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terra Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terra Industries, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Terra Industries
provider_slug: terra-industries
slug: terra-industries-domain-security
source_filename: terra-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: terraindustries.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 05:19:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: terraindustries.co\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terra-industries/refs/heads/main/security/terra-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Defense
- Defense Technology
- Autonomous Systems
- Drones
- Robotics
- Security
- Hardware
- Artificial Intelligence
- Africa
---
