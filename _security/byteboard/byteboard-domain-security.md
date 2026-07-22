---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: true
  domain: byteboard.dev
  spf: true
hosts:
- cert_expires: Oct  7 09:29:20 2026 GMT
  host: byteboard.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Byteboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Byteboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Byteboard
provider_slug: byteboard
slug: byteboard-domain-security
source_filename: byteboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: byteboard.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:29:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: byteboard.dev\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byteboard/refs/heads/main/security/byteboard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Future Of Work
- Technical Interviews
- Hiring
- Recruiting
- Developer Assessment
- Coding Assessment
---
