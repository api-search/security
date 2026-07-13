---
api_specs:
- filename: bird-gbfs-openapi.yml
  format: yaml
  label: Bird GBFS Feed
  slug: bird-gbfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird-rides/refs/heads/main/openapi/bird-gbfs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bird.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: birdapp.com
  spf: true
hosts:
- cert_expires: Sep 23 21:45:08 2026 GMT
  host: www.bird.co
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: city-data.bird.co
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.birdapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bird Rides Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bird, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bird
provider_slug: bird-rides
slug: bird-rides-domain-security
source_filename: bird-rides-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bird.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:45:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: city-data.bird.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.birdapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bird.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: birdapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bird-rides/refs/heads/main/security/bird-rides-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Micromobility
- Shared Mobility
- Electric Scooters
- E-Scooters
- E-Bikes
- Bikeshare
- Transportation
- Urban Mobility
- GBFS
- General Bikeshare Feed Specification
- Mobility Data Specification
- MDS
- Geofencing
- Cities
- Smart Cities
- Fleet Management
- Third Lane Mobility
---
