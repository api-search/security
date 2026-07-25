---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cuscal.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cuscalpaymentshub.com.au
  spf: false
hosts:
- cert_expires: Sep 14 02:59:49 2026 GMT
  host: www.cuscal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: www.cuscalpaymentshub.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cuscal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cuscal, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cuscal
provider_slug: cuscal
slug: cuscal-domain-security
source_filename: cuscal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cuscal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 02:59:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.cuscalpaymentshub.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cuscal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cuscalpaymentshub.com.au\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuscal/refs/heads/main/security/cuscal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Australia
- Card Issuing
- Issuer Processor
- Real-Time Payments
- Acquiring
- Open Banking
- Consumer Data Right
- Account-to-Account
- Fraud
- Banking-as-a-Service
---
