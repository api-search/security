---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: worldia.com
  spf: true
hosts:
- cert_expires: Jan 10 12:49:27 2027 GMT
  host: corp.worldia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 08:48:53 2026 GMT
  host: api.worldia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Worldia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Worldia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Worldia
provider_slug: worldia
slug: worldia-domain-security
source_filename: worldia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corp.worldia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 12:49:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.worldia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 08:48:53 2026 GMT\n  hsts: null\ndomains:\n- domain: worldia.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldia/refs/heads/main/security/worldia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Travel
- Tourism
- Booking
- Trip Planning
- Travel Technology
- Hospitality
- B2B2C
- White Label
- Itinerary
- Distribution
---
