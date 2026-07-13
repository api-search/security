---
api_specs:
- filename: travelcenters-of-america-openapi.yml
  format: yaml
  label: TravelCenters of America API
  slug: travelcenters-of-america
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelcenters-of-america/refs/heads/main/openapi/travelcenters-of-america-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ta-petro.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: accessta.com
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: www.ta-petro.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: developer.accessta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: api.accessta.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Travelcenters Of America Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TravelCenters of America, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TravelCenters of America
provider_slug: travelcenters-of-america
slug: travelcenters-of-america-domain-security
source_filename: travelcenters-of-america-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ta-petro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.accessta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.accessta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ta-petro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: accessta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelcenters-of-america/refs/heads/main/security/travelcenters-of-america-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel Centers
- Truck Service
- Retail
- Fuel
- Locations
- Trucking
- Fleet Management
- Fortune 500
---
