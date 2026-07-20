---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coupa.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: coupahost.com
  spf: true
hosts:
- cert_expires: Oct  6 20:15:47 2026 GMT
  host: www.coupa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: compass.coupa.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
- host: your-instance.coupahost.com
  https: false
kind: domain-security
layout: security
method: probed
name: Coupa Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coupa Software, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coupa Software
provider_slug: coupa-software
slug: coupa-software-domain-security
source_filename: coupa-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coupa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 20:15:47 2026 GMT\n  hsts: null\n- host: compass.coupa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: your-instance.coupahost.com\n  https: false\ndomains:\n- domain: coupa.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: coupahost.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coupa-software/refs/heads/main/security/coupa-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Procurement
- Spend Management
- Invoicing
- Expenses
- Payments
- Supply Chain
- Sourcing
- Contracts
- ERP
---
