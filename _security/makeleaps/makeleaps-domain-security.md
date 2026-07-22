---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: makeleaps.com
  spf: true
hosts:
- cert_expires: Oct 12 13:38:31 2026 GMT
  host: www.makeleaps.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 06:41:52 2026 GMT
  host: developer.makeleaps.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 07:29:48 2026 GMT
  host: api.makeleaps.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Makeleaps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MakeLeaps, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MakeLeaps
provider_slug: makeleaps
slug: makeleaps-domain-security
source_filename: makeleaps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.makeleaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 13:38:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.makeleaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 06:41:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.makeleaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 07:29:48 2026 GMT\n  hsts: null\ndomains:\n- domain: makeleaps.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makeleaps/refs/heads/main/security/makeleaps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Invoicing
- Billing
- Accounting
- Finance
- Payments
- Document Management
- E-Invoicing
- SaaS
- Japan
- Ricoh
---
