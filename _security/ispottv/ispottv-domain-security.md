---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ispot.tv
  spf: true
hosts:
- cert_expires: Sep 28 12:53:03 2026 GMT
  host: www.ispot.tv
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: developer.ispot.tv
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: api.ispot.tv
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ispottv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iSpot.tv, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iSpot.tv
provider_slug: ispottv
slug: ispottv-domain-security
source_filename: ispottv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ispot.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:53:03 2026 GMT\n  hsts: false\n- host: developer.ispot.tv\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ispot.tv\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ispot.tv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ispottv/refs/heads/main/security/ispottv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- TV Advertising
- Advertising Measurement
- Analytics
- Attribution
- Media
- Marketing
- Streaming
---
