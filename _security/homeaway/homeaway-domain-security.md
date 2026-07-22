---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: homeaway.com
  spf: true
hosts:
- cert_expires: Sep 22 11:54:28 2026 GMT
  host: www.homeaway.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Homeaway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HomeAway *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HomeAway *
provider_slug: homeaway
slug: homeaway-domain-security
source_filename: homeaway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.homeaway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:54:28 2026 GMT\n  hsts: null\ndomains:\n- domain: homeaway.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homeaway/refs/heads/main/security/homeaway-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Vacation Rentals
- Travel
- Hospitality
- Marketplace
- Bookings
- Property Management
---
