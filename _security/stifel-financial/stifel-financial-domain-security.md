---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: stifel.com
  spf: true
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fintable.io
  spf: true
hosts:
- cert_expires: Aug 31 11:55:22 2026 GMT
  host: www.stifel.com
  hsts: true
  hsts_max_age: 3153600
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 19:06:50 2026 GMT
  host: fintable.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stifel Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stifel Financial, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Stifel Financial
provider_slug: stifel-financial
slug: stifel-financial-domain-security
source_filename: stifel-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stifel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 11:55:22 2026 GMT\n  hsts: true\n  hsts_max_age: 3153600\n- host: fintable.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 19:06:50 2026 GMT\n  hsts: false\ndomains:\n- domain: stifel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: fintable.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stifel-financial/refs/heads/main/security/stifel-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Wealth Management
- Investment Banking
- Open Banking
- Financial Services
- Fortune 1000
---
