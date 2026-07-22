---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: air-dr.com
  spf: true
hosts:
- cert_expires: Aug 19 06:03:40 2026 GMT
  host: www.air-dr.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Air Doctor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Air Doctor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Air Doctor
provider_slug: air-doctor
slug: air-doctor-domain-security
source_filename: air-doctor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.air-dr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 06:03:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: air-dr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/air-doctor/refs/heads/main/security/air-doctor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Health
- Telemedicine
- Healthcare
- Travel
- Travel Insurance
- Medical Services
- Health Tech
---
