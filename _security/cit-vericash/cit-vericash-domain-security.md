---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: citvericash.com
  spf: true
hosts:
- cert_expires: Sep 24 13:57:33 2026 GMT
  host: www.citvericash.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cit Vericash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cit Vericash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cit Vericash
provider_slug: cit-vericash
slug: cit-vericash-domain-security
source_filename: cit-vericash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.citvericash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 13:57:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: citvericash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cit-vericash/refs/heads/main/security/cit-vericash-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fintech
- Digital Banking
- Payments
- Mobile Wallet
- Agency Banking
- Financial Inclusion
- Banking as a Service
---
