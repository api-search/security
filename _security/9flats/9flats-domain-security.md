---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 9flats.com
  spf: true
hosts:
- cert_expires: Oct 31 14:40:30 2026 GMT
  host: www.9flats.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 9Flats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 9flats, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 9flats
provider_slug: 9flats
slug: 9flats-domain-security
source_filename: 9flats-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.9flats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 14:40:30 2026 GMT\n  hsts: null\ndomains:\n- domain: 9flats.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/9flats/refs/heads/main/security/9flats-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Hospitality
- Vacation Rentals
- Short-Term Rental
- Accommodation
- Marketplace
- Booking
- Europe
---
