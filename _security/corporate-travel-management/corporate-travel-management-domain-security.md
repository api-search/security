---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: travelctm.com
  spf: true
hosts:
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: www.travelctm.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: au.travelctm.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: us.travelctm.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Corporate Travel Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corporate Travel Management, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Corporate Travel Management
provider_slug: corporate-travel-management
slug: corporate-travel-management-domain-security
source_filename: corporate-travel-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.travelctm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: au.travelctm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: us.travelctm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: travelctm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corporate-travel-management/refs/heads/main/security/corporate-travel-management-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Travel
- Australia
- Corporate Travel
- Travel Management Company
- Aviation
- NDC
- Distribution
- Booking
- Hotels
- Meetings and Events
---
