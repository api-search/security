---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bikky.com
  spf: true
hosts:
- cert_expires: Sep  4 14:47:32 2026 GMT
  host: bikky.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 15:05:01 2026 GMT
  host: www.bikky.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bikky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bikky, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bikky
provider_slug: bikky
slug: bikky-domain-security
source_filename: bikky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bikky.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 14:47:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.bikky.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:05:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bikky.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bikky/refs/heads/main/security/bikky-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Customer Data Platform
- Guest Analytics
- Integrations
- Marketing
- Loyalty
---
