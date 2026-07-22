---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meetcleo.com
  spf: true
hosts:
- cert_expires: Oct  8 22:33:28 2026 GMT
  host: web.meetcleo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cleo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cleo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cleo
provider_slug: cleo
slug: cleo-domain-security
source_filename: cleo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: web.meetcleo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 22:33:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: meetcleo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleo/refs/heads/main/security/cleo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Banking
- Budgeting
- Cash Advance
- Consumer Finance
- Financial Assistant
- Personal Finance
---
