---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airbase.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airbase.io
  spf: true
hosts:
- cert_expires: Aug 11 19:42:47 2026 GMT
  host: www.airbase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 20:03:53 2026 GMT
  host: developer.airbase.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airbase, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Airbase
provider_slug: airbase
slug: airbase-domain-security
source_filename: airbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 19:42:47 2026 GMT\n  hsts: false\n- host: developer.airbase.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 20:03:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: airbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: airbase.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbase/refs/heads/main/security/airbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Spend Management
- Accounts Payable
- Bill Pay
- Procurement
- Corporate Cards
- Expense Management
- FinTech
- Paylocity
- Gated API
---
