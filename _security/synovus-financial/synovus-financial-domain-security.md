---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "amazonaws.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: synovus.com
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.synovus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: developer.synovus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.synovus.com
  https: false
kind: domain-security
layout: security
method: probed
name: Synovus Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synovus Financial, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Synovus Financial
provider_slug: synovus-financial
slug: synovus-financial-domain-security
source_filename: synovus-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synovus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.synovus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\n- host: api.synovus.com\n  https: false\ndomains:\n- domain: synovus.com\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synovus-financial/refs/heads/main/security/synovus-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Financial Services
---
