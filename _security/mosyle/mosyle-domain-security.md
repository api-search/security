---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mosyle.com
  spf: true
hosts:
- cert_expires: Nov 21 21:24:22 2026 GMT
  host: mosyle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 21 21:24:22 2026 GMT
  host: business.mosyle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 21 21:24:22 2026 GMT
  host: businessapi.mosyle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mosyle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mosyle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mosyle
provider_slug: mosyle
slug: mosyle-domain-security
source_filename: mosyle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mosyle.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 21:24:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: business.mosyle.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 21:24:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: businessapi.mosyle.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 21:24:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mosyle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mosyle/refs/heads/main/security/mosyle-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Apple
- Device Management
- MDM
- Endpoint Security
- Identity
- SSO
- macOS
- iOS
- IT Operations
- Security
---
