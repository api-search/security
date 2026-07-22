---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:security@tourradar.com"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tourradar.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.tourradar.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.b2b.tourradar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tourradar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TourRadar, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TourRadar
provider_slug: tourradar
slug: tourradar-domain-security
source_filename: tourradar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tourradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.b2b.tourradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tourradar.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:security@tourradar.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/security/tourradar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Tours
- Booking
- Marketplace
- Adventure Travel
- Distribution
- Affiliates
---
