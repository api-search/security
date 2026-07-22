---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shuttlecentral.com
  spf: true
hosts:
- cert_expires: Sep 10 07:37:11 2026 GMT
  host: shuttlecentral.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Shuttle Central Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shuttle Central, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shuttle Central
provider_slug: shuttle-central
slug: shuttle-central-domain-security
source_filename: shuttle-central-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shuttlecentral.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 07:37:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shuttlecentral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shuttle-central/refs/heads/main/security/shuttle-central-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Travel
- Transportation
- Ground Transportation
- Airport Shuttle
- Booking
- Hospitality
- Mexico
- Caribbean
---
