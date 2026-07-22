---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tourlane.com
  spf: true
hosts:
- cert_expires: Sep 12 19:15:20 2026 GMT
  host: www.tourlane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tourlane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tourlane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tourlane
provider_slug: tourlane
slug: tourlane-domain-security
source_filename: tourlane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tourlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 19:15:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tourlane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tourlane/refs/heads/main/security/tourlane-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Travel
- Trip Planning
- Tours
- Booking
- Tailor-Made Trips
---
