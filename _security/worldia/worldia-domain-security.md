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
- cert_expires: Nov 12 10:22:52 2026 GMT
  host: corp.worldia.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 14:33:08 2026 GMT
  host: api.worldia.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 2592000
  hsts_preload: true
  https: true
  note: 'HSTS corrected by direct probe on 2026-09-04: the automated pass recorded null because api.worldia.com answers its root path with HTTP 404, but the header is present on both the 404 root and on 200 responses — "strict-transport-security: max-age=2592000; includeSubDomains; preload". The API host carries includeSubDomains and preload, which the corporate host (max-age=31536000, neither directive) does not.'
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Worldia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Worldia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Worldia
provider_slug: worldia
slug: worldia-domain-security
source_filename: worldia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corp.worldia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 10:22:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  hsts_preload: false\n- host: api.worldia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 14:33:08 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: 'HSTS corrected by direct probe on 2026-09-04: the automated pass recorded null because api.worldia.com\n    answers its root path with HTTP 404, but the header is present on both the 404 root and on 200 responses\n    — \"strict-transport-security: max-age=2592000; includeSubDomains; preload\". The API host carries includeSubDomains\n    and preload, which the corporate host (max-age=31536000, neither directive) does not.'\ndomains:\n- domain: worldia.com\n  dnssec:\
  \ true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnote: worldia.com publishes DNSSEC, SPF and DMARC but the DMARC policy is p=none, which requests reporting\n  only and does not instruct receivers to quarantine or reject spoofed mail. No CAA record is published,\n  so any public CA may issue for the domain. No security.txt is served on any host (see well-known/worldia-well-known.yml).\n"
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
