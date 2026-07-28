---
api_specs:
- filename: ercot-public-data-api-openapi.json
  format: json
  label: ERCOT Public Data API
  slug: ercot-public-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ercot/refs/heads/main/openapi/ercot-public-data-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ercot.com
  spf: true
hosts:
- cert_expires: Oct  3 02:56:13 2026 GMT
  host: www.ercot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 19:38:20 2026 GMT
  host: developer.ercot.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 02:56:13 2026 GMT
  host: api.ercot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ercot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ERCOT, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ERCOT
provider_slug: ercot
slug: ercot-domain-security
source_filename: ercot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ercot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:56:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.ercot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:38:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.ercot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:56:13 2026 GMT\n  hsts: null\ndomains:\n- domain: ercot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ercot/refs/heads/main/security/ercot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Electricity
- Energy Markets
- Grid
- System Operator
- Texas
- Renewables
- Demand Response
- Open Data
---
