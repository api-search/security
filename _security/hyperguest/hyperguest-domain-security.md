---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hyperguest.com
  spf: true
hosts:
- cert_expires: Sep  9 06:59:48 2026 GMT
  host: www.hyperguest.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: api.hyperguest.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperguest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperguest, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hyperguest
provider_slug: hyperguest
slug: hyperguest-domain-security
source_filename: hyperguest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hyperguest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 06:59:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hyperguest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hyperguest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperguest/refs/heads/main/security/hyperguest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hospitality
- Hotels
- Travel
- Distribution
- Connectivity
- Booking
- Payments
---
