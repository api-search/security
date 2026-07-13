---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: db.com
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: www.db.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: developer.db.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deutsche Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deutsche Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Deutsche Bank
provider_slug: deutsche-bank
slug: deutsche-bank-domain-security
source_filename: deutsche-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.db.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: false\n- host: developer.db.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: db.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deutsche-bank/refs/heads/main/security/deutsche-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Financial
- Wealth Management
- Open Banking
- PSD2
---
