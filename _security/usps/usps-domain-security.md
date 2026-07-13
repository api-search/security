---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usps.com
  spf: true
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: www.usps.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: developers.usps.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: apis.usps.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Usps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for USPS, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: USPS
provider_slug: usps
slug: usps-domain-security
source_filename: usps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.usps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apis.usps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: usps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usps/refs/heads/main/security/usps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shipping
- Postal
- Address Validation
- Tracking
- Labels
- Logistics
---
