---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: akoya.com
  spf: true
hosts:
- cert_expires: Sep 14 21:03:37 2026 GMT
  host: akoya.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: docs.akoya.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: api.akoya.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Akoya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akoya, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Akoya
provider_slug: akoya
slug: akoya-domain-security
source_filename: akoya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: akoya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:03:37 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: docs.akoya.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\n- host: api.akoya.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: akoya.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akoya/refs/heads/main/security/akoya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Open Banking
- Aggregator
- Tokenized
- US
- FDX
- Account Aggregation
---
