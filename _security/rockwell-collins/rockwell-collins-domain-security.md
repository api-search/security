---
api_specs:
- filename: flightaware-aeroapi-openapi.yml
  format: yaml
  label: FlightAware AeroAPI
  slug: flightaware-aeroapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockwell-collins/refs/heads/main/openapi/flightaware-aeroapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rockwellcollins.com
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "sectigo.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rtx.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.rockwellcollins.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 10:20:19 2026 GMT
  host: www.rtx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: developer.collins.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rockwell Collins Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rockwell Collins, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rockwell Collins
provider_slug: rockwell-collins
slug: rockwell-collins-domain-security
source_filename: rockwell-collins-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rockwellcollins.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.rtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:20:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.collins.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rockwellcollins.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rtx.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"sectigo.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockwell-collins/refs/heads/main/security/rockwell-collins-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Avionics
- Aerospace
- Defense
- Aviation
- Flight Deck
- Fortune 500
---
