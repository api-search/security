---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kotak.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: bank.in
  spf: false
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: kotak.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 18 02:46:56 2026 GMT
  host: api.kotak.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 21:09:31 2026 GMT
  host: api.kotak.bank.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kotak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kotak Mahindra Bank, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kotak Mahindra Bank
provider_slug: kotak
slug: kotak-domain-security
source_filename: kotak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kotak.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kotak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:46:56 2026 GMT\n  hsts: null\n- host: api.kotak.bank.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 21:09:31 2026 GMT\n  hsts: null\ndomains:\n- domain: kotak.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bank.in\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kotak/refs/heads/main/security/kotak-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Banking
- Financial Services
- Open Banking
- Payments
- Collections
- Trade Finance
- Corporate Banking
- India
- UPI
---
