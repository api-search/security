---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eql.com
  spf: true
hosts:
- cert_expires: Oct  1 04:57:09 2026 GMT
  host: www.eql.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: portal.eql.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EQL, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EQL
provider_slug: eql
slug: eql-domain-security
source_filename: eql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:57:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.eql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eql.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eql/refs/heads/main/security/eql-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- E-Commerce
- Product Launches
- Bot Mitigation
- Fraud Prevention
- Retail
- Shopify
- Queue Management
- Fair Allocation
---
