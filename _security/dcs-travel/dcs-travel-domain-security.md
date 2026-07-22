---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dcs.travel
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: dcs.travel
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dcs Travel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DCS-Touristik (DCS Travel), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DCS-Touristik (DCS Travel)
provider_slug: dcs-travel
slug: dcs-travel-domain-security
source_filename: dcs-travel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dcs.travel\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: dcs.travel\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dcs-travel/refs/heads/main/security/dcs-travel-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Travel
- Tourism
- Cruises
- River Cruises
- Hospitality
- Germany
- Booking
---
