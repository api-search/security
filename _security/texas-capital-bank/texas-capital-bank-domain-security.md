---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: texascapitalbank.com
  spf: true
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
  domain: fintable.io
  spf: true
hosts:
- cert_expires: Oct  6 21:48:12 2026 GMT
  host: texascapitalbank.com
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 21:25:25 2026 GMT
  host: fintable.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Texas Capital Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Texas Capital Bank, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Texas Capital Bank
provider_slug: texas-capital-bank
slug: texas-capital-bank-domain-security
source_filename: texas-capital-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: texascapitalbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:48:12 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\n- host: fintable.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 21:25:25 2026 GMT\n  hsts: false\ndomains:\n- domain: texascapitalbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fintable.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/texas-capital-bank/refs/heads/main/security/texas-capital-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- United States
- Commercial Banking
- Treasury Management
- Regional Bank
- Open Finance
- Data Aggregation
---
