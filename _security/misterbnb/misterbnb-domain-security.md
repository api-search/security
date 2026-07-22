---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: misterbandb.com
  spf: true
hosts:
- cert_expires: Sep 21 07:45:12 2026 GMT
  host: misterbandb.com
  hsts: true
  hsts_max_age: 63113904
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Misterbnb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MisterBnB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MisterBnB
provider_slug: misterbnb
slug: misterbnb-domain-security
source_filename: misterbnb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: misterbandb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:45:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63113904\ndomains:\n- domain: misterbandb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/misterbnb/refs/heads/main/security/misterbnb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Accommodation
- Booking
- Vacation Rental
- Marketplace
- LGBTQ
- Hospitality
---
