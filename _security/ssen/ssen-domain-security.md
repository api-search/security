---
api_specs:
- filename: ssen-transmission-opendatasoft-explore-v2.1-openapi.json
  format: json
  label: SSEN Transmission Open Data Explore API
  slug: ssen-transmission-open-data-explore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ssen/refs/heads/main/openapi/ssen-transmission-opendatasoft-explore-v2.1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ssen.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opendatasoft.com
  spf: true
hosts:
- cert_expires: Sep  3 12:28:53 2026 GMT
  host: www.ssen.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 18:29:06 2026 GMT
  host: data.ssen.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 21:02:03 2026 GMT
  host: ssentransmission.opendatasoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ssen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scottish and Southern Electricity Networks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Scottish and Southern Electricity Networks
provider_slug: ssen
slug: ssen-domain-security
source_filename: ssen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ssen.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 12:28:53 2026 GMT\n  hsts: false\n- host: data.ssen.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:29:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ssentransmission.opendatasoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 21:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ssen.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: opendatasoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ssen/refs/heads/main/security/ssen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Grid
- Distribution Network Operator
- Transmission
- Smart Metering
- Open Data
- Flexibility
- Renewables
- DER
---
