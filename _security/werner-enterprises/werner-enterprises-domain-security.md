---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: werner.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: wernerbridge.com
  spf: true
hosts:
- cert_expires: Sep 30 12:22:57 2026 GMT
  host: www.werner.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 03:59:29 2026 GMT
  host: www.wernerbridge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Werner Enterprises Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Werner Enterprises, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Werner Enterprises
provider_slug: werner-enterprises
slug: werner-enterprises-domain-security
source_filename: werner-enterprises-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.werner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:22:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.wernerbridge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:59:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: werner.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wernerbridge.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/werner-enterprises/refs/heads/main/security/werner-enterprises-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Transportation
- Logistics
- Freight
- Supply Chain
- Trucking
- EDI
- Fortune 1000
---
