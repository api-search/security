---
api_specs:
- filename: ordnance-survey-ngd-features-openapi.json
  format: json
  label: OS NGD API - Features
  slug: os-ngd-api-features
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-ngd-features-openapi.json
- filename: ordnance-survey-ngd-tiles-openapi.json
  format: json
  label: OS NGD API - Tiles
  slug: os-ngd-api-tiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-ngd-tiles-openapi.json
- filename: ordnance-survey-downloads-openapi.yaml
  format: yaml
  label: OS Downloads API
  slug: os-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-downloads-openapi.yaml
- filename: ordnance-survey-osnet-openapi.yaml
  format: yaml
  label: OS Net API
  slug: os-net-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-osnet-openapi.yaml
- filename: ordnance-survey-places-openapi.json
  format: json
  label: OS Places API
  slug: os-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-places-openapi.json
- filename: ordnance-survey-names-openapi.json
  format: json
  label: OS Names API
  slug: os-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-names-openapi.json
- filename: ordnance-survey-linked-identifiers-openapi.json
  format: json
  label: OS Linked Identifiers API
  slug: os-linked-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-linked-identifiers-openapi.json
- filename: ordnance-survey-features-wfs-openapi.json
  format: json
  label: OS Features API
  slug: os-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-features-wfs-openapi.json
- filename: ordnance-survey-maps-openapi.json
  format: json
  label: OS Maps API
  slug: os-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-maps-openapi.json
- filename: ordnance-survey-vector-tile-openapi.json
  format: json
  label: OS Vector Tile API
  slug: os-vector-tile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/openapi/ordnance-survey-vector-tile-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ordnancesurvey.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: os.uk
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.ordnancesurvey.co.uk
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 11:25:42 2026 GMT
  host: docs.os.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.os.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ordnance Survey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ordnance Survey, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ordnance Survey
provider_slug: ordnance-survey
slug: ordnance-survey-domain-security
source_filename: ordnance-survey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ordnancesurvey.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: docs.os.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 11:25:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.os.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: ordnancesurvey.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: os.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ordnance-survey/refs/heads/main/security/ordnance-survey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United Kingdom
- Land Registry
- Geospatial
- Addressing
- Open Data
- Property Data
- PropTech
- Government
- Mapping
- OGC
- UPRN
- National Mapping
- GNSS
- Vector Tiles
---
