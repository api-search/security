---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: travelier.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seatos.com
  spf: true
hosts:
- cert_expires: Nov 18 22:09:14 2026 GMT
  host: www.travelier.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: www.seatos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Travelier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Travelier, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Travelier
provider_slug: travelier
slug: travelier-domain-security
source_filename: travelier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.travelier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 22:09:14 2026 GMT\n  hsts: false\n- host: www.seatos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: travelier.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: seatos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelier/refs/heads/main/security/travelier-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Transportation
- Ground Transportation
- Ferries
- Bus
- Trains
- Booking
- Marketplace
- Distribution
---
