---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cps.com
  spf: true
hosts:
- cert_expires: Sep 14 21:15:13 2026 GMT
  host: cps.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Comprehensive Pharmacy Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comprehensive Pharmacy Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Comprehensive Pharmacy Services
provider_slug: comprehensive-pharmacy-services
slug: comprehensive-pharmacy-services-domain-security
source_filename: comprehensive-pharmacy-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:15:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comprehensive-pharmacy-services/refs/heads/main/security/comprehensive-pharmacy-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Digital Health
- Pharmacy
- Healthcare
- Specialty Pharmacy
- Telepharmacy
- Hospital
- 340B
- SaaS
---
