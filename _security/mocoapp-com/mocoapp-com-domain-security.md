---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mocoapp.com
  spf: true
hosts:
- cert_expires: Jan 29 19:44:36 2027 GMT
  host: mocoapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MOCO Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MOCO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MOCO
provider_slug: mocoapp-com
slug: mocoapp-com-domain-security
source_filename: mocoapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mocoapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 19:44:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mocoapp.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mocoapp-com/security/mocoapp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ERP
- Agency Software
- Project Management
- Time Tracking
- Billing
- Resource Planning
- Integration
- Artificial Intelligence
---
