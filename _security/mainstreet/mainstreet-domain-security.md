---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mainstreet.ai
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mainstreet.com
  spf: true
hosts:
- cert_expires: Sep 17 19:37:48 2026 GMT
  host: mainstreet.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 10:36:11 2026 GMT
  host: login.mainstreet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mainstreet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MainStreet, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MainStreet
provider_slug: mainstreet
slug: mainstreet-domain-security
source_filename: mainstreet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mainstreet.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:37:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: login.mainstreet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 10:36:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mainstreet.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: mainstreet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mainstreet/refs/heads/main/security/mainstreet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tax
- Tax Credits
- Accounting
- Financial-Services
- Small Business
- Fintech
- Bookkeeping
- Compliance
- Payroll
---
