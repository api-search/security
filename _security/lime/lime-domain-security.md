---
api_specs:
- filename: lime-free-bike-status-api-openapi.yml
  format: yaml
  label: Lime Free Bike Status API
  slug: lime-free-bike-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/openapi/lime-free-bike-status-api-openapi.yml
- filename: lime-gbfs-json-api-openapi.yml
  format: yaml
  label: Lime Gbfs.json API
  slug: lime-gbfs-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/openapi/lime-gbfs-json-api-openapi.yml
- filename: lime-station-information-api-openapi.yml
  format: yaml
  label: Lime Station Information API
  slug: lime-station-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/openapi/lime-station-information-api-openapi.yml
- filename: lime-station-status-api-openapi.yml
  format: yaml
  label: Lime Station Status API
  slug: lime-station-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/openapi/lime-station-status-api-openapi.yml
- filename: lime-system-information-api-openapi.yml
  format: yaml
  label: Lime System Information API
  slug: lime-system-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/openapi/lime-system-information-api-openapi.yml
- filename: lime-vehicle-types-api-openapi.yml
  format: yaml
  label: Lime Vehicle Types API
  slug: lime-vehicle-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/openapi/lime-vehicle-types-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: li.me
  spf: true
hosts:
- cert_expires: Aug 27 18:10:46 2026 GMT
  host: www.li.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lime, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lime
provider_slug: lime
slug: lime-domain-security
source_filename: lime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.li.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 18:10:46 2026 GMT\n  hsts: null\ndomains:\n- domain: li.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lime/refs/heads/main/security/lime-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Shared Mobility
- Micromobility
- Electric Scooters
- Electric Bikes
- E-Bikes
- E-Scooters
- Transportation
- Urban Mobility
- GBFS
- MDS
- Smart Cities
- Transit
---
