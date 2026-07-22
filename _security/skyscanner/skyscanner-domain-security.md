---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: skyscanner.net
  spf: true
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: www.skyscanner.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skyscanner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skyscanner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Skyscanner
provider_slug: skyscanner
slug: skyscanner-domain-security
source_filename: skyscanner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skyscanner.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: skyscanner.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyscanner/refs/heads/main/security/skyscanner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Travel Search
- Flights
- Hotels
- Car Hire
- Metasearch
- Affiliate
- Distribution
- Online Travel Agency
- Trip.com Group
---
