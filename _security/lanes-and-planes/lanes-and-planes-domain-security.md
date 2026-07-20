---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lanes-planes.com
  spf: true
hosts:
- cert_expires: Sep 17 17:15:14 2026 GMT
  host: www.lanes-planes.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 00:26:11 2026 GMT
  host: api.lanes-planes.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lanes And Planes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lanes & Planes, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lanes & Planes
provider_slug: lanes-and-planes
slug: lanes-and-planes-domain-security
source_filename: lanes-and-planes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lanes-planes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 17:15:14 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.lanes-planes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 00:26:11 2026 GMT\n  hsts: false\ndomains:\n- domain: lanes-planes.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lanes-and-planes/refs/heads/main/security/lanes-and-planes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Business Travel
- Travel Management
- Expense Management
- Spend Management
- Finance
- Accounting
- ERP Integration
- HRIS
- SaaS
- Germany
- Europe
---
