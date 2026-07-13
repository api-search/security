---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hsbc.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.hsbc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: develop.hsbc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hsbc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HSBC, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HSBC
provider_slug: hsbc
slug: hsbc-domain-security
source_filename: hsbc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hsbc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: develop.hsbc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hsbc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hsbc/refs/heads/main/security/hsbc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Banks
- Global Banking
- Open Banking
- PSD2
---
