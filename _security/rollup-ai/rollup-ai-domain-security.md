---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: rollup.ai
  spf: false
hosts:
- cert_expires: Sep 24 03:32:05 2026 GMT
  host: rollup.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 16:28:42 2026 GMT
  host: api.rollup.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rollup Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rollup AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Rollup AI
provider_slug: rollup-ai
slug: rollup-ai-domain-security
source_filename: rollup-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rollup.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:32:05 2026 GMT\n  hsts: null\n- host: api.rollup.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:28:42 2026 GMT\n  hsts: null\ndomains:\n- domain: rollup.ai\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rollup-ai/refs/heads/main/security/rollup-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Hardware Engineering
- Systems Engineering
- Requirements Management
- Product Lifecycle Management
- Collaboration
- CAD
- Aerospace
- Robotics
- Developer Tools
---
